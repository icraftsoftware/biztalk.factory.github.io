#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Interop](Be.Stateless.BizTalk.Dsl.Binding.Interop.md 'Be.Stateless.BizTalk.Dsl.Binding.Interop')

## PropertyBag Class

Provides an object with a property bag in which the object can save its properties persistently.

```csharp
public class PropertyBag :
Microsoft.BizTalk.Component.Interop.IPropertyBag,
Microsoft.BizTalk.ExplorerOM.IPropertyBag,
System.Xml.Serialization.IXmlSerializable
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; PropertyBag

Implements [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag'), [Microsoft.BizTalk.ExplorerOM.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.ExplorerOM.IPropertyBag 'Microsoft.BizTalk.ExplorerOM.IPropertyBag'), [System.Xml.Serialization.IXmlSerializable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable 'System.Xml.Serialization.IXmlSerializable')

### See Also
- [Microsoft.BizTalk.Internal.BTMPropertyBag](Microsoft.BizTalk.Internal.BTMPropertyBag 'Microsoft.BizTalk.Internal.BTMPropertyBag')

| Properties | |
| :--- | :--- |
| [Bag](PropertyBag.Bag.md 'Be.Stateless.BizTalk.Dsl.Binding.Interop.PropertyBag.Bag') | |
| [Count](PropertyBag.Count.md 'Be.Stateless.BizTalk.Dsl.Binding.Interop.PropertyBag.Count') | |
| [Properties](PropertyBag.Properties.md 'Be.Stateless.BizTalk.Dsl.Binding.Interop.PropertyBag.Properties') | |

| Methods | |
| :--- | :--- |
| [GetSchema()](PropertyBag.GetSchema().md 'Be.Stateless.BizTalk.Dsl.Binding.Interop.PropertyBag.GetSchema()') | |
| [Read(string, object, int)](PropertyBag.Read(string,object,int).md 'Be.Stateless.BizTalk.Dsl.Binding.Interop.PropertyBag.Read(string, object, int)') | Reads a named property from the property bag. |
| [ReadXml(XmlReader)](PropertyBag.ReadXml(XmlReader).md 'Be.Stateless.BizTalk.Dsl.Binding.Interop.PropertyBag.ReadXml(System.Xml.XmlReader)') | |
| [ToString()](PropertyBag.ToString().md 'Be.Stateless.BizTalk.Dsl.Binding.Interop.PropertyBag.ToString()') | |
| [Write(string, object)](PropertyBag.Write(string,object).md 'Be.Stateless.BizTalk.Dsl.Binding.Interop.PropertyBag.Write(string, object)') | Saves a named property into the property bag. |
| [WriteXml(XmlWriter)](PropertyBag.WriteXml(XmlWriter).md 'Be.Stateless.BizTalk.Dsl.Binding.Interop.PropertyBag.WriteXml(System.Xml.XmlWriter)') | |
