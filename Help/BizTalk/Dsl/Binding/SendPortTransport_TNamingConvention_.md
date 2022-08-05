#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## SendPortTransport<TNamingConvention> Class

```csharp
public sealed class SendPortTransport<TNamingConvention> : Be.Stateless.BizTalk.Dsl.Binding.TransportBase<Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter>
    where TNamingConvention : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.SendPortTransport_TNamingConvention_.TNamingConvention'></a>

`TNamingConvention`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.TransportBase&lt;](TransportBase_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>')[IOutboundAdapter](IOutboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter')[&gt;](TransportBase_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>') &#129106; SendPortTransport<TNamingConvention>

| Constructors | |
| :--- | :--- |
| [SendPortTransport(ISendPort&lt;TNamingConvention&gt;)](SendPortTransport_TNamingConvention_.SendPortTransport(ISendPort_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortTransport<TNamingConvention>.SendPortTransport(Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>)') | |

| Properties | |
| :--- | :--- |
| [RetryPolicy](SendPortTransport_TNamingConvention_.RetryPolicy.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortTransport<TNamingConvention>.RetryPolicy') | |
| [SendPort](SendPortTransport_TNamingConvention_.SendPort.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortTransport<TNamingConvention>.SendPort') | |
| [ServiceWindow](SendPortTransport_TNamingConvention_.ServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortTransport<TNamingConvention>.ServiceWindow') | [ServiceWindow](SendPortTransport_TNamingConvention_.ServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortTransport<TNamingConvention>.ServiceWindow') restricts the [SendPortBase&lt;TNamingConvention&gt;](SendPortBase_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>') to work during certain hours             of the day. |

| Methods | |
| :--- | :--- |
| [ApplyEnvironmentOverrides(string)](SendPortTransport_TNamingConvention_.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortTransport<TNamingConvention>.ApplyEnvironmentOverrides(string)') | |
| [ResolveHost()](SendPortTransport_TNamingConvention_.ResolveHost().md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortTransport<TNamingConvention>.ResolveHost()') | |
