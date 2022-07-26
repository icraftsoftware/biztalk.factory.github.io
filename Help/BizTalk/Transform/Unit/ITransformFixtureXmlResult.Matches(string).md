#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Transform](Be.Stateless.BizTalk.Unit.Transform.md 'Be.Stateless.BizTalk.Unit.Transform').[ITransformFixtureXmlResult](ITransformFixtureXmlResult.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult')

## ITransformFixtureXmlResult.Matches(string) Method

Determines whether the current node matches the specified XPath expression implicitly using the [NamespaceManager](ITransformFixtureXmlResult.NamespaceManager.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.NamespaceManager') to resolve namespace prefixes.

```csharp
bool Matches(string xpath);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.Matches(string).xpath'></a>

`xpath` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

A [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') representing an XPath expression.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
[true](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/bool 'https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/bool') if the current node matches the specified XPath expression; otherwise, [false](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/bool 'https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/bool').