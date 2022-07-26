#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.LookupNamespace(string) Method

Resolves a namespace prefix in the current element's scope.

```csharp
public override string LookupNamespace(string prefix);
```
#### Parameters

<a name='Be.Stateless.Xml.XmlBuilderReader.LookupNamespace(string).prefix'></a>

`prefix` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The prefix whose namespace URI you want to resolve. To match the default namespace, pass an empty string.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The namespace URI to which the prefix maps or `null` if no matching prefix is found.