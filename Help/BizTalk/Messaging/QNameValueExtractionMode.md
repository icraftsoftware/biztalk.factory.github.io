#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema.Annotation](Be.Stateless.BizTalk.Schema.Annotation.md 'Be.Stateless.BizTalk.Schema.Annotation')

## QNameValueExtractionMode Enum

Denotes how the value, which might be a QName, pointed to by an [QNameValueExtractor](QNameValueExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor') is extracted.
This is typically the case for the [System.Xml.Schema.XmlSchema.InstanceNamespace](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema.InstanceNamespace 'System.Xml.Schema.XmlSchema.InstanceNamespace') type attribute's value.

```csharp
public enum QNameValueExtractionMode
```
### Fields

<a name='Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode.Default'></a>

`Default` 0

Default extraction mode, i.e. [Name](QNameValueExtractionMode.md#Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode.Name 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode.Name').

<a name='Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode.LocalName'></a>

`LocalName` 1

Extracts only the local part QName, i.e. the equivalent of the local-name() xpath function.

### Remarks
This extraction mode usually allows to discard the xml namespace prefix from the [System.Xml.Schema.XmlSchema.InstanceNamespace](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema.InstanceNamespace 'System.Xml.Schema.XmlSchema.InstanceNamespace') type attribute's value and therefore allows to write subscription filters
against xml type names without having to care about varying xml namespace prefixes that can mangle the type
name.

<a name='Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode.Name'></a>

`Name` 0

Extracts the whole QName, i.e. the equivalent of the name() xpath function.

### Remarks
Notice that this extraction mode will keep the xml namespace prefix in the extracted value if present and is
therefore not the recommended way to extract an [System.Xml.Schema.XmlSchema.InstanceNamespace](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema.InstanceNamespace 'System.Xml.Schema.XmlSchema.InstanceNamespace') type attribute's if
one wants to write a subscription filter against a type name.

### Remarks
Extraction can either means
- [Name](QNameValueExtractionMode.md#Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode.Name 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode.Name') — the name() of the QName value is extracted. This is the default extraction mode.
- [LocalName](QNameValueExtractionMode.md#Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode.LocalName 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode.LocalName') — only the local-name() of the QName value is extracted.

### See Also
- [Qualified Names](http://www.w3.org/TR/xml-names/#ns-qualnames 'http://www.w3.org/TR/xml-names/#ns-qualnames')