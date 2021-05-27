
[Protocols](#protocol)

[Enums](#enums)

[Structure](#structures)

[Inheritance](#inheritance)

---

### Protocol

Protocols in Combine

```
Cancellable
ConnectablePublisher
CustomCombineIdentifierConvertible
ObservableObject
Publisher
Scheduler
SchedulerTimeIntervalConvertible
Subject
Subscriber
Subscription
TopLevelDecoder
TopLevelEncoder
```

---

### Enums

Enums in Combine

```
Publishers
TimeGroupingStrategy<Context>
PrefetchStrategy
BufferingStrategy<Failure>
Subscribers
Completion<Failure>                     // frozen
Subscriptions
```

---

### Structures

Structure in Combine

```
AnyPublisher<Output, Failure>           // frozen
AnySubscriber<Input, Failure>           // frozen
CombineIdentifier
Deferred<DeferredPublisher>
Empty<Output, Failure>
Fail<Output, Failure>
ImmediateScheduler
SchedulerTimeType
Stride
Just<Output>
Published<Value>                        // propertyWrapper
Publisher

SubscribeOn<Upstream, Context>
SubscribeOn<Upstream, Context>
DropWhile<Upstream>
TryDropWhile<Upstream>
Filter<Upstream>
TryFilter<Upstream>
Breakpoint<Upstream>
AllSatisfy<Upstream>
TryAllSatisfy<Upstream>
RemoveDuplicates<Upstream>
TryRemoveDuplicates<Upstream>
Decode<Upstream, Output, Coder>
Encode<Upstream, Coder>
Contains<Upstream>
CombineLatest<A, B>
CombineLatest3<A, B, C>
CombineLatest4<A, B, C, D>
Print<Upstream>
PrefixWhile<Upstream>
TryPrefixWhile<Upstream>
SetFailureType<Upstream, Failure>
ContainsWhere<Upstream>
TryContainsWhere<Upstream>
CollectByTime<Upstream, Context>
Collect<Upstream>
CollectByCount<Upstream>
ReceiveOn<Upstream, Context>
MapKeyPath<Upstream, Output>
MapKeyPath2<Upstream, Output0, Output1>
MapKeyPath3<Upstream, Output0, Output1, Output2>
PrefixUntilOutput<Upstream, Other>
Reduce<Upstream, Output>
TryReduce<Upstream, Output>
CompactMap<Upstream, Output>
TryCompactMap<Upstream, Output>
Merge<A, B>
Merge3<A, B, C>
Merge4<A, B, C, D>
Merge5<A, B, C, D, E>
Merge6<A, B, C, D, E, F>
Merge7<A, B, C, D, E, F, G>
Merge8<A, B, C, D, E, F, G, H>
MergeMany<Upstream>
Scan<Upstream, Output>
TryScan<Upstream, Output>
Count<Upstream>
LastWhere<Upstream>
TryLastWhere<Upstream>
IgnoreOutput<Upstream>
SwitchToLatest<P, Upstream>
Retry<Upstream> : Publisher
MapError<Upstream, Failure>
Throttle<Upstream, Context>
Comparison<Upstream>
TryComparison<Upstream>
ReplaceEmpty<Upstream>
ReplaceError<Upstream>
AssertNoFailure<Upstream>
DropUntilOutput<Upstream, Other>
HandleEvents<Upstream>
Concatenate<Prefix, Suffix>
Debounce<Upstream, Context>
Last<Upstream>
Map<Upstream, Output>
TryMap<Upstream, Output>
Timeout<Upstream, Context>
Buffer<Upstream>
Sequence<Elements, Failure>
Zip<A, B>
Zip3<A, B, C>
Zip4<A, B, C, D>
Output<Upstream>
Catch<Upstream, NewPublisher>
TryCatch<Upstream, NewPublisher>
FlatMap<NewPublisher, Upstream>
Delay<Upstream, Context>
Drop<Upstream>
First<Upstream>
FirstWhere<Upstream>
TryFirstWhere<Upstream>
Record<Output, Failure>
Record<Output, Failure>.Recording
Publisher
Deferred<DeferredPublisher>
Empty<Output, Failure>
Fail<Output, Failure>
Just<Output>
MakeConnectable<Upstream>
Subscribers.Demand                      // frozen
Optional.Publisher
Result.Publisher
AnyPublisher<Output, Failure>
AnySubscriber<Input, Failure>
CombineIdentifier
ImmediateScheduler
ImmediateScheduler.SchedulerTimeType
ImmediateScheduler.Stride
```

---

# Inheritance

Type inheritance in Combine

```
Cancellable
- AnyCancellable
```

```
AnyObject
- ObservableObject
```

```
CustomCombineIdentifierConvertible
- Subscriber
-- AnySubscriber<Input, Failure>
- Subscription
```

```
Hashable
- CombineIdentifier
```

```
Codable
- Subscribers.Demand
```

```
Published<Value>                              // propertyWrapper
CombineIdentifier
AnyPublisher<Output, Failure>                 // frozen
AnySubscriber<Input, Failure>                 // frozen
```

```
Scheduler
- ImmediateScheduler
```

```
Strideable
- ImmediateScheduler.SchedulerTimeType
```

```
SchedulerTimeIntervalConvertible
- ImmediateScheduler.Stride
```

```
Publisher
- Subject
--- CurrentValueSubject<Output, Failure>
--- PassthroughSubject<Output, Failure>
```

```
Publisher
- ObservableObjectPublisher
- Deferred<DeferredPublisher>
- Empty<Output, Failure>
- Fail<Output, Failure>
- Just<Output>
- Published<Value>.Publisher
- SubscribeOn<Upstream, Context>
- SubscribeOn<Upstream, Context>
- DropWhile<Upstream>
- TryDropWhile<Upstream>
- Filter<Upstream>
- TryFilter<Upstream>
- Breakpoint<Upstream>
- AllSatisfy<Upstream>
- TryAllSatisfy<Upstream>
- RemoveDuplicates<Upstream>
- TryRemoveDuplicates<Upstream>
- Decode<Upstream, Output, Coder>
- Encode<Upstream, Coder>
- Contains<Upstream>
- CombineLatest<A, B>
- CombineLatest3<A, B, C>
- CombineLatest4<A, B, C, D>
- Print<Upstream>
- PrefixWhile<Upstream>
- TryPrefixWhile<Upstream>
- SetFailureType<Upstream, Failure>
- ContainsWhere<Upstream>
- TryContainsWhere<Upstream>
- CollectByTime<Upstream, Context>
- Collect<Upstream>
- CollectByCount<Upstream>
- ReceiveOn<Upstream, Context>
- MapKeyPath<Upstream, Output>
- MapKeyPath2<Upstream, Output0, Output1>
- MapKeyPath3<Upstream, Output0, Output1, Output2>
- PrefixUntilOutput<Upstream, Other>
- Reduce<Upstream, Output>
- TryReduce<Upstream, Output>
- CompactMap<Upstream, Output>
- TryCompactMap<Upstream, Output>
- Merge<A, B>
- Merge3<A, B, C>
- Merge4<A, B, C, D>
- Merge5<A, B, C, D, E>
- Merge6<A, B, C, D, E, F>
- Merge7<A, B, C, D, E, F, G>
- Merge8<A, B, C, D, E, F, G, H>
- MergeMany<Upstream>
- Scan<Upstream, Output>
- TryScan<Upstream, Output>
- Count<Upstream>
- LastWhere<Upstream>
- TryLastWhere<Upstream>
- IgnoreOutput<Upstream>
- SwitchToLatest<P, Upstream>
- Retry<Upstream> : Publisher
- MapError<Upstream, Failure>
- Throttle<Upstream, Context>
- Comparison<Upstream>
- TryComparison<Upstream>
- ReplaceEmpty<Upstream>
- ReplaceError<Upstream>
- AssertNoFailure<Upstream>
- DropUntilOutput<Upstream, Other>
- HandleEvents<Upstream>
- Concatenate<Prefix, Suffix>
- Debounce<Upstream, Context>
- Last<Upstream>
- Map<Upstream, Output>
- TryMap<Upstream, Output>
- Timeout<Upstream, Context>
- Buffer<Upstream>
- Sequence<Elements, Failure>
- Zip<A, B>
- Zip3<A, B, C>
- Zip4<A, B, C, D>
- Output<Upstream>
- Catch<Upstream, NewPublisher>
- TryCatch<Upstream, NewPublisher>
- FlatMap<NewPublisher, Upstream>
- Delay<Upstream, Context>
- Drop<Upstream>
- First<Upstream>
- FirstWhere<Upstream>
- TryFirstWhere<Upstream>
- Record<Output, Failure>
- Record<Output, Failure>.Recording
- Publisher
- Deferred<DeferredPublisher>
- Empty<Output, Failure>
- Fail<Output, Failure>
- Just<Output>
- Optional.Publisher
- Result.Publisher
```

```
Publisher
- ConnectablePublisher
-- MakeConnectable<Upstream>
```

