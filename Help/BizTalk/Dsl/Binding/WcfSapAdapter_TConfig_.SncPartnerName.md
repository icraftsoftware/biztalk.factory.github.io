#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter&lt;TConfig&gt;](WcfSapAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<TConfig>')

## WcfSapAdapter<TConfig>.SncPartnerName Property

The SNC Partner Name. Required if SNC is used.

```csharp
public string SncPartnerName { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
The SncPartnerName binding property surfaces an SAP connection property. For more information, see the SAP
documentation. You must set the UseSnc parameter in the connection URI to enable Secure Network Communications (SNC).
For more information about the SAP connection URI, [Create
            the SAP system connection URI](https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/create-the-sap-system-connection-uri 'https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/create-the-sap-system-connection-uri').