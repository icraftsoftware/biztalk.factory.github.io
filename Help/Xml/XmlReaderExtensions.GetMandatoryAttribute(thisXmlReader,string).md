#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.Extensions](Be.Stateless.Xml.Extensions.md 'Be.Stateless.Xml.Extensions').[XmlReaderExtensions](XmlReaderExtensions.md 'Be.Stateless.Xml.Extensions.XmlReaderExtensions')

## XmlReaderExtensions.GetMandatoryAttribute(this XmlReader, string) Method

Gets the value of the attribute with the specified [name](XmlReaderExtensions.GetMandatoryAttribute(thisXmlReader,string).md#Be.Stateless.Xml.Extensions.XmlReaderExtensions.GetMandatoryAttribute(thisSystem.Xml.XmlReader,string).name 'Be.Stateless.Xml.Extensions.XmlReaderExtensions.GetMandatoryAttribute(this System.Xml.XmlReader, string).name'); throws if the value is either not found
or [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').

```csharp
public static string GetMandatoryAttribute(this System.Xml.XmlReader reader, string name);
```
#### Parameters

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.GetMandatoryAttribute(thisSystem.Xml.XmlReader,string).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

An [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.GetMandatoryAttribute(thisSystem.Xml.XmlReader,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The qualified name of the attribute.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The value of the specified attribute.

#### Exceptions

[System.ArgumentNullException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentNullException 'System.ArgumentNullException')  
[name](XmlReaderExtensions.GetMandatoryAttribute(thisXmlReader,string).md#Be.Stateless.Xml.Extensions.XmlReaderExtensions.GetMandatoryAttribute(thisSystem.Xml.XmlReader,string).name 'Be.Stateless.Xml.Extensions.XmlReaderExtensions.GetMandatoryAttribute(this System.Xml.XmlReader, string).name') is `null`.

[System.Xml.XmlException](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlException 'System.Xml.XmlException')  
The attribute is not found or the value is [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').