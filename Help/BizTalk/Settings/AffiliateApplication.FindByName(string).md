#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings.Sso](Be.Stateless.BizTalk.Settings.Sso.md 'Be.Stateless.BizTalk.Settings.Sso').[AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')

## AffiliateApplication.FindByName(string) Method

Finds and returns an [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') by name in the Enterprise Single Sign-On (SSO) server
database.

```csharp
public static Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication FindByName(string name);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.FindByName(string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') to find in Enterprise Single Sign-On (SSO) server database.

#### Returns
[AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')  
The [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') currently deployed in the Enterprise Single Sign-On (SSO) server database.
`null` if the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') does not exist in Enterprise Single Sign-On (SSO) server
database.