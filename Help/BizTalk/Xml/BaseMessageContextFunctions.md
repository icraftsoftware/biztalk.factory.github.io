#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Message.ExtensionObjects](Be.Stateless.BizTalk.Message.ExtensionObjects.md 'Be.Stateless.BizTalk.Message.ExtensionObjects')

## BaseMessageContextFunctions Class

XSLT extension object offering support for the [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext') of the current [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage').

```csharp
public class BaseMessageContextFunctions
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; BaseMessageContextFunctions

### See Also
- [System.Xml.Xsl.XsltArgumentList.AddExtensionObject(System.String,System.Object)](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XsltArgumentList.AddExtensionObject#System_Xml_Xsl_XsltArgumentList_AddExtensionObject_System_String,System_Object_ 'System.Xml.Xsl.XsltArgumentList.AddExtensionObject(System.String,System.Object)')

| Constructors | |
| :--- | :--- |
| [BaseMessageContextFunctions(IBaseMessageContext, IXmlNamespaceResolver)](BaseMessageContextFunctions.BaseMessageContextFunctions(IBaseMessageContext,IXmlNamespaceResolver).md 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions.BaseMessageContextFunctions(Microsoft.BizTalk.Message.Interop.IBaseMessageContext, System.Xml.IXmlNamespaceResolver)') | |

| Methods | |
| :--- | :--- |
| [Promote(string, string)](BaseMessageContextFunctions.Promote(string,string).md 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions.Promote(string, string)') | Promote the property, identified by its XML Qualified name, with a given value into the current message context. |
| [Read(string)](BaseMessageContextFunctions.Read(string).md 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions.Read(string)') | Returns the value of the property, identified by its XML Qualified name, from the current message context. |
| [Write(string, string)](BaseMessageContextFunctions.Write(string,string).md 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions.Write(string, string)') | Write the property, identified by its XML Qualified name, with a given value into the current message context. |
