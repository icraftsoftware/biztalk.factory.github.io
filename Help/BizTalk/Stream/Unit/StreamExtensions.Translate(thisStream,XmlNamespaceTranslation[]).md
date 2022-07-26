#### [Be.Stateless.BizTalk.Stream.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Stream.Extensions](Be.Stateless.BizTalk.Unit.Stream.Extensions.md 'Be.Stateless.BizTalk.Unit.Stream.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.BizTalk.Unit.Stream.Extensions.StreamExtensions')

## StreamExtensions.Translate(this Stream, XmlNamespaceTranslation[]) Method

Applies a set of [Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation 'Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation') translations to an XML [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').

```csharp
public static System.IO.Stream Translate(this System.IO.Stream stream, Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation[] translations);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Stream.Extensions.StreamExtensions.Translate(thisSystem.IO.Stream,Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation[]).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The XML [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') to be translated.

<a name='Be.Stateless.BizTalk.Unit.Stream.Extensions.StreamExtensions.Translate(thisSystem.IO.Stream,Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation[]).translations'></a>

`translations` [Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation 'Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

The set of [Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation 'Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation') translations to apply.

#### Returns
[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')  
The translated [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').