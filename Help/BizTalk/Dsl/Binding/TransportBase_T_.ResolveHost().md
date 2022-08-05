#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding').[TransportBase&lt;T&gt;](TransportBase_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>')

## TransportBase<T>.ResolveHost() Method

Resolve host name that is to be bound to this transport's adapter.

```csharp
public abstract string ResolveHost();
```

Implements [ResolveHost()](ISupportHostResolution.ResolveHost().md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution.ResolveHost()')

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The name of the host.

### Remarks
Notice that TransportBase.ResolveHost delegates to either ReceiveLocationTransport's or SendPortTransport's
protected ResolveHost(), which delegate in turn to actual HostResolutionPolicy instance but this time with the
ReceiveLocationTransport or SendPortTransport instance being concerned passed as argument to help with resolution.