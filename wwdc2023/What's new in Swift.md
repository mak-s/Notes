# Whats new in Swift
## WWDC 2023
[What's new in Swift](https://developer.apple.com/videos/play/wwdc2023/10164/)

---
### Swift Project Updates:

swift.org/swift-evolution
- Language Streering Group
  - Vision Documents
- Ecosystem Streeting Group

See [Evolving the Swift Workgroup](https://www.swift.org/blog/evolving-swift-project-workgroups/)

---
### Expressive Code:

[Swift 5.9]

- use of if/else/swift as expressions
  - initializing a variable using ternary operator can be repaced with if/else
  - variable initialized using closure can directly use expressions dropping closure

- Result Builders
  - faster type checking
  - improved code completion
  - more accurate error messages

- Generics
  - multiple argument length
  ```swift
  <each Result>
  ```
  See [Generalized APIs using parameter packs](https://developer.apple.com/videos/play/wwdc2023/10168/) 
 
 - Macros `macro`
   ```swift
   import PowerAssert
   #assert(max(a,b) == c)

   // macro declaration
   public macro assert(_ condition: Bool)

   // macros are separate programs
   public macro assert(_ condition: Bool) = #externalMacro(
    module: "PowerAssertPlugin",
    type: "PowerAssertMacro"
   )
   ```
   
   Freestanding Macro
   ```swift
   // freestanding macro roles
   
   @freestanding(expression)
   public macro assert(_ condition: Bool) = #externalMacro(
    module: "PowerAssertPlugin",
    type: "PowerAssertMacro"
   )
   ```

   Predicate Expression Macro
   ```swift
   // predicate expression macro

   @freestanding(expression)
   public macro Predicate<each Input>(
    _ body: (repeat each Input) -> Bool
   ) -> Predicate<repeat each Input>

   let pred = #Predicate<Person> {
    $0.favoriteColor == .blue
   }
   let blueLovers = people.filter(pred)
   ```

   Example: Testing for a specific enum case

   ```swift
   // Testing for a specific enum case

   enum Path {
    case relative(String)
    case absolute(String)
   }

   let absPath = paths.filter { $0.isAbsolute }

   extension Path {
    var isAbsolute: Bool {
        if case .absolute == self { true }
        else { false }
    }

    var isRelative: Bool {
        if case .relative == self { true }
        else { false }
    }
   }

   ```

   ```swift
   // Testing for a specific enum case with macros

   @CaseDetection
   enum Path {
    case relative(String)
    case absolute(String)
   }

   let absPath = paths.filter { $0.isAbsolute }

   // CaseDetection macro will auto generate the code for comparison
   ```

   __Attached macro roles__
   | macro| description |
   |---|---|
   | @attached(member) | Adds new declarations inside the type.extension it's applied to|
   |@attached(peer)| Adds new declarations alongside the declaration it's applied to|
   |@attached(accessor)| Adds accessors to a property|
   |@attached(memberAttribute)| Adds attributes to the declarations in the type/extension it's applied to|
   |@attached(conformance)|Adds conformances to the type/extension it's applied to|

   Macros can be combined together to achieve useful effects.

   For example:
   
   Observation in SwiftUI
   ```swift
   // observation in SwiftUI
   final class Person: ObservableObject {
    @Published var name: String
    @Published var age: Int
    @Published var isFavorite: Bool
   }

   struct ContentView: View {
    @ObservedObject var person: Person

    var body: some View {
        Text("Hello, \(person.name)")
    }
   }
   ```
   With Macro based observation, updates to the following:
   ```swift
   @Observable final class Person {
    var name: String
    var age: Int
    var isFavorite: Bool
   }

   struct ContentView: View {
    var person: Person

    var body: some View {
        Text("Hello, \(person.name)")
    }
   }
   ```

   The `Observable` macro is composed as
   ```swift

   @attached(member, names:...)
   @attached(memberAttribute)
   @attached(conformance)
   public macro Observable() = #externalMacro(...)
   ```

   The `Observable` macro is expanded as

   ```swift
   // conformance role introduces conformance to the Observable protocol
   @Observable final class Person: Observable {
   ```
   ```swift
    // memberAttribute role adds ObservationTracked macro 
    // which in turn expands to add getters/setters to trigger observation events
    @ObservationTracked var name: String { get { ... } set { ... } }
    @ObservationTracked var age: Int { get { ... } set { ... } }
    @ObservationTracked var isFavorite: Bool { get { ... } set { ... } }
   ```
   ```swift
    // member role introduces new properties and methods
    internal let _$observationRegistrar = ObservationRegistrar<Person>()
    internal func access<Member>(
     keyPath: KeyPath<person, Member>
    ) {
     _$observationRegistrar.access(self, keyPath: keyPath)
    }

    internal func withMutation<Member, T> (
     keyPath: KeyPath<Person, Member>,
     _ mutation: () throws -> T
    ) rethrows -> T {
     try _$observationRegistrar.withMutation(of: self, keyPath: keyPath, mutation)
    }
   }
   ```

   __Swift macros__
   - Macros enable expression APIs and eliminate boilerplate
   - Macros integrate seamlessly into the development environment

   See: 
   - [Expand on Swift macros](https://developer.apple.com/videos/play/wwdc2023/10167/)
   - [Write Swift macros](https://developer.apple.com/videos/play/wwdc2023/10166)

---
### Swift Everywhere:

#### __Swift Foundation__
- Open source Foundation project, written in swift. See [The Future of Foundation](https://www.swift.org/blog/future-of-foundation/)
  - FoundationEssentials
  - FoundationInternationalization
  - FoundationObjCCompatibility

- Swift Foundation (swift efficiency, bridging cost reduction)
  - Calandar calculations: 20% faster
  - Date formatting: 150% faster
  - JSON coding: 200-500% faster

 ---
 #### __Ownership Concept__
 
 ```swift
 struct FileDescriptor {
    private var fd: CInt

    init(descriptor: CInt) { self.fd = descriptor }

    func write(buffer: [UInt8]) throws {
        let written = buffer.withUnsafeBufferPointer {
            Darwin.write(fd, $0.baseAddress, $0.count)
        }
        // ...
    }

    func close() {
        Darwin.close(fd)
    }
 }
 ```
 __Drawbacks:__
 - trying to write after calling `close()`
 - failing to `close()` before type goes out of scope, resulting in resource leak.
 - making a copy of this Type, could lead to unintentional sharing of mutable state across threads
 
 One solution would be to make it a `class` and closing `fd` on `deinit`
 ```swift
 class FileDescriptor {
    private var fd: CInt

    init(descriptor: CInt) { self.fd = descriptor }

    func write(buffer: [UInt8]) throws {
        let written = buffer.withUnsafeBufferPointer {
            Darwin.write(fd, $0.baseAddress, $0.count)
        }
        // ...
    }

    func close() {
        Darwin.close(fd)
    }

    deinit {
        Darwin.close(fd)    
    }
 }
 ```
 __Drawbacks:__
 - additional memory allocation
 - classes have are reference semantics, so they may lead to sharing reference across threads leading to race condition
 - unintentional storate


Swift Struct/Class can be copied by default.
To disable copy, `~Copyable` can be used on Struct and Enum declaration.
```swift
 struct FileDescriptor: ~Copyable {
    private var fd: CInt

    init(descriptor: CInt) { self.fd = descriptor }

    func write(buffer: [UInt8]) throws {
        let written = buffer.withUnsafeBufferPointer {
            Darwin.write(fd, $0.baseAddress, $0.count)
        }
        // ...
    }

    // non-copyable type can also be used to solve the problem of calling close
    // and then using other methods
    // by marking the method as `consuming`
    // calling a `consuming` method/argument gives out ownership of the value to the method you called (by default, methods in Swift borrow their arguments, including self)
    // since the type is non-copyable, giving up ownership mean you can no longer use the value
    consuming func close() {
        Darwin.close(fd)
    }

    // once a type is non-copyable, we can define a deinit like a class
    // that would run when value of a type goes out of scope
    deinit {
        Darwin.close(fd)
    }
 }
 ```

 ```swift
 let file = FileDescriptor(fd: descriptor)
 file.write(buffer: data)
 file.close()                   
 file.write(buffer: data)       // compile time error
 ```
 ---

 #### __C++ Interoperability__
 
 - Project Build Settings: Swift Compiler - Language > C++ and Objective-C Interoperability
 - C++ can use most Swift Types without any bridging overhead.
 ```swift
 // Geometry.swift
 struct LabledPoint {
    var x = 0.0, y = 0.0
    var label: String = "origin"
    mutating func moveBy(x deltaX: Double, y deltaY: Double) { ... }
    var magnitude: Double { ... }
 }
 ```
 ```c++
 // C++ client
 #include <Geometry-Swift.h>

 void test() {
    LabeledPoint origin = LabeledPoint()
    LabeledPoint unit = LabeledPoint::init(1.0, 1.0, "unit")
    unit.moveBy(2, -2)
    std::cout << unit.label << "moved to " << unit.magnitude() << std::endl;
 }
 ```

  - use c++ APIs directly from Swift (occasional annotation required)
  - expose most Swift APIs directly to C++ (no annotation required)

  See [Mix Swift and C++](https://developer.apple.com/videos/play/wwdc2023/10172)

___

#### __Swift Suport in CMake__
Integrate Swift code in CMake build.
```
project(PingPong LANGUAGES CXX Swift)

add_library(PingPong
  Ping.swift
  Pong.swift
  TableTennisUtils.cpp
)
```
___

#### __Actors and concurrency__

__Abstract Concurrency Model__

Tasks: 
- Sequential Unit of work that can run anywhere

Actors:
- Mutually exclusive access to isolated state

__Tasks in different environments__

Global concurrency pool determines scheduling:
- Dispatch on Apple platforms
- Single-threaded cooperative queue in restricted environments

Checked continuations provide interoperability with callback-based systems
```swift
withCheckedContinuation { continuation in
  sendMessage(message) { response in
    continuation.resume(returning: response)
  }
}
```
__Actors__

Actors can be implemented in different ways.
Custom actor executors enable customization.
```swift
actor MyConnection {
    private var database: UnsafeMutablePointer<sqlite3>
    init(fileName: String) throws { ... }

    func pruneOldEntries() { ... }
    func fetchEntry<Entry>(named: String, type: Entry.Type) -> Entry? { ... }
}

await connection.pruneOldEntries()
```

```swift
// with custom actor executors
actor MyConnection {
    private var database: UnsafeMutablePointer<sqlite3>

    private let queue: DispatchSerialQueue
    nonisolated var unownedExecutor: UnownedSerialExecutor {
        queue.asUnownedSerialExecutor()
    }

    init(fileName: String) throws { ... }

    func pruneOldEntries() { ... }
    func fetchEntry<Entry>(named: String, type: Entry.Type) -> Entry? { ... }
}

await connection.pruneOldEntries()
```

```swift
// Executor protocols
protocol Executor: AnyObject, Sendable {
    func enqueue(_ job: consuming ExecutorJob)
}

protocol SerialExecutor: Executor {
    func asUnownedSerialExecutor() -> UnownedSerialExecutor
    func isSameExclusiveExecutionContext(other executor: Self) -> Bool
}

extension DispatchSerialQueue: SerialExecutor { ... }

```

Swift Concurrency
- Tasks and actors for the abstract model for Swift concurrency
- Abstract model can be adapted to different execution environments
- Abstract model provides customization points for tasks and actors

For more, see:
- [Swift Concurrency: Behind the Scenes](https://developer.apple.com/videos/play/wwdc2021/10254)
- [Beyond the basics of structured concurrency](https://developer.apple.com/videos/play/wwdc2023/10170)

___

Use case: C++ - Swift Interoperability

[__FoundationDB__](https://www.foundationdb.org)
- large cross-platform C++ code base
- heavy use of asynchronous programming based on C++ features
- distributed actor runtime providing deterministic simulation

