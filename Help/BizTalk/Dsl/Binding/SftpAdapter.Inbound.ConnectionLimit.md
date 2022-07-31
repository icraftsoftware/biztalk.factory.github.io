#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter').[Inbound](SftpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound')

## SftpAdapter.Inbound.ConnectionLimit Property

Specify the maximum number of concurrent connections that can be opened to the server.

```csharp
public int ConnectionLimit { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks
This setting is per server and per receive location. Consider the following scenarios:
- There are two receive locations that have the same configuration property values, including the ConnectionLimit
  property set to the same value. For example, the property is set to 6. In this situation, there is one connection
  pool (with 6 available connections) that is used by both receive locations.
- There are two receive locations configured with same configuration values, and have the ConnectionLimit property
  set to different values. For example, ReceiveLocation1 property is set to 6 and ReceiveLocation2 property is set
  to 5. In this situation, each receive location has its own connection pool with its own available connections.
  ReceiveLocation1 connection pool has 6 available connections. ReceiveLocation2 connection pool has 5 available
  connections.