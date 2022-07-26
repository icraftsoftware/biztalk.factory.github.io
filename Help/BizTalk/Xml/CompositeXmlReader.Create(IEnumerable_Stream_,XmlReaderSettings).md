#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Xml](Be.Stateless.BizTalk.Xml.md 'Be.Stateless.BizTalk.Xml').[CompositeXmlReader](CompositeXmlReader.md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader')

## CompositeXmlReader.Create(IEnumerable<Stream>, XmlReaderSettings) Method

Creates a new [CompositeXmlReader](CompositeXmlReader.md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader') instance wrapping a set of XML data [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s as specified
by [streams](CompositeXmlReader.Create(IEnumerable_Stream_,XmlReaderSettings).md#Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable_System.IO.Stream_,System.Xml.XmlReaderSettings).streams 'Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable<System.IO.Stream>, System.Xml.XmlReaderSettings).streams') and with the specified [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') object.

```csharp
public static System.Xml.XmlReader Create(System.Collections.Generic.IEnumerable<System.IO.Stream> streams, System.Xml.XmlReaderSettings settings=null);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable_System.IO.Stream_,System.Xml.XmlReaderSettings).streams'></a>

`streams` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

The set of compound [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s containing the pieces of XML data to wrap.

<a name='Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable_System.IO.Stream_,System.Xml.XmlReaderSettings).settings'></a>

`settings` [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings')

The [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') object used to configure the new [CompositeXmlReader](CompositeXmlReader.md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader') instance. This
value can be `null`.

#### Returns
[System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')  
A [CompositeXmlReader](CompositeXmlReader.md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader') object to read the compound XML [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s as a whole XML composite.