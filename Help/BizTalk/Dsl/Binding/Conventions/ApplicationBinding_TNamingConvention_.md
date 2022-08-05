#### [Be.Stateless.BizTalk.Dsl.Binding.Conventions](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Convention](Be.Stateless.BizTalk.Dsl.Binding.Convention.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention')

## ApplicationBinding<TNamingConvention> Class

```csharp
public class ApplicationBinding<TNamingConvention> : Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>
    where TNamingConvention : class, Be.Stateless.BizTalk.Dsl.Binding.Convention.INamingConvention<TNamingConvention>, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding_TNamingConvention_.TNamingConvention'></a>

`TNamingConvention`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase-1 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase`1')[TNamingConvention](ApplicationBinding_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding<TNamingConvention>.TNamingConvention')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase-1 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase`1') &#129106; ApplicationBinding<TNamingConvention>

| Constructors | |
| :--- | :--- |
| [ApplicationBinding()](ApplicationBinding_TNamingConvention_.ApplicationBinding().md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding<TNamingConvention>.ApplicationBinding()') | |
| [ApplicationBinding(Action&lt;IApplicationBinding&lt;TNamingConvention&gt;&gt;)](ApplicationBinding_TNamingConvention_.ApplicationBinding(Action_IApplicationBinding_TNamingConvention__).md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding<TNamingConvention>.ApplicationBinding(System.Action<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>>)') | |

| Properties | |
| :--- | :--- |
| [ApplicationName](ApplicationBinding_TNamingConvention_.ApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding<TNamingConvention>.ApplicationName') | |
| [ReceiveLocationName](ApplicationBinding_TNamingConvention_.ReceiveLocationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding<TNamingConvention>.ReceiveLocationName') | |
| [ReceivePortName](ApplicationBinding_TNamingConvention_.ReceivePortName.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding<TNamingConvention>.ReceivePortName') | |
| [SendPortName](ApplicationBinding_TNamingConvention_.SendPortName.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding<TNamingConvention>.SendPortName') | |

| Methods | |
| :--- | :--- |
| [ReceiveLocation(Action&lt;IReceiveLocation&lt;TNamingConvention&gt;&gt;)](ApplicationBinding_TNamingConvention_.ReceiveLocation(Action_IReceiveLocation_TNamingConvention__).md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding<TNamingConvention>.ReceiveLocation(System.Action<Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation<TNamingConvention>>)') | |
| [ReceivePort(Action&lt;IReceivePort&lt;TNamingConvention&gt;&gt;)](ApplicationBinding_TNamingConvention_.ReceivePort(Action_IReceivePort_TNamingConvention__).md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding<TNamingConvention>.ReceivePort(System.Action<Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>>)') | |
| [SendPort(Action&lt;ISendPort&lt;TNamingConvention&gt;&gt;)](ApplicationBinding_TNamingConvention_.SendPort(Action_ISendPort_TNamingConvention__).md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ApplicationBinding<TNamingConvention>.SendPort(System.Action<Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>>)') | |
