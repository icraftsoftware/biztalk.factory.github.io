#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Message.ExtensionObjects](Be.Stateless.BizTalk.Message.ExtensionObjects.md 'Be.Stateless.BizTalk.Message.ExtensionObjects').[BaseMessageContextFunctions](BaseMessageContextFunctions.md 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions')

## BaseMessageContextFunctions.Promote(string, string) Method

Promote the property, identified by its XML Qualified name, with a given value into the current message context.

```csharp
public void Promote(string qName, string value);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions.Promote(string,string).qName'></a>

`qName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The XML Qualified name of the property, e.g. `bts:MessageType`.

<a name='Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions.Promote(string,string).value'></a>

`value` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The property value as a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String').

### Remarks
[qName](BaseMessageContextFunctions.Promote(string,string).md#Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions.Promote(string,string).qName 'Be.Stateless.BizTalk.Message.ExtensionObjects.BaseMessageContextFunctions.Promote(string, string).qName') has to be an XML Qualified of the form `ns:name` where
            
- `ns` is the prefix that the XSLT, to which an instance of this class will be added as an extension object,
              defines when declaring the target namespace of some property schema;
- `name` is the name a property defined in the latter property schema.