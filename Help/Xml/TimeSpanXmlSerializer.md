#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml')

## TimeSpanXmlSerializer Class

XML serializer surrogate that supports the serialization of [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan').

```csharp
public class TimeSpanXmlSerializer :
System.Xml.Serialization.IXmlSerializable
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; TimeSpanXmlSerializer

Implements [System.Xml.Serialization.IXmlSerializable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable 'System.Xml.Serialization.IXmlSerializable')

| Constructors | |
| :--- | :--- |
| [TimeSpanXmlSerializer()](TimeSpanXmlSerializer.TimeSpanXmlSerializer().md 'Be.Stateless.Xml.TimeSpanXmlSerializer.TimeSpanXmlSerializer()') | |
| [TimeSpanXmlSerializer(string)](TimeSpanXmlSerializer.TimeSpanXmlSerializer(string).md 'Be.Stateless.Xml.TimeSpanXmlSerializer.TimeSpanXmlSerializer(string)') | |

| Methods | |
| :--- | :--- |
| [GetSchema()](TimeSpanXmlSerializer.GetSchema().md 'Be.Stateless.Xml.TimeSpanXmlSerializer.GetSchema()') | |
| [ReadXml(XmlReader)](TimeSpanXmlSerializer.ReadXml(XmlReader).md 'Be.Stateless.Xml.TimeSpanXmlSerializer.ReadXml(System.Xml.XmlReader)') | |
| [WriteXml(XmlWriter)](TimeSpanXmlSerializer.WriteXml(XmlWriter).md 'Be.Stateless.Xml.TimeSpanXmlSerializer.WriteXml(System.Xml.XmlWriter)') | |

| Operators | |
| :--- | :--- |
| [implicit operator TimeSpanXmlSerializer(TimeSpan)](TimeSpanXmlSerializer.implicitoperatorTimeSpanXmlSerializer(TimeSpan).md 'Be.Stateless.Xml.TimeSpanXmlSerializer.op_Implicit Be.Stateless.Xml.TimeSpanXmlSerializer(System.TimeSpan)') | |
| [implicit operator TimeSpan(TimeSpanXmlSerializer)](TimeSpanXmlSerializer.implicitoperatorTimeSpan(TimeSpanXmlSerializer).md 'Be.Stateless.Xml.TimeSpanXmlSerializer.op_Implicit System.TimeSpan(Be.Stateless.Xml.TimeSpanXmlSerializer)') | |
