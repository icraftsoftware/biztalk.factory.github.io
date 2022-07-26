#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings.Sso](Be.Stateless.BizTalk.Settings.Sso.md 'Be.Stateless.BizTalk.Settings.Sso').[AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')

## AffiliateApplication.Create(string, string[], string[], string) Method

Creates an [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') in the Enterprise Single Sign-On (SSO) server database.

```csharp
public static Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication Create(string name, string[] administratorGroups=null, string[] userGroups=null, string description=null);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Create(string,string[],string[],string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The Application name; it cannot be NULL, an empty string, or contain spaces.

<a name='Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Create(string,string[],string[],string).administratorGroups'></a>

`administratorGroups` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

The Application Administrators group name. It defaults to "BizTalk Server Administrators" ; [DefaultAdministratorGroups](AffiliateApplication.DefaultAdministratorGroups.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.DefaultAdministratorGroups').

<a name='Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Create(string,string[],string[],string).userGroups'></a>

`userGroups` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

The Application Users group name. It defaults to "BizTalk Application Users" and "BizTalk Isolated Host Users"; [DefaultUserGroups](AffiliateApplication.DefaultUserGroups.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.DefaultUserGroups').

<a name='Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Create(string,string[],string[],string).description'></a>

`description` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The Application description.

#### Returns
[AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')  
The <seealso cref="T:Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication"/> created in the Enterprise Single Sign-On (SSO) server database.

### Remarks
Application names are not case-sensitive, but case will be preserved.

### See Also
- [How to Create and Describe an Application to Single Sign-On](https://docs.microsoft.com/en-us/biztalk/core/how-to-create-and-describe-an-application-to-single-sign-on 'https://docs.microsoft.com/en-us/biztalk/core/how-to-create-and-describe-an-application-to-single-sign-on')
- [ISSOAdmin.CreateApplication Method](https://github.com/MicrosoftDocs/biztalk-docs/blob/master/technical-reference/issoadmin-createapplication-method.md 'https://github.com/MicrosoftDocs/biztalk-docs/blob/master/technical-reference/issoadmin-createapplication-method.md')