#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter&lt;TConfig&gt;](WcfSapAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<TConfig>')

## WcfSapAdapter<TConfig>.SncLibrary Property

Specifies the location of the SNC library on your computer. If the PATH environment variable contains the directory
in which the library resides, you only have to supply the filename of the library; otherwise you must supply the full
path.

```csharp
public string SncLibrary { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
The SncLibrary binding property surfaces an SAP connection property. For more information see the SAP documentation.
You must set the UseSnc parameter in the connection URI to enable Secure Network Communications (SNC). For more
information about the SAP connection URI, [Create
            the SAP system connection URI](https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/create-the-sap-system-connection-uri 'https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/create-the-sap-system-connection-uri').