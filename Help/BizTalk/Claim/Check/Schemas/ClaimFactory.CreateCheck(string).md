#### [Be.Stateless.BizTalk.Claim.Check.Schemas](README.md 'README')
### [Be.Stateless.BizTalk.Message](Be.Stateless.BizTalk.Message.md 'Be.Stateless.BizTalk.Message').[ClaimFactory](ClaimFactory.md 'Be.Stateless.BizTalk.Message.ClaimFactory')

## ClaimFactory.CreateCheck(string) Method

Creates a [Be.Stateless.BizTalk.Schemas.Xml.Claim.Check](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schemas.Xml.Claim.Check 'Be.Stateless.BizTalk.Schemas.Xml.Claim.Check') message with a given [url](ClaimFactory.CreateCheck(string).md#Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheck(string).url 'Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheck(string).url') claim.

```csharp
public static System.Xml.XmlDocument CreateCheck(string url);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheck(string).url'></a>

`url` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The URL to some payload that will later on be checked out.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
The [Be.Stateless.BizTalk.Schemas.Xml.Claim.Check](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schemas.Xml.Claim.Check 'Be.Stateless.BizTalk.Schemas.Xml.Claim.Check') message as an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').