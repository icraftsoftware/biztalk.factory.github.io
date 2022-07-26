#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.Xsl](Be.Stateless.Xml.Xsl.md 'Be.Stateless.Xml.Xsl').[XsltArgumentList](XsltArgumentList.md 'Be.Stateless.Xml.Xsl.XsltArgumentList')

## XsltArgumentList.Union(object[]) Method

Adds custom transform arguments to the transform argument list.

```csharp
public System.Xml.Xsl.XsltArgumentList Union(object[] splatteredArguments);
```
#### Parameters

<a name='Be.Stateless.Xml.Xsl.XsltArgumentList.Union(object[]).splatteredArguments'></a>

`splatteredArguments` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

The arguments to add to the list. The array must contain a number of items that is a multiple of 3. Each series of 3
items contains, in that order, an XSL parameter name, the namespace URI of the parameter, and its value.

#### Returns
[System.Xml.Xsl.XsltArgumentList](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XsltArgumentList 'System.Xml.Xsl.XsltArgumentList')  
A new list being the result of the union.