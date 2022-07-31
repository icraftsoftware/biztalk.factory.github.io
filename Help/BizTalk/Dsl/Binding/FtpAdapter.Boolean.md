#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter')

## FtpAdapter.Boolean Class

Hack to serialize [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') back and forth to Pascal-cased strings.

```csharp
public class FtpAdapter.Boolean :
System.Xml.Serialization.IXmlSerializable
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; Boolean

Implements [System.Xml.Serialization.IXmlSerializable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable 'System.Xml.Serialization.IXmlSerializable')

### Remarks
This class is intended to be used only with [FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter')-derived classes.

| Constructors | |
| :--- | :--- |
| [Boolean()](FtpAdapter.Boolean.Boolean().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean.Boolean()') | |

| Properties | |
| :--- | :--- |
| [False](FtpAdapter.Boolean.False.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean.False') | |
| [True](FtpAdapter.Boolean.True.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean.True') | |

| Methods | |
| :--- | :--- |
| [GetSchema()](FtpAdapter.Boolean.GetSchema().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean.GetSchema()') | |
| [ReadXml(XmlReader)](FtpAdapter.Boolean.ReadXml(XmlReader).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean.ReadXml(System.Xml.XmlReader)') | |
| [WriteXml(XmlWriter)](FtpAdapter.Boolean.WriteXml(XmlWriter).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean.WriteXml(System.Xml.XmlWriter)') | |

| Operators | |
| :--- | :--- |
| [implicit operator Boolean(bool)](FtpAdapter.Boolean.implicitoperatorBoolean(bool).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean.op_Implicit Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean(bool)') | |
| [implicit operator bool(Boolean)](FtpAdapter.Boolean.implicitoperatorbool(Boolean).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean.op_Implicit bool(Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean)') | |
