#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding').[TransportBase&lt;T&gt;](TransportBase_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>')

## TransportBase<T>.Host Property

The BizTalk Server Host Name that will host this transport's [Adapter](TransportBase_T_.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.Adapter') at runtime.

```csharp
public Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy Host { get; set; }
```

#### Property Value
[HostResolutionPolicy](HostResolutionPolicy.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy')

### Remarks
The [Host](TransportBase_T_.Host.md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.Host') property can either be set directly to a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') value or to a [HostResolutionPolicy](HostResolutionPolicy.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy')-derived object instance.