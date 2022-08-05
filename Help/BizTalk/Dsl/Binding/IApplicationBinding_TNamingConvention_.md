#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## IApplicationBinding<TNamingConvention> Interface

```csharp
public interface IApplicationBinding<TNamingConvention> :
Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution
    where TNamingConvention : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding_TNamingConvention_.TNamingConvention'></a>

`TNamingConvention`

Derived  
&#8627; [ApplicationBindingBase&lt;TNamingConvention&gt;](ApplicationBindingBase_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>')

Implements [IApplicationBinding](IApplicationBinding.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding'), [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding&lt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>')[TNamingConvention](IApplicationBinding_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>.TNamingConvention')[&gt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>'), [ISupportNameResolution](ISupportNameResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution')

| Properties | |
| :--- | :--- |
| [ReceivePorts](IApplicationBinding_TNamingConvention_.ReceivePorts.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>.ReceivePorts') | |
| [SendPorts](IApplicationBinding_TNamingConvention_.SendPorts.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>.SendPorts') | |
