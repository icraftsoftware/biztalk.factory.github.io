#### [Be.Stateless.BizTalk.Claim.Check.Schemas](README.md 'README')
### [Be.Stateless.BizTalk.Message](Be.Stateless.BizTalk.Message.md 'Be.Stateless.BizTalk.Message').[ClaimFactory](ClaimFactory.md 'Be.Stateless.BizTalk.Message.ClaimFactory')

## ClaimFactory.CreateCheckOut(string) Method

Creates a [Be.Stateless.BizTalk.Schemas.Xml.Claim.CheckOut](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schemas.Xml.Claim.CheckOut 'Be.Stateless.BizTalk.Schemas.Xml.Claim.CheckOut') message with a given [url](ClaimFactory.CreateCheckOut(string).md#Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheckOut(string).url 'Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheckOut(string).url') claim.

```csharp
public static System.Xml.XmlDocument CreateCheckOut(string url);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Message.ClaimFactory.CreateCheckOut(string).url'></a>

`url` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The URL to some payload that is to be checked out.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
The [Be.Stateless.BizTalk.Schemas.Xml.Claim.CheckOut](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schemas.Xml.Claim.CheckOut 'Be.Stateless.BizTalk.Schemas.Xml.Claim.CheckOut') message as an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').