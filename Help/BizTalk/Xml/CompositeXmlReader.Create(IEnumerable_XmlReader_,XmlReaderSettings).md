#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Xml](Be.Stateless.BizTalk.Xml.md 'Be.Stateless.BizTalk.Xml').[CompositeXmlReader](CompositeXmlReader.md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader')

## CompositeXmlReader.Create(IEnumerable<XmlReader>, XmlReaderSettings) Method

Creates a new [CompositeXmlReader](CompositeXmlReader.md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader') instance wrapping a set of XML data [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')s as
specified by [readers](CompositeXmlReader.Create(IEnumerable_XmlReader_,XmlReaderSettings).md#Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable_System.Xml.XmlReader_,System.Xml.XmlReaderSettings).readers 'Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable<System.Xml.XmlReader>, System.Xml.XmlReaderSettings).readers') and with the specified [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') object.

```csharp
public static System.Xml.XmlReader Create(System.Collections.Generic.IEnumerable<System.Xml.XmlReader> readers, System.Xml.XmlReaderSettings settings=null);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable_System.Xml.XmlReader_,System.Xml.XmlReaderSettings).readers'></a>

`readers` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

The set of compound [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')s containing the pieces of XML data to wrap.

<a name='Be.Stateless.BizTalk.Xml.CompositeXmlReader.Create(System.Collections.Generic.IEnumerable_System.Xml.XmlReader_,System.Xml.XmlReaderSettings).settings'></a>

`settings` [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings')

The [System.Xml.XmlReaderSettings](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReaderSettings 'System.Xml.XmlReaderSettings') object used to configure the new [CompositeXmlReader](CompositeXmlReader.md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader') instance. This
value can be `null`.

#### Returns
[System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')  
A [CompositeXmlReader](CompositeXmlReader.md 'Be.Stateless.BizTalk.Xml.CompositeXmlReader') object to read the compound XML [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s as a whole XML composite.