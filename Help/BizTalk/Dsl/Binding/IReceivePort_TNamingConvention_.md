#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## IReceivePort<TNamingConvention> Interface

```csharp
public interface IReceivePort<TNamingConvention> :
Be.Stateless.BizTalk.Dsl.Binding.IReceivePort,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution
    where TNamingConvention : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.IReceivePort_TNamingConvention_.TNamingConvention'></a>

`TNamingConvention`

Derived  
&#8627; [ReceivePortBase&lt;TNamingConvention&gt;](ReceivePortBase_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>')

Implements [IReceivePort](IReceivePort.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceivePort'), [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding&lt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>')[TNamingConvention](IReceivePort_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.IReceivePort_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>.TNamingConvention')[&gt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>'), [ISupportNameResolution](ISupportNameResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution')

| Properties | |
| :--- | :--- |
| [ApplicationBinding](IReceivePort_TNamingConvention_.ApplicationBinding.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>.ApplicationBinding') | |
| [ReceiveLocations](IReceivePort_TNamingConvention_.ReceiveLocations.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>.ReceiveLocations') | |
