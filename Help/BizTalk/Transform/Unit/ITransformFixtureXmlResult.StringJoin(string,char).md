#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Transform](Be.Stateless.BizTalk.Unit.Transform.md 'Be.Stateless.BizTalk.Unit.Transform').[ITransformFixtureXmlResult](ITransformFixtureXmlResult.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult')

## ITransformFixtureXmlResult.StringJoin(string, char) Method

Concatenates all the text values of the nodes selected using the specified XPath expression and uses the specified
separator between each value.

```csharp
string StringJoin(string xpath, char separator='#');
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.StringJoin(string,char).xpath'></a>

`xpath` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

A [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') representing an XPath expression.

<a name='Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.StringJoin(string,char).separator'></a>

`separator` [System.Char](https://docs.microsoft.com/en-us/dotnet/api/System.Char 'System.Char')

The [System.Char](https://docs.microsoft.com/en-us/dotnet/api/System.Char 'System.Char') to use as a separator; it defaults to '#'.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
A string that consists of the selected nodes' values delimited by the separator [System.Char](https://docs.microsoft.com/en-us/dotnet/api/System.Char 'System.Char').

### Remarks
[StringJoin(string, char)](ITransformFixtureXmlResult.StringJoin(string,char).md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.StringJoin(string, char)') automatically benefits of an [System.Xml.IXmlNamespaceResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.IXmlNamespaceResolver 'System.Xml.IXmlNamespaceResolver')
            resolver that declares all of the namespaces that the XSLT transform of [TransformFixture&lt;TTransform&gt;](TransformFixture_TTransform_.md 'Be.Stateless.BizTalk.Unit.Transform.TransformFixture<TTransform>') have
            declared.

### See Also
- [http://www.w3.org/TR/2002/WD-xquery-operators-20021115/#func-string-join](http://www.w3.org/TR/2002/WD-xquery-operators-20021115/#func-string-join 'http://www.w3.org/TR/2002/WD-xquery-operators-20021115/#func-string-join')