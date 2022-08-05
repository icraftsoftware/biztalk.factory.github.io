#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.UserAssembliesLoadPath Property

Specifies the name of the DLLs, separated by a semi-colon, which the adapter creates while generating metadata.

```csharp
public string UserAssembliesLoadPath { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
These DLLs are saved at the location you specified for the [Microsoft.Adapters.OracleDB.OracleDBBindingConfigurationElement.GeneratedUserTypesAssemblyFilePath](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.OracleDB.OracleDBBindingConfigurationElement.GeneratedUserTypesAssemblyFilePath 'Microsoft.Adapters.OracleDB.OracleDBBindingConfigurationElement.GeneratedUserTypesAssemblyFilePath') property while generating metadata.
You must manually copy these DLLs to the following locations:
- For BizTalk projects, copy the DLLs at the same location as BTSNTSvc.exe. For BizTalk Server 2013 R2, this is
  available typically under <installation drive>:\Program Files\Microsoft BizTalk Server 2013 R2.
- For .NET Projects, copy the DLLs to the \bin\Development folder within your .NET project folder.
This property is required only while sending and receiving messages to perform operations on the Oracle database.