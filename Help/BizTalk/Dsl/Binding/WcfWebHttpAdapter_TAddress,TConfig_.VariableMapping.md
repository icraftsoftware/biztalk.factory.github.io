#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter&lt;TAddress,TConfig&gt;](WcfWebHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>')

## WcfWebHttpAdapter<TAddress,TConfig>.VariableMapping Property

Allows to specify what the variable maps to at runtime if variables have been declared in the HTTP Method URL
Mappings.

```csharp
public string VariableMapping { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
You must specify the name of the property that provides the value to be associated to the variable. You must have
already defined/promoted this property as part of your solution. You must also provide the namespace for the property
in the Property Namespace field.

### See Also
- [Be.Stateless.BizTalk.Adapter.Metadata.VariableMapping](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Adapter.Metadata.VariableMapping 'Be.Stateless.BizTalk.Adapter.Metadata.VariableMapping')
- [Be.Stateless.BizTalk.Adapter.Metadata.VariablePropertyMapping](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Adapter.Metadata.VariablePropertyMapping 'Be.Stateless.BizTalk.Adapter.Metadata.VariablePropertyMapping')