#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema](Be.Stateless.BizTalk.Schema.md 'Be.Stateless.BizTalk.Schema')

## ISchemaAnnotationReader Interface

XML-serialized schema annotation reader.

```csharp
public interface ISchemaAnnotationReader
```

| Properties | |
| :--- | :--- |
| [SchemaMetadata](ISchemaAnnotationReader.SchemaMetadata.md 'Be.Stateless.BizTalk.Schema.ISchemaAnnotationReader.SchemaMetadata') | The [ISchemaMetadata](ISchemaMetadata.md 'Be.Stateless.BizTalk.Schema.ISchemaMetadata') of the [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema for which annotations are being retrieved. |

| Methods | |
| :--- | :--- |
| [GetAnnotationElement(string)](ISchemaAnnotationReader.GetAnnotationElement(string).md 'Be.Stateless.BizTalk.Schema.ISchemaAnnotationReader.GetAnnotationElement(string)') | Get annotation's XML-serialized element by annotation's name. |
