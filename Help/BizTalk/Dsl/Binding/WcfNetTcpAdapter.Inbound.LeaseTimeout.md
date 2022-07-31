#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpAdapter](WcfNetTcpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter').[Inbound](WcfNetTcpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter.Inbound')

## WcfNetTcpAdapter.Inbound.LeaseTimeout Property

Specify the maximum lifetime of an active pooled connection. After the specified time elapses, the connection
closes after the current request is serviced.

```csharp
public System.TimeSpan LeaseTimeout { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

The WCF-NetTcp adapter leverages the [System.ServiceModel.NetTcpBinding](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.NetTcpBinding 'System.ServiceModel.NetTcpBinding') class to communicate with an endpoint. When using
the [System.ServiceModel.NetTcpBinding](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.NetTcpBinding 'System.ServiceModel.NetTcpBinding') in load-balanced scenarios, consider reducing the default lease timeout.

It defaults to 00:05:00.