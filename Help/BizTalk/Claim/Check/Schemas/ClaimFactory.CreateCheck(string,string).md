#### [Be.Stateless.BizTalk.Claim.Check.Schemas](README.md 'README')
### [Be.Stateless.BizTalk.Message](Be.Stateless.BizTalk.Message.md 'Be.Stateless.BizTalk.Message').[ClaimFactory](ClaimFactory.md 'Be.Stateless.BizTalk.Message.ClaimFactory')

## ClaimFactory.CreateCheck(string, string) Method

Creates a [Be.Stateless.BizTalk.Schemas.Xml.Claim.Check](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schemas.Xml.Claim.Check 'Be.Stateless.BizTalk.Schemas.Xml.Claim.Check') message with a given [messageType](ClaimFactory.CreateCheck(string,string).md#Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheck(string,string).messageType 'Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheck(string, string).messageType') and [url](ClaimFactory.CreateCheck(string,string).md#Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheck(string,string).url 'Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheck(string, string).url')
claim.

```csharp
public static System.Xml.XmlDocument CreateCheck(string messageType, string url);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheck(string,string).messageType'></a>

`messageType` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The actual message type of the payload being claimed.

<a name='Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheck(string,string).url'></a>

`url` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The URL to some payload that will later on be checked out.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
The [Be.Stateless.BizTalk.Schemas.Xml.Claim.Check](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schemas.Xml.Claim.Check 'Be.Stateless.BizTalk.Schemas.Xml.Claim.Check') message as an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').