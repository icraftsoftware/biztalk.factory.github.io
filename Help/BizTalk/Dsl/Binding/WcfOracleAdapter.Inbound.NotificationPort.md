#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter](WcfOracleAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter').[Inbound](WcfOracleAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound')

## WcfOracleAdapter.Inbound.NotificationPort Property

Specifies the port number that ODP.NET must open to listen for database change notification from Oracle database.

```csharp
public int NotificationPort { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks

If there is more than one application in an application domain receiving notifications using the Oracle Database
adapter, the [NotificationPort](WcfOracleAdapter.Inbound.NotificationPort.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.NotificationPort') binding property for all applications must be set to the same port
number. This is because ODP.NET creates only one listener that listens on one port within an application domain.

Adapter clients will not receive database change notifications if Windows Firewall is turned on. Also, turning off
Windows Firewall to receive notifications is not advisable. So, to receive notifications without compromising the
security of the client-side computers, we recommend specifying a positive integer value as a port number and then
adding that port number to the Windows Firewall exceptions list. If you set this binding property to the default
value of -1, ODP.NET uses a random port and adapter clients will not know which port to add to Windows Firewall
exceptions list.

It defaults to -1, which signifies that ODP.NET uses a valid, random, unused port number.