#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Schema.Extensions](Be.Stateless.BizTalk.Xml.Schema.Extensions.md 'Be.Stateless.BizTalk.Xml.Schema.Extensions').[XmlSchemaExtensions](XmlSchemaExtensions.md 'Be.Stateless.BizTalk.Xml.Schema.Extensions.XmlSchemaExtensions')

## XmlSchemaExtensions.Merge(this XmlSchema, XmlSchema) Method

Merge an [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') into another [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema').

```csharp
public static System.Xml.Schema.XmlSchema Merge(this System.Xml.Schema.XmlSchema existingSchema, System.Xml.Schema.XmlSchema schema);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.Schema.Extensions.XmlSchemaExtensions.Merge(thisSystem.Xml.Schema.XmlSchema,System.Xml.Schema.XmlSchema).existingSchema'></a>

`existingSchema` [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema')

The [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') into which the other [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') will be merged.

<a name='Be.Stateless.BizTalk.Xml.Schema.Extensions.XmlSchemaExtensions.Merge(thisSystem.Xml.Schema.XmlSchema,System.Xml.Schema.XmlSchema).schema'></a>

`schema` [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema')

The [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') to be merged into the other [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema').

#### Returns
[System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema')  
The resulting [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema'); i.e. the [existingSchema](XmlSchemaExtensions.Merge(thisXmlSchema,XmlSchema).md#Be.Stateless.BizTalk.Xml.Schema.Extensions.XmlSchemaExtensions.Merge(thisSystem.Xml.Schema.XmlSchema,System.Xml.Schema.XmlSchema).existingSchema 'Be.Stateless.BizTalk.Xml.Schema.Extensions.XmlSchemaExtensions.Merge(this System.Xml.Schema.XmlSchema, System.Xml.Schema.XmlSchema).existingSchema') into which the other [schema](XmlSchemaExtensions.Merge(thisXmlSchema,XmlSchema).md#Be.Stateless.BizTalk.Xml.Schema.Extensions.XmlSchemaExtensions.Merge(thisSystem.Xml.Schema.XmlSchema,System.Xml.Schema.XmlSchema).schema 'Be.Stateless.BizTalk.Xml.Schema.Extensions.XmlSchemaExtensions.Merge(this System.Xml.Schema.XmlSchema, System.Xml.Schema.XmlSchema).schema') has been merged.

### See Also
- [http://stackoverflow.com/questions/6312154/xmlschema-removing-duplicate-types](http://stackoverflow.com/questions/6312154/xmlschema-removing-duplicate-types 'http://stackoverflow.com/questions/6312154/xmlschema-removing-duplicate-types')