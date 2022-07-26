#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Xml](Be.Stateless.BizTalk.Xml.md 'Be.Stateless.BizTalk.Xml')

## CompositeXmlReader Class

Aggregates, at the XML information set level, several [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s whose contents is XML.

```csharp
public class CompositeXmlReader : Be.Stateless.Xml.XmlReaderWrapper
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') &#129106; [Be.Stateless.Xml.XmlReaderWrapper](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Xml.XmlReaderWrapper 'Be.Stateless.Xml.XmlReaderWrapper') &#129106; CompositeXmlReader

### Remarks

Because the input streams are aggregated at the XML information set level, the contents of the input streams can be of
various and distinct encodings and might, as well, include or not an [System.Xml.XmlDeclaration](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDeclaration 'System.Xml.XmlDeclaration').

The contents of the aggregated [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s is wrapped in an XML structured as follows:

```csharp
<agg:Root xmlns:agg="http://schemas.microsoft.com/BizTalk/2003/aggschema">
  <agg:InputMessagePart_0>
    ... content of 1st message part ...
  </agg:InputMessagePart_0>
  <agg:InputMessagePart_1>
    ... content of 2nd message part ...
  </agg:InputMessagePart_1>
  ...
  <agg:InputMessagePart_n>
    ... content of nth message part ...
  </agg:InputMessagePart_n>
</agg:Root>
```

### See Also
- [Microsoft.XLANGs.Core.Service.CompositeStreamReader, Microsoft.BizTalk.BtsDbVersion, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35](Microsoft.XLANGs.Core.Service.CompositeStreamReader, Microsoft.BizTalk.BtsDbVersion, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35 'Microsoft.XLANGs.Core.Service.CompositeStreamReader, Microsoft.BizTalk.BtsDbVersion, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35')

| Methods | |
| :--- | :--- |
| [Close()](CompositeXmlReader.Close().md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader.Close()') | |
| [Create(IEnumerable&lt;Stream&gt;, XmlReaderSettings)](CompositeXmlReader.Create(IEnumerable_Stream_,XmlReaderSettings).md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable<System.IO.Stream>, System.Xml.XmlReaderSettings)') | Creates a new [CompositeXmlReader](CompositeXmlReader.md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader') instance wrapping a set of XML data [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s as specified by [streams](CompositeXmlReader.Create(IEnumerable_Stream_,XmlReaderSettings).md#Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable_System.IO.Stream_,System.Xml.XmlReaderSettings).streams 'Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable<System.IO.Stream>, System.Xml.XmlReaderSettings).streams') and with the specified [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') object. |
| [Create(IEnumerable&lt;XmlReader&gt;, XmlReaderSettings)](CompositeXmlReader.Create(IEnumerable_XmlReader_,XmlReaderSettings).md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable<System.Xml.XmlReader>, System.Xml.XmlReaderSettings)') | Creates a new [CompositeXmlReader](CompositeXmlReader.md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader') instance wrapping a set of XML data [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')s as specified by [readers](CompositeXmlReader.Create(IEnumerable_XmlReader_,XmlReaderSettings).md#Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable_System.Xml.XmlReader_,System.Xml.XmlReaderSettings).readers 'Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable<System.Xml.XmlReader>, System.Xml.XmlReaderSettings).readers') and with the specified [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') object. |
| [Read()](CompositeXmlReader.Read().md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader.Read()') | |
