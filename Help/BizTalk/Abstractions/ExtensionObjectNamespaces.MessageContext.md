#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Namespaces](Be.Stateless.BizTalk.Namespaces.md 'Be.Stateless.BizTalk.Namespaces').[ExtensionObjectNamespaces](ExtensionObjectNamespaces.md 'Be.Stateless.BizTalk.Namespaces.ExtensionObjectNamespaces')

## ExtensionObjectNamespaces.MessageContext Field

The namespace that any XSLT must declare to <b>automatically</b> benefit from an extension object supporting [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext') read, write, and promote operations.

```csharp
public const string MessageContext = urn:extensions.stateless.be:biztalk:message:context:2012:12;
```

#### Field Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
If an XSLT choose not to declare this namespace then it is up to itself to instantiate this class and add it as an
extension object.