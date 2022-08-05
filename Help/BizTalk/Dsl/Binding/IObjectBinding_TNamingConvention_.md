#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## IObjectBinding<TNamingConvention> Interface

```csharp
public interface IObjectBinding<TNamingConvention> :
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution,
Be.Stateless.BizTalk.IFluentInterface
    where TNamingConvention : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding_TNamingConvention_.TNamingConvention'></a>

`TNamingConvention`

Derived  
&#8627; [ApplicationBindingBase&lt;TNamingConvention&gt;](ApplicationBindingBase_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>')  
&#8627; [IApplicationBinding&lt;TNamingConvention&gt;](IApplicationBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>')  
&#8627; [IReceiveLocation&lt;TNamingConvention&gt;](IReceiveLocation_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation<TNamingConvention>')  
&#8627; [IReceivePort&lt;TNamingConvention&gt;](IReceivePort_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>')  
&#8627; [ISendPort&lt;TNamingConvention&gt;](ISendPort_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>')  
&#8627; [ReceiveLocationBase&lt;TNamingConvention&gt;](ReceiveLocationBase_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>')  
&#8627; [ReceivePortBase&lt;TNamingConvention&gt;](ReceivePortBase_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>')  
&#8627; [SendPortBase&lt;TNamingConvention&gt;](SendPortBase_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>')

Implements [ISupportNameResolution](ISupportNameResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution'), [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface')

| Properties | |
| :--- | :--- |
| [Description](IObjectBinding_TNamingConvention_.Description.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>.Description') | |
| [Name](IObjectBinding_TNamingConvention_.Name.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>.Name') | |
