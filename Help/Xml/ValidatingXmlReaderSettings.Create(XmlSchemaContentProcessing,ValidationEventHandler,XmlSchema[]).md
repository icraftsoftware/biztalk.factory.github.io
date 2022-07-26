#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[ValidatingXmlReaderSettings](ValidatingXmlReaderSettings.md 'Be.Stateless.Xml.ValidatingXmlReaderSettings')

## ValidatingXmlReaderSettings.Create(XmlSchemaContentProcessing, ValidationEventHandler, XmlSchema[]) Method

Specifies a set of [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') features to support XSD validation on the [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')
object created by the [System.Xml.XmlReader.Create(System.Xml.XmlReader,System.Xml.XmlReaderSettings)](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Create#System_Xml_XmlReader_Create_System_Xml_XmlReader,System_Xml_XmlReaderSettings_ 'System.Xml.XmlReader.Create(System.Xml.XmlReader,System.Xml.XmlReaderSettings)') method or one of its other
overloads.

```csharp
public static System.Xml.XmlReaderSettings Create(System.Xml.Schema.XmlSchemaContentProcessing contentProcessing, System.Xml.Schema.ValidationEventHandler validationEventHandler, params System.Xml.Schema.XmlSchema[] schemas);
```
#### Parameters

<a name='Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing,System.Xml.Schema.ValidationEventHandler,System.Xml.Schema.XmlSchema[]).contentProcessing'></a>

`contentProcessing` [System.Xml.Schema.XmlSchemaContentProcessing](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing 'System.Xml.Schema.XmlSchemaContentProcessing')

The validation mode of the whole document and not only the any and anyAttribute element replacements.

<a name='Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing,System.Xml.Schema.ValidationEventHandler,System.Xml.Schema.XmlSchema[]).validationEventHandler'></a>

`validationEventHandler` [System.Xml.Schema.ValidationEventHandler](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.ValidationEventHandler 'System.Xml.Schema.ValidationEventHandler')

Represents the callback method that will handle XML schema validation events and the [System.Xml.Schema.ValidationEventArgs](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.ValidationEventArgs 'System.Xml.Schema.ValidationEventArgs'). Notice the callback will only be invoked if there is an exception thrown by the
validating [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader'), via [System.Xml.Schema.ValidationEventArgs](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.ValidationEventArgs 'System.Xml.Schema.ValidationEventArgs').[System.Xml.Schema.ValidationEventArgs.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.ValidationEventArgs.Exception 'System.Xml.Schema.ValidationEventArgs.Exception'), and [contentProcessing](ValidatingXmlReaderSettings.Create(XmlSchemaContentProcessing,ValidationEventHandler,XmlSchema[]).md#Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing,System.Xml.Schema.ValidationEventHandler,System.Xml.Schema.XmlSchema[]).contentProcessing 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing, System.Xml.Schema.ValidationEventHandler, System.Xml.Schema.XmlSchema[]).contentProcessing') is different than [System.Xml.Schema.XmlSchemaContentProcessing.Skip](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing.Skip 'System.Xml.Schema.XmlSchemaContentProcessing.Skip').

<a name='Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing,System.Xml.Schema.ValidationEventHandler,System.Xml.Schema.XmlSchema[]).schemas'></a>

`schemas` [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

The XSD schemas against which to validate the XML content.

#### Returns
[System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings')  
The [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') needed by an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') instance needs to validate its content
against the given XSD [schemas](ValidatingXmlReaderSettings.Create(XmlSchemaContentProcessing,ValidationEventHandler,XmlSchema[]).md#Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing,System.Xml.Schema.ValidationEventHandler,System.Xml.Schema.XmlSchema[]).schemas 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing, System.Xml.Schema.ValidationEventHandler, System.Xml.Schema.XmlSchema[]).schemas').

### Remarks

If [contentProcessing](ValidatingXmlReaderSettings.Create(XmlSchemaContentProcessing,ValidationEventHandler,XmlSchema[]).md#Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing,System.Xml.Schema.ValidationEventHandler,System.Xml.Schema.XmlSchema[]).contentProcessing 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing, System.Xml.Schema.ValidationEventHandler, System.Xml.Schema.XmlSchema[]).contentProcessing') is [System.Xml.Schema.XmlSchemaContentProcessing.Lax](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing.Lax 'System.Xml.Schema.XmlSchemaContentProcessing.Lax'), the [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')
won't fail the validation if it cannot obtain a schema for any of the processed XML namespaces.

If the [contentProcessing](ValidatingXmlReaderSettings.Create(XmlSchemaContentProcessing,ValidationEventHandler,XmlSchema[]).md#Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing,System.Xml.Schema.ValidationEventHandler,System.Xml.Schema.XmlSchema[]).contentProcessing 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing, System.Xml.Schema.ValidationEventHandler, System.Xml.Schema.XmlSchema[]).contentProcessing') is [System.Xml.Schema.XmlSchemaContentProcessing.Strict](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing.Strict 'System.Xml.Schema.XmlSchemaContentProcessing.Strict'), the [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') will fail the validation if it cannot obtain a schema for any of the processed XML namespaces and,
more specifically, any reported validation warning ([System.Xml.Schema.XmlSchemaValidationFlags.ReportValidationWarnings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaValidationFlags.ReportValidationWarnings 'System.Xml.Schema.XmlSchemaValidationFlags.ReportValidationWarnings'))
will converted into an [System.Xml.Schema.XmlSchemaValidationException](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaValidationException 'System.Xml.Schema.XmlSchemaValidationException').

### See Also
- [System.Xml.Schema.XmlSchemaContentProcessing](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing 'System.Xml.Schema.XmlSchemaContentProcessing')