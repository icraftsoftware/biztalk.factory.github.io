#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl').[XslCompiledTransformDescriptor](XslCompiledTransformDescriptor.md 'Be.Stateless.BizTalk.Xml.Xsl.XslCompiledTransformDescriptor')

## XslCompiledTransformDescriptor.NamespaceResolver Property

The [System.Xml.IXmlNamespaceResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.IXmlNamespaceResolver 'System.Xml.IXmlNamespaceResolver') that will be passed to the [BaseMessageContextFunctions](BaseMessageContextFunctions.md 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions') extension
object.

```csharp
public System.Xml.IXmlNamespaceResolver NamespaceResolver { get; }
```

#### Property Value
[System.Xml.IXmlNamespaceResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.IXmlNamespaceResolver 'System.Xml.IXmlNamespaceResolver')

### Remarks
The [System.Xml.IXmlNamespaceResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.IXmlNamespaceResolver 'System.Xml.IXmlNamespaceResolver') resolver will automatically resolve all of the namespaces declared in the
stylesheet markup of [XslCompiledTransform](XslCompiledTransformDescriptor.XslCompiledTransform.md 'Be.Stateless.BizTalk.Xml.Xsl.XslCompiledTransformDescriptor.XslCompiledTransform') and is therefore suited to help [BaseMessageContextFunctions](BaseMessageContextFunctions.md 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions') extensions objects to resolve the namespace prefix of the XML Qualified name
passed to [Read(string)](BaseMessageContextFunctions.Read(string).md 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions.Read(string)').