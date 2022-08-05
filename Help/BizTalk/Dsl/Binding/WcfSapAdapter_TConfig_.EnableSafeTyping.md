#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter&lt;TConfig&gt;](WcfSapAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<TConfig>')

## WcfSapAdapter<TConfig>.EnableSafeTyping Property

Determines whether DATS, TIMS and NUMC are exposed as <seealso cref="T:System.String"/>.

```csharp
public bool EnableSafeTyping { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

This feature controls how the adapter surfaces certain SAP data types. For more information about safe typing, [see Basic
            SAP Data Types](https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/basic-sap-data-types 'https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/basic-sap-data-types').

The default is false; safe typing is disabled.