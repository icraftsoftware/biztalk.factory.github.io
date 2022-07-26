#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml')

## ValidatingXmlReaderSettings Class

Creates the necessary [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') that an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') instance needs to validate its
content against one or more XSD schemas while reading it.

```csharp
public static class ValidatingXmlReaderSettings
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ValidatingXmlReaderSettings

| Methods | |
| :--- | :--- |
| [Create(XmlSchemaContentProcessing, ValidationEventHandler, XmlSchema[])](ValidatingXmlReaderSettings.Create(XmlSchemaContentProcessing,ValidationEventHandler,XmlSchema[]).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing, System.Xml.Schema.ValidationEventHandler, System.Xml.Schema.XmlSchema[])') | Specifies a set of [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') features to support XSD validation on the [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object created by the [System.Xml.XmlReader.Create(System.Xml.XmlReader,System.Xml.XmlReaderSettings)](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Create#System_Xml_XmlReader_Create_System_Xml_XmlReader,System_Xml_XmlReaderSettings_ 'System.Xml.XmlReader.Create(System.Xml.XmlReader,System.Xml.XmlReaderSettings)') method or one of its other overloads. |
| [Create(XmlSchemaContentProcessing, XmlSchema[])](ValidatingXmlReaderSettings.Create(XmlSchemaContentProcessing,XmlSchema[]).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create(System.Xml.Schema.XmlSchemaContentProcessing, System.Xml.Schema.XmlSchema[])') | Specifies a set of [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') features to support XSD validation on the [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object created by the [System.Xml.XmlReader.Create(System.Xml.XmlReader,System.Xml.XmlReaderSettings)](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Create#System_Xml_XmlReader_Create_System_Xml_XmlReader,System_Xml_XmlReaderSettings_ 'System.Xml.XmlReader.Create(System.Xml.XmlReader,System.Xml.XmlReaderSettings)') method or one of its other overloads. |
| [Create&lt;T&gt;(XmlSchemaContentProcessing)](ValidatingXmlReaderSettings.Create_T_(XmlSchemaContentProcessing).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create<T>(System.Xml.Schema.XmlSchemaContentProcessing)') | |
| [Create&lt;T1,T2,T3,T4,T5,T6,T7,T8,T9&gt;(XmlSchemaContentProcessing)](ValidatingXmlReaderSettings.Create_T1,T2,T3,T4,T5,T6,T7,T8,T9_(XmlSchemaContentProcessing).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create<T1,T2,T3,T4,T5,T6,T7,T8,T9>(System.Xml.Schema.XmlSchemaContentProcessing)') | |
| [Create&lt;T1,T2,T3,T4,T5,T6,T7,T8&gt;(XmlSchemaContentProcessing)](ValidatingXmlReaderSettings.Create_T1,T2,T3,T4,T5,T6,T7,T8_(XmlSchemaContentProcessing).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create<T1,T2,T3,T4,T5,T6,T7,T8>(System.Xml.Schema.XmlSchemaContentProcessing)') | |
| [Create&lt;T1,T2,T3,T4,T5,T6,T7&gt;(XmlSchemaContentProcessing)](ValidatingXmlReaderSettings.Create_T1,T2,T3,T4,T5,T6,T7_(XmlSchemaContentProcessing).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create<T1,T2,T3,T4,T5,T6,T7>(System.Xml.Schema.XmlSchemaContentProcessing)') | |
| [Create&lt;T1,T2,T3,T4,T5,T6&gt;(XmlSchemaContentProcessing)](ValidatingXmlReaderSettings.Create_T1,T2,T3,T4,T5,T6_(XmlSchemaContentProcessing).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create<T1,T2,T3,T4,T5,T6>(System.Xml.Schema.XmlSchemaContentProcessing)') | |
| [Create&lt;T1,T2,T3,T4,T5&gt;(XmlSchemaContentProcessing)](ValidatingXmlReaderSettings.Create_T1,T2,T3,T4,T5_(XmlSchemaContentProcessing).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create<T1,T2,T3,T4,T5>(System.Xml.Schema.XmlSchemaContentProcessing)') | |
| [Create&lt;T1,T2,T3,T4&gt;(XmlSchemaContentProcessing)](ValidatingXmlReaderSettings.Create_T1,T2,T3,T4_(XmlSchemaContentProcessing).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create<T1,T2,T3,T4>(System.Xml.Schema.XmlSchemaContentProcessing)') | |
| [Create&lt;T1,T2,T3&gt;(XmlSchemaContentProcessing)](ValidatingXmlReaderSettings.Create_T1,T2,T3_(XmlSchemaContentProcessing).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create<T1,T2,T3>(System.Xml.Schema.XmlSchemaContentProcessing)') | |
| [Create&lt;T1,T2&gt;(XmlSchemaContentProcessing)](ValidatingXmlReaderSettings.Create_T1,T2_(XmlSchemaContentProcessing).md 'Be.Stateless.Xml.ValidatingXmlReaderSettings.Create<T1,T2>(System.Xml.Schema.XmlSchemaContentProcessing)') | |
