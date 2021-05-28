
[Classes](#classes)
[Enums](#enums)
[Structures](#structures)

# Classes

open class UIHostingController<Content> : UIViewController where Content : View

---

# Enums

```
@frozen enum AccessibilityLabeledPairRole
@frozen enum Axis : Int8, CaseIterable, CustomStringConvertible, Equatable, Hashable,: RawRepresentable
```

```
@frozen enum ContentMode : Hashable, CaseIterable
```

```
@frozen enum Edge : Int8, CaseIterable, Equatable, Hashable, RawRepresentable
```

```
@frozen enum ExclusiveGesture.Value: Equatable where First.Value : Equatable, Second.Value : Equatable
```

```
@frozen enum Image.Orientation : UInt8, CaseIterable, Hashable, RawRepresentable
```

```
@frozen enum Path.Element : Equatable
```

```
@frozen enum SequenceGesture.Value
```

```
@frozen enum TextAlignment : Hashable, CaseIterable
```


```
enum AccessibilityAdjustmentDirection: Equatable, Hashable
```

```
enum BlendMode: Equatable, Hashable
```

```
enum Color.RGBColorSpace : Equatable, Hashable
enum ColorRenderingMode : Equatable, Hashable
enum ColorSchemeContrast : CaseIterable, Equatable, Hashable
enum ColorScheme : CaseIterable, Equatable, Hashable
enum ContentSizeCategory : Hashable, CaseIterable
enum CoordinateSpace : Equatable, Hashable
```

```
enum DropOperation : Equatable, Hashable
```

```
enum EditMode: Equatable, Hashable
```

```
enum Font.TextStyle : CaseIterable, Equatable, Hashable
enum Font.Leading: Equatable, Hashable
enum Font.Design : Hashable
```

```
enum GridItem.Size
```

```
enum Image.TemplateRenderingMode: Equatable, Hashable
enum Image.Scale: Equatable, Hashable
enum Image.Interpolation: Equatable, Hashable
enum Image.ResizingMode: Equatable, Hashable
```

```
enum LayoutDirection : Hashable, CaseIterable
enum LegibilityWeight : Hashable
```

```
enum NavigationBarItem.TitleDisplayMode : Equatable, Hashable
enum NSUserActivity.TypedPayloadError : Error
```

```
enum PopoverAttachmentAnchor
enum PreviewLayout
enum PreviewPlatform: Equatable, Hashable
```

```
enum RoundedCornerStyle: Equatable, Hashable
```

```
enum ScenePhase : Comparable, Hashable
```

```
enum Text.TruncationMode: Equatable, Hashable
enum Text.Case: Equatable, Hashable
```

```
enum UserInterfaceSizeClass: Equatable, Hashable
```

- - - - - - - - 
# Protocols

```
protocol AlignmentID
```

```
protocol Animatable
extension Animatable where Self : VectorArithmetic
extension Animatable where Self.AnimatableData == EmptyAnimatableData

protocol AnimatableModifier : Animatable, ViewModifier
protocol App
```

```
protocol ButtonStyle
```

```
protocol Commands
protocol CustomizableToolbarContent : ToolbarContent where Self.Body : CustomizableToolbarContent
```

```
protocol DatePickerStyle
protocol DropDelegate
protocol DynamicProperty
protocol DynamicViewContent : View
```

```
protocol EnvironmentKey
protocol EnvironmentalModifier : ViewModifier where Self.Body == Never
```

```
protocol FileDocument
protocol FocusedValueKey
```

```
protocol GeometryEffect : Animatable, ViewModifier where Self.Body == Never
protocol Gesture
protocol GroupBoxStyle
```

```
protocol IndexViewStyle
protocol InsettableShape : Shape
```

```
protocol LabelStyle
protocol ListStyle
```

```
protocol MenuStyle
```

```
protocol NavigationViewStyle
```

```
protocol PickerStyle
protocol PreferenceKey
extension PreferenceKey where Self.Value : ExpressibleByNilLiteral

protocol PreviewContext
protocol PreviewContextKey

protocol PreviewProvider : _PreviewProvider
protocol PrimitiveButtonStyle
protocol ProgressViewStyle
```

```
protocol ReferenceFileDocument : ObservableObject
```

```
protocol Scene
protocol Shape : Animatable, View

protocol ShapeStyle
extension ShapeStyle where Self : View, Self.Body == _ShapeView<Rectangle, Self>
```

```
protocol TabViewStyle
protocol TextFieldStyle
protocol ToggleStyle
protocol ToolbarContent
```

```
protocol UIViewControllerRepresentable : View where Self.Body == Never
extension UIViewControllerRepresentable where Self.Coordinator == Void
extension UIViewRepresentable where Self.Coordinator == Void

protocol UIViewRepresentable : View where Self.Body == Never
```

```
protocol VectorArithmetic : AdditiveArithmetic
protocol View

protocol ViewModifier
extension ViewModifier where Self.Body == Never
```

```
protocol Widget
protocol WidgetBundle
protocol WidgetConfiguration
```

- - - - - - - - 
# Function Builder

```
@_functionBuilder struct CommandsBuilder
@_functionBuilder struct SceneBuilder
@_functionBuilder struct ToolbarContentBuilder
@_functionBuilder struct ViewBuilder
@_functionBuilder struct WidgetBundleBuilder
```

- - - - - - - - 
# Structures

## Frozen Structures

```
@frozen struct Alignment : Equatable
@frozen struct Anchor<Value>
@frozen struct Anchor.Source
@frozen struct Angle : Hashable, Comparable, Animatable
@frozen struct AngularGradient : ShapeStyle, View
@frozen struct AnimatablePair<First, Second> : VectorArithmetic where First : VectorArithmetic, Second : VectorArithmetic
@frozen struct Animation : Equatable, CustomStringConvertible, CustomDebugStringConvertible, CustomReflectable
@frozen struct AnyGesture<Value> : Gesture
@frozen struct AnyTransition
@frozen struct AnyView : View

@frozen @propertyWrapper struct AppStorage<Value> : DynamicProperty
extension AppStorage where Value : ExpressibleByNilLiteral

@frozen struct Axis.Set : OptionSet
```

```
@frozen struct BackgroundStyle : ShapeStyle
@frozen @propertyWrapper @dynamicMemberLookup struct Binding<Value> : DynamicProperty
```

```
@frozen struct Capsule : Shape, InsettableShape
@frozen struct Circle : Shape, InsettableShape
@frozen struct Color : Hashable, CustomStringConvertible, View, ShapeStyle
@frozen struct ContainerRelativeShape : Shape, InsettableShape
```

```
@frozen struct Edge.Set : OptionSet

@frozen struct EdgeInsets : Equatable
extension EdgeInsets : Animatable

@frozen struct Ellipse : Shape, InsettableShape
@frozen struct EmptyAnimatableData : VectorArithmetic
@frozen struct EmptyModifier : ViewModifier
@frozen struct EmptyView : View
@frozen struct EmptyWidgetConfiguration : WidgetConfiguration
@frozen @propertyWrapper struct Environment<Value> : DynamicProperty
@frozen @propertyWrapper struct EnvironmentObject<ObjectType> : DynamicProperty where ObjectType : ObservableObject
@frozen @dynamicMemberLookup struct EnvironmentObject.Wrapper

@frozen struct EquatableView<Content> : View where Content : Equatable, Content : View
@frozen struct EventModifiers : OptionSet
@frozen struct ExclusiveGesture<First, Second> : Gesture where First : Gesture, Second : Gesture
```

```
@frozen struct FillStyle : Equatable
@frozen struct Font : Hashable
@frozen struct Font.Weight : Hashable
@frozen struct ForegroundStyle : ShapeStyle
```

```
@frozen struct GeometryReader<Content> : View where Content : View
@frozen struct GestureMask : OptionSet

@propertyWrapper @frozen struct GestureState<Value> : DynamicProperty
extension GestureState where Value : ExpressibleByNilLiteral

@frozen struct GestureStateGesture<Base, State> : Gesture where Base : Gesture
@frozen struct Gradient : Equatable
@frozen struct Gradient.Stop : Equatable

@frozen struct Group<Content>
extension Group : ToolbarContent where Content : ToolbarContent
extension Group : CustomizableToolbarContent where Content : CustomizableToolbarContent
extension Group where Content : _Widget
extension Group : Scene where Content : Scene
extension Group : View where Content : View
extension Group : Commands where Content : Commands
```

```
@frozen struct HStack<Content> : View where Content : View
@frozen struct HorizontalAlignment : Equatable
```

```
@frozen struct Image : Equatable: View
@frozen struct ImagePaint : ShapeStyle
```

```
@frozen struct LinearGradient : ShapeStyle, View
@frozen struct LocalizedStringKey : Equatable, ExpressibleByStringInterpolation
```

```
@frozen struct MatchedGeometryProperties : OptionSet
```

```
@frozen struct ModifiedContent<Content, Modifier>
extension ModifiedContent where Content : _Widget, Modifier : _WidgetModifier
extension ModifiedContent where Modifier == AccessibilityAttachmentModifier
extension ModifiedContent where Modifier == AccessibilityAttachmentModifier
extension ModifiedContent : Equatable where Content : Equatable, Modifier : Equatable
extension ModifiedContent : View where Content : View, Modifier : ViewModifier
extension ModifiedContent : ViewModifier where Content : ViewModifier, Modifier : ViewModifier
extension ModifiedContent : DynamicViewContent where Content : DynamicViewContent, Modifier : ViewModifier
extension ModifiedContent : Scene where Content : Scene, Modifier : _SceneModifier
extension ModifiedContent where Modifier == AccessibilityAttachmentModifier
extension ModifiedContent where Modifier == AccessibilityAttachmentModifier
extension ModifiedContent where Modifier == AccessibilityAttachmentModifier
extension ModifiedContent where Modifier == AccessibilityAttachmentModifier
extension ModifiedContent where Modifier == AccessibilityAttachmentModifier
```

```
@frozen @propertyWrapper struct Namespace : DynamicProperty
@frozen struct Namespace.ID : Hashable
```

```
@propertyWrapper @frozen struct ObservedObject<ObjectType> : DynamicProperty where ObjectType : ObservableObject
@dynamicMemberLookup @frozen struct ObservedObject.Wrapper

@frozen struct OffsetShape<Content> : Shape where Content : Shape
extension OffsetShape : InsettableShape where Content : InsettableShape
```

```
@frozen struct Path : Equatable, LosslessStringConvertible, Shape
@frozen struct ProjectionTransform : Equatable
```

```
@frozen struct RadialGradient : ShapeStyle, View
@frozen struct Rectangle : Shape, InsettableShape

@frozen struct RotatedShape<Content> : Shape where Content : Shape
extension RotatedShape : InsettableShape where Content : InsettableShape

@frozen struct RoundedRectangle : Shape, InsettableShape
```

```
@frozen struct SafeAreaRegions : OptionSet
@frozen struct ScaledShape<Content> : Shape where Content : Shape

@frozen @propertyWrapper struct SceneStorage<Value> : DynamicProperty
extension SceneStorage where Value : ExpressibleByNilLiteral

@frozen struct ScrollViewReader<Content> : View where Content : View
@frozen struct SimultaneousGesture<First, Second> : Gesture where First : Gesture, Second : Gesture

@frozen struct SimultaneousGesture.Value
extension SimultaneousGesture.Value : Equatable where First.Value : Equatable, Second.Value : Equatable
extension SimultaneousGesture.Value : Hashable where First.Value : Hashable, Second.Value : Hashable

@frozen struct SequenceGesture<First, Second> : Gesture where First : Gesture, Second : Gesture
extension SequenceGesture.Value : Equatable where First.Value : Equatable, Second.Value : Equatable

@frozen struct Spacer : View
@frozen struct StrokeStyle : Equatable, Animatable
@frozen struct SubscriptionView<PublisherType, Content> : View where PublisherType : Publisher, Content : View, PublisherType.Failure == Never

@frozen @propertyWrapper struct State<Value> : DynamicProperty
extension State where Value : ExpressibleByNilLiteral

@frozen @propertyWrapper struct StateObject<ObjectType> : DynamicProperty where ObjectType : ObservableObject
```

```
@frozen struct Text : Equatable, View
@frozen struct Transaction
@frozen struct TransformedShape<Content> : Shape where Content : Shape
@frozen struct TupleView<T> : View
```

```
@frozen struct UnitPoint : Hashable
extension UnitPoint : Animatable
```

```
@frozen struct VStack<Content> : View where Content : View
@frozen struct VerticalAlignment : Equatable
```

```
@frozen struct ZStack<Content> : View where Content : View
```

---

```
struct AccessibilityActionKind : Equatable
struct AccessibilityAttachmentModifier : ViewModifier
struct AccessibilityChildBehavior : Hashable
struct AccessibilityTraits : SetAlgebra
struct ActionSheet
struct Alert
```

```
struct BorderlessButtonMenuStyle : MenuStyle
struct BorderlessButtonStyle : PrimitiveButtonStyle

struct Button<Label> : View where Label : View
extension Button where Label == Text
extension Button where Label == PrimitiveButtonStyleConfiguration.Label

struct ButtonStyleConfiguration
```

```
struct CircularProgressViewStyle : ProgressViewStyle

struct ColorPicker<Label> : View where Label : View
extension ColorPicker where Label == Text

struct CommandGroup<Content> : Commands where Content : View
struct CommandGroupPlacement
struct CommandMenu<Content> : Commands where Content : View
struct CompactDatePickerStyle : DatePickerStyle
struct ContextMenu<MenuItems> where MenuItems : View
```

```
struct DatePicker<Label> : View where Label : View
struct DatePickerComponents : OptionSet
struct DefaultButtonStyle : PrimitiveButtonStyle
struct DefaultDatePickerStyle : DatePickerStyle
struct DefaultGroupBoxStyle : GroupBoxStyle
struct DefaultLabelStyle : LabelStyle
struct DefaultListStyle : ListStyle
struct DefaultMenuStyle : MenuStyle
struct DefaultNavigationViewStyle : NavigationViewStyle
struct DefaultPickerStyle : PickerStyle
struct DefaultProgressViewStyle : ProgressViewStyle
struct DefaultTabViewStyle : TabViewStyle
struct DefaultTextFieldStyle : TextFieldStyle
struct DefaultToggleStyle : ToggleStyle

struct DisclosureGroup<Label, Content> : View where Label : View, Content : View
extension DisclosureGroup where Label == Text

struct Divider : View

struct DocumentGroup<Document, Content> : Scene where Content : View
extension DocumentGroup where Document : FileDocument
extension DocumentGroup where Document : ReferenceFileDocument

struct DoubleColumnNavigationViewStyle : NavigationViewStyle
struct DragGesture : Gesture
struct DragGesture.Value : Equatable
struct DropInfo
struct DropProposal
```

```
struct EditButton : View
struct EmptyCommands : Commands
struct EnvironmentValues : CustomStringConvertible
```

```
@propertyWrapper struct FetchRequest<Result> : DynamicProperty where Result : NSFetchRequestResult
extension FetchRequest where Result : NSManagedObject

struct FetchedResults<Result> : RandomAccessCollection where Result : NSFetchRequestResult
struct FileDocumentConfiguration<Document> where Document : FileDocument
struct FileDocumentReadConfiguration
struct FileDocumentWriteConfiguration
@propertyWrapper struct FocusedBinding<Value> : DynamicProperty
@propertyWrapper struct FocusedValue<Value> : DynamicProperty
struct FocusedValues

struct ForEach<Data, ID, Content> where Data : RandomAccessCollection, ID : Hashable
extension ForEach : DynamicViewContent where Content : View
extension ForEach : View where Content : View
extension ForEach where ID == Data.Element.ID, Content : View, Data.Element : Identifiable
extension ForEach where Content : View
extension ForEach where Data == Range<Int>, ID == Int, Content : View

struct Form<Content> : View where Content : View
```

```
struct GeometryProxy
struct GraphicalDatePickerStyle : DatePickerStyle
struct GridItem

struct GroupBox<Label, Content> : View where Label : View, Content : View
extension GroupBox where Label == GroupBoxStyleConfiguration.Label, Content == GroupBoxStyleConfiguration.Content
extension GroupBox where Label == EmptyView

struct GroupBoxStyleConfiguration 
struct GroupBoxStyleConfiguration.Label : View
struct GroupBoxStyleConfiguration.Content : View
struct GroupedListStyle : ListStyle
```

```
struct HoverEffect
```

```
struct IconOnlyLabelStyle : LabelStyle
struct InlinePickerStyle : PickerStyle
struct InsetGroupedListStyle : ListStyle
struct InsetListStyle : ListStyle
```

```
struct KeyEquivalent : ExpressibleByExtendedGraphemeClusterLiteral
struct KeyboardShortcut
```

```
struct Label<Title, Icon> : View where Title : View, Icon : View
extension Label where Title == Text, Icon == Image
extension Label where Title == LabelStyleConfiguration.Title, Icon == LabelStyleConfiguration.Icon

struct LabelStyleConfiguration
struct LabelStyleConfiguration.Title : View
struct LabelStyleConfiguration.Icon : View
struct LazyHGrid<Content> : View where Content : View
struct LazyHStack<Content> : View where Content : View
struct LazyVGrid<Content> : View where Content : View
struct LazyVStack<Content> : View where Content : View
struct LinearProgressViewStyle : ProgressViewStyle

struct Link<Label> : View where Label : View
extension Link where Label == Text

struct List<SelectionValue, Content> : View where SelectionValue : Hashable, Content : View
extension List where SelectionValue == Never

struct ListItemTint
struct LocalizedStringKey.StringInterpolation : StringInterpolationProtocol
struct LongPressGesture : Gesture
```

```
struct MagnificationGesture : Gesture

struct Menu<Label, Content> : View where Label : View, Content : View
extension Menu where Label == MenuStyleConfiguration.Label, Content == MenuStyleConfiguration.Content

struct MenuPickerStyle : PickerStyle
struct MenuStyleConfiguration
struct MenuStyleConfiguration.Label : View
struct MenuStyleConfiguration.Content : View
struct NavigationBarItem 

struct NavigationLink<Label, Destination> : View where Label : View, Destination : View
extension NavigationLink where Label == Text

struct NavigationView<Content> : View where Content : View
```

```
struct OpenURLAction
struct OutlineGroup<Data, ID, Parent, Leaf, Subgroup> where Data : RandomAccessCollection, ID : Hashable
extension OutlineGroup where ID == Data.Element.ID, Parent : View, Parent == Leaf, Subgroup == DisclosureGroup<Parent, OutlineSubgroupChildren>, Data.Element : Identifiable
extension OutlineGroup where Parent : View, Parent == Leaf, Subgroup == DisclosureGroup<Parent, OutlineSubgroupChildren>
extension OutlineGroup : View where Parent : View, Leaf : View, Subgroup : View

struct OutlineSubgroupChildren : View
```

```
struct PageIndexViewStyle : IndexViewStyle
struct PageIndexViewStyle.BackgroundDisplayMode
struct PageTabViewStyle : TabViewStyle
struct PageTabViewStyle.IndexDisplayMode


struct Picker<Label, SelectionValue, Content> : View where Label : View, SelectionValue : Hashable, Content : View
extension Picker where Label == Text

struct PinnedScrollableViews : OptionSet
struct PlainButtonStyle : PrimitiveButtonStyle
struct PlainListStyle : ListStyle
struct PlainTextFieldStyle : TextFieldStyle
struct PreferredColorSchemeKey : PreferenceKey
struct PresentationMode
struct PreviewDevice : RawRepresentable, ExpressibleByStringLiteral
struct PrimitiveButtonStyleConfiguration
struct PrimitiveButtonStyleConfiguration.Label : View

struct ProgressView<Label, CurrentValueLabel> : View where Label : View, CurrentValueLabel : View
extension ProgressView where CurrentValueLabel == EmptyView

struct ProgressViewStyleConfiguration
struct ProgressViewStyleConfiguration.Label : View
struct ProgressViewStyleConfiguration.CurrentValueLabel : View 
```

```
struct RedactionReasons : OptionSet
struct ReferenceFileDocumentConfiguration<Document> where Document : ReferenceFileDocument
struct RotationGesture : Gesture
struct RoundedBorderTextFieldStyle : TextFieldStyle
```

```
@propertyWrapper struct ScaledMetric<Value> : DynamicProperty where Value : BinaryFloatingPoint

struct ScrollView<Content> : View where Content : View
struct ScrollViewProxy

struct Section<Parent, Content, Footer>
extension Section : View where Parent : View, Content : View, Footer : View
extension Section where Parent == EmptyView, Content : View, Footer : View
extension Section where Parent : View, Content : View, Footer == EmptyView
extension Section where Parent == EmptyView, Content : View, Footer == EmptyView

struct SecureField<Label> : View where Label : View
extension SecureField where Label == Text

struct SegmentedPickerStyle : PickerStyle
struct SidebarCommands : Commands
struct SidebarListStyle : ListStyle

struct Slider<Label, ValueLabel> : View where Label : View, ValueLabel : View
extension Slider where ValueLabel == EmptyView
extension Slider where Label == EmptyView, ValueLabel == EmptyView

struct StackNavigationViewStyle : NavigationViewStyle

struct Stepper<Label> : View where Label : View
extension Stepper where Label == Text

struct SwitchToggleStyle : ToggleStyle
```

```
struct TabView<SelectionValue, Content> : View where SelectionValue : Hashable, Content : View
extension TabView where SelectionValue == Int

struct TapGesture : Gesture
struct Text.DateStyle: Equatable, Codable
struct TextEditingCommands : Commands
struct TextEditor : View

struct TextField<Label> : View where Label : View
extension TextField where Label == Text

struct TextFormattingCommands : Commands
struct TitleOnlyLabelStyle : LabelStyle

struct Toggle<Label> : View where Label : View
extension Toggle where Label == ToggleStyleConfiguration.Label
extension Toggle where Label == Text

struct ToggleStyleConfiguration
struct ToolbarCommands : Commands

struct ToolbarItem<ID, Content> : ToolbarContent where Content : View
extension ToolbarItem where ID == Void
extension ToolbarItem : CustomizableToolbarContent where ID == String
extension ToolbarItem : Identifiable where ID : Hashable

struct ToolbarItemGroup<Content> : ToolbarContent where Content : View
struct ToolbarItemPlacement
```

```
@propertyWrapper struct UIApplicationDelegateAdaptor<DelegateType> : DynamicProperty where DelegateType : NSObject, DelegateType : UIApplicationDelegate
extension UIApplicationDelegateAdaptor where DelegateType : ObservableObject

struct UIViewControllerRepresentableContext<Representable> where Representable : UIViewControllerRepresentable
struct UIViewRepresentableContext<Representable> where Representable : UIViewRepresentable
```

```
struct ViewDimensions : Equatable
```

```
struct WheelDatePickerStyle : DatePickerStyle
struct WheelPickerStyle : PickerStyle
struct WindowGroup<Content> : Scene where Content : View
```

```
extension Never : Gesture, Scene, WidgetConfiguration, ToolbarContent, CustomizableToolbarContent, View
extension Optional : Gesture where Wrapped : Gesture
extension Optional : View where Wrapped : View
extension RangeReplaceableCollection where Self : MutableCollection
extension CGPoint : Animatable
extension CGSize : Animatable
extension CGRect : Animatable
extension Float : VectorArithmetic
extension Double : VectorArithmetic
extension CGFloat : VectorArithmetic
extension Never : Commands
```

---
