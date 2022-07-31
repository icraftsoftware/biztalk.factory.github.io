#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter&lt;TConfig&gt;](WcfSapAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<TConfig>')

## WcfSapAdapter<TConfig>.MaxConnectionsPerSystem Property

Specifies the maximum number of connections in the SAP adapter connection pool that are allowed to connect to a SAP
system.

```csharp
public int MaxConnectionsPerSystem { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks

<seealso cref="P:Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter`1.MaxConnectionsPerSystem"/> is a static property within an application domain. This means that when you
            change <seealso cref="P:Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter`1.MaxConnectionsPerSystem"/> for one binding instance in an application domain, the new value
            applies to all objects created from all binding instances within that application domain.

By default, the SAP client library (librfc32u.dll) supports a maximum of 100 connections to the SAP system. If you
exceed this number of connections, an exception will be thrown by the SAP adapter. For this reason, you should not
set MaxConnectionsPerSystem to a value greater than the number of connections supported by the SAP client library.
You can increase the number of connections that the SAP client library supports by setting the environment variable,
CPIC_MAX_CONV. You must reboot your computer after setting this variable for the change to take effect.

It defaults to 50.