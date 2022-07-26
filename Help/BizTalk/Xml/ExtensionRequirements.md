#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl')

## ExtensionRequirements Enum

Describes the requirements of a [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') in terms of extension objects.

```csharp
public enum ExtensionRequirements
```
### Fields

<a name='Be.Stateless.BizTalk.Xml.Xsl.ExtensionRequirements.MessageContext'></a>

`MessageContext` 1

The [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') needs the [BaseMessageContextFunctions](BaseMessageContextFunctions.md 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions') extension object.

### Remarks
If will automatically be set if the stylesheet markup declares the namespace of the [BaseMessageContextFunctions](BaseMessageContextFunctions.md 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions') (see [Be.Stateless.BizTalk.Namespaces.ExtensionObjectNamespaces.MessageContext](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Namespaces.ExtensionObjectNamespaces.MessageContext 'Be.Stateless.BizTalk.Namespaces.ExtensionObjectNamespaces.MessageContext')).

### See Also
- [Be.Stateless.BizTalk.Namespaces.ExtensionObjectNamespaces.MessageContext](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Namespaces.ExtensionObjectNamespaces.MessageContext 'Be.Stateless.BizTalk.Namespaces.ExtensionObjectNamespaces.MessageContext')

<a name='Be.Stateless.BizTalk.Xml.Xsl.ExtensionRequirements.None'></a>

`None` 0

The [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') has no requirement.