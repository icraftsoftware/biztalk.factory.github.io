#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema](Be.Stateless.BizTalk.Schema.md 'Be.Stateless.BizTalk.Schema').[ISchemaAnnotationReader](ISchemaAnnotationReader.md 'Be.Stateless.BizTalk.Schema.ISchemaAnnotationReader')

## ISchemaAnnotationReader.GetAnnotationElement(string) Method

Get annotation's XML-serialized element by annotation's name.

```csharp
System.Xml.Linq.XElement GetAnnotationElement(string annotationElementLocalName);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Schema.ISchemaAnnotationReader.GetAnnotationElement(string).annotationElementLocalName'></a>

`annotationElementLocalName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

Local name of the annotation whose XML-serialized element need to be returned.

#### Returns
[System.Xml.Linq.XElement](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Linq.XElement 'System.Xml.Linq.XElement')  
XML-serialized element for annotation whose name is [annotationElementLocalName](ISchemaAnnotationReader.GetAnnotationElement(string).md#Be.Stateless.BizTalk.Schema.ISchemaAnnotationReader.GetAnnotationElement(string).annotationElementLocalName 'Be.Stateless.BizTalk.Schema.ISchemaAnnotationReader.GetAnnotationElement(string).annotationElementLocalName').