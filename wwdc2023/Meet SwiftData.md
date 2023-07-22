# Meet SwiftData
## WWDC 2023
[Meet SwiftData - WWDC23][Meet SwiftData]

---
- [Intro](#intro)
- [Using the model Macro](#using-the-model-macro)
  - [Adding @Model](#adding-model-to-trip)
  - [Attributes](#attributes)
  - [Relationships](#relationships)
  - [Additional Metadata](#additional-metadata)
- [Working with your data](#working-with-your-data)
  - [ModelContainer](#modelcontainer)
  - [ModelContext](#modelcontext)
  - [Fetching your data](#fetching-your-data)
    - [Predicate](#predicate)
    - [FetchDescriptor](#fetchdescriptor)
    - [SortDescriptor](#sortdescriptor)
- [Use SwiftData with SwiftUI](#use-swiftdata-with-swiftui)
    - [View Modifiers](#view-modifiers)
    - [Observing Changes](#observing-changes)
- [Wrap-up](#wrap-up)

---

## Intro
- framework for data modeling and management
- enhances your modern Swift app
- Like SwiftUI, it focuses entirely on code with no external file formats
- uses Swift's new macro system to create a seamless API experience.
- It is naturally integrated with SwiftUI and works with other platform features, like CloudKit and Widgets.

new `@Model` macro
- to model your data directly from Swift code

## Using the model Macro
`@Model` is a new Swift macro
- Powerful new Swift macro
- Define your model's schema from your Swift code
- Add SwiftData functionality to model types

SwiftData schemas are normal Swift code, but when needed, you can annotate your properties with additional metadata. Using this schema, SwiftData adds powerful functionality to your model objects.
 
 #### Adding @Model to Trip
```swift
class Trip {
    var name: String
    var destination: String
    var endDate: Date
    var startDate: Date

    var bucketList: [BucketListItem]? = []
    var livingAccomodation: LivingAccomodation?
}
```
Decorate your class with `@Model``, and the schema is generated.
```swift
import SwiftData

@Model
class Trip {
    ...
}
```

Models in SwiftData are the source of truth for your application's schema and drive the persistence experience. 
- transform the class' stored properties and turns them into persisted properties.

#### Attributes
- Attributes inferred from properties.
    - SwiftData natively adapts your value type properties to be used as attributes right away.
- Support for basic value types
    - string, int, and float.
- Complex value types
    - structs, enums, and codable types, including collections.

#### Relationships 

Relationships are inferred from reference types
- Other model types
- Collections of model types

SwiftData models reference types as relationships. You can create links between your model types with relationships and collections of model types.

#### Additional Metadata
- `@Model`modifies all the stored properties on your type.
- Control how SwiftData builds your schema using metadata on your properties
    - `@Attribute`
        - add uniqueness constraints
    - `@Relationship`
        - control the choice of inverses
        - specify delete propagation rules

    These change the behaviors of links between models.

- Exclude properties with `@Transient`
    - tell SwiftData not to include specific properties with the Transient macro.
    
```swift
// providing additional metadata

import SwiftData

@Model
class Trip {
    // specify that this property should be unique
    @Attribute(.unique) var name: String

    var destination: String
    var endDate: Date
    var startDate: Date

    // instruct Swift Data to delete all the related bucket list items whenever this trip is deleted
    @Relationship(.cascade) var bucketList: [BucketListItem]? = []

    var livingAccomodation: LivingAccomodation?
}
```

For more, see: [Model your schema with SwiftData - WWDC23][Model your schema with SwiftData]

## Working with your Data

SwiftData's two key objects to drive operations:
- ModelContainer
- ModelContext

### ModelContainer
- Provides Persistence backend for your model types.
- Customized with configurations
- Provides schema migration options

(Use default settings just by specifying your schema)

You can create a model container just by specifying the list of model types you want stored. 
```swift
import SwiftData

let container = try ModelContainer([Trip.self, LivingAccommodation.self])
```

If you want to customize your container further, you can use a configuration to change your URL, CloudKit and group container identifiers, and migration options
```swift
import SwiftData

let container = try ModelContainer(
    for: [Trip.self, LivingAccommodation.self],
    configurations: ModelConfiguration(url: URL("path"))
)
```

With your container set up, you're ready to fetch and save data with model contexts.
```swift
import SwiftData
import SwiftUI

@main
struct TripsApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
        .modelContainer(
            for: [
                Trip.self,
                LivingAccommodation.self
            ]
        )
    }
}

let container = try ModelContainer([Trip.self, LivingAccommodation.self])
```

You can also use SwiftUI's view and scene modifiers to set up container and have it automatically established in the view's environment. 

### ModelContext
- Tracking udpates
- Fetching models
- Saving changes
- Undoing changes

In SwiftUI, you'll generally get the modelContext from your view's environment after you create your model container.

Outside the view hierarchy, you can ask the model container to give you a shared main actor bound context
```swift
import SwiftData

let context = container.mainContext
```
or you can simply instantiate new contexts for a given model container. 
```swift
import SwiftData

let context = ModelContext(container)
```

### Fetching your data
Once you have a context, you're ready to fetch data.

- New Swift native types
    - `Predicate`
    - `FetchDescriptor`
- Improvements to `SortDescriptor`


#### Predicate
- Fully type checked modern replacement for NSPredicate
- `#Predicate` construction instead of text parsing
- Autocompleted keypaths, with Xcode support

e.g.
```swift
// all the trips whose destination is New York
let tripPredicate  #Predicate<Trip> { $0.destination == "New York" }
```

```swift
// all the trips about birthdays, whose destination is New York
let tripPredicate  #Predicate<Trip> { 
    $0.destination == "New York" &&
    $0.name.contains("birthday")
}
```

```swift
// all the trips about birthdays, whose destination is New York
// and planned for the future
let today = Date()
let tripPredicate  #Predicate<Trip> { 
    $0.destination == "New York" &&
    $0.name.contains("birthday") &&
    $0.startDate > today
}
```
#### FetchDescriptor
Use the new FetchDescriptor type and instruct your ModelContext to fetch those trips.
```swift
let descriptor = FetchDescriptor<Trip>(predicate: tripPredicate)
let trips = try context.fetch(desriptor)
```

More FetchDescriptor options
- Relationships to prefetch
- Result limits
- Exclude unsaved changes

#### SortDescriptor
- updates to support all `Comparable` types
- Swift native keypaths

We can use SortDescriptor to specify the order in which we'd like our fetched Trips to be organized.
```swift
let descriptor = FetchDescriptor<Trip>(
    sortBy: SortDescriptor(\Trip.name),
    predicate: tripPredicate
)
let trips = try context.fetch(desriptor)
```

#### Modifying your data

Basic operations
- Inserting
- Deleting
- Saving
- Changing

```swift
var myTrip = Trip(
    name: "Birthday trip",
    destination: "New York"
)

// inserting object
context.insert(myTrip)

// deleting object
context.delete(myTrip)

// saving
try context.save()
```

- `@Model` macro modifies setters for change tracking and observation
- Updates automatically by the `ModelContext`

For more, see [Dive deeper into SwiftData][Dive deeper into SwiftData]


## Use SwiftData with SwiftUI
- seamless integration with SwiftUI
- Easy configuration
- Automatically fetch data and update views

### View Modifiers
- Leverage scene and view modifiers
- Configure data store with `.modelContainer`
- Propagated throughout SwiftUI environment

With SwiftUI, you can configure your data store, change your options, enable undo, and toggle autosaving. SwiftUI will propagate your model context in its environment. 

Once you've set up, the easiest way to start using your data is the new `@Query` property wrapper.
```swift
import SwiftData
import SwiftUI

struct ContentView: View {
    @Query(sort: \.startDate, order: .reverse) var trips: [Trip]
    @Environment(\.modelContext) var modelContext

    var body: some View {
        NavigationStack() {
            List {
                ForEach(trips) { trip in
                    // ...
                }
            }
        }
    }
}
```

### Observing changes
- No need for `@Published`
- SwiftUI automatically refresh changes on any of the observed properties


To learn more about using SwiftUI and SwiftData together, see [Build an app with SwiftData][Build an app with SwiftData]

## Wrap up
- Define your schema using `@Model`
- Configure your `ModelContainer`
- Leverage SwiftUI and SwiftData

For more see: 
- [Migrate to SwiftData][Migrate to SwiftData]

---

## Reference

- [Meet SwiftData - WWDC23][Meet SwiftData]
- [Model your schema with SwiftData][Model your schema with SwiftData]
- [Dive deeper into SwiftData][Dive deeper into SwiftData]
- [Build an app with SwiftData][Build an app with SwiftData]
- [Migrate to SwiftData][Migrate to SwiftData]

- [Discover Observation in SwiftUI][Discover Observation in SwiftUI]
- [Whats new in Swift][Whats new in Swift]
- [Whats new in SwiftUI][Whats new in SwiftUI]

[Meet SwiftData]: https://developer.apple.com/videos/play/wwdc2023/10187/
[Model your schema with SwiftData]: https://developer.apple.com/videos/play/wwdc2023/10195
[Dive deeper into SwiftData]: https://developer.apple.com/videos/play/wwdc2023/10196
[Build an app with SwiftData]: https://developer.apple.com/videos/play/wwdc2023/10154
[Migrate to SwiftData]: https://developer.apple.com/videos/play/wwdc2023/10189

[Discover Observation in SwiftUI]: https://developer.apple.com/videos/play/wwdc2023/10149
[Whats new in Swift]: https://developer.apple.com/videos/play/wwdc2023/10164
[Whats new in SwiftUI]: https://developer.apple.com/videos/play/wwdc2023/10148