#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings.Sso](Be.Stateless.BizTalk.Settings.Sso.md 'Be.Stateless.BizTalk.Settings.Sso')

## AffiliateApplication Class

Manages the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')s in the Enterprise Single Sign-On (SSO) server database.

```csharp
public class AffiliateApplication
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; AffiliateApplication

| Fields | |
| :--- | :--- |
| [ANY_CONTACT_INFO](AffiliateApplication.ANY_CONTACT_INFO.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.ANY_CONTACT_INFO') | |

| Properties | |
| :--- | :--- |
| [AdministratorGroups](AffiliateApplication.AdministratorGroups.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.AdministratorGroups') | The application Administrators group name. |
| [ConfigStores](AffiliateApplication.ConfigStores.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.ConfigStores') | The application's [ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore')s. |
| [Contact](AffiliateApplication.Contact.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Contact') | The application contact information. |
| [DefaultAdministratorGroups](AffiliateApplication.DefaultAdministratorGroups.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.DefaultAdministratorGroups') | |
| [DefaultUserGroups](AffiliateApplication.DefaultUserGroups.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.DefaultUserGroups') | |
| [Description](AffiliateApplication.Description.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Description') | The application description. |
| [Name](AffiliateApplication.Name.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Name') | The application name. |
| [UserGroups](AffiliateApplication.UserGroups.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.UserGroups') | The application Users group name. |

| Methods | |
| :--- | :--- |
| [Create(string, string[], string[], string)](AffiliateApplication.Create(string,string[],string[],string).md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Create(string, string[], string[], string)') | Creates an [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') in the Enterprise Single Sign-On (SSO) server database. |
| [Delete()](AffiliateApplication.Delete().md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Delete()') | Deletes an [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') from the Enterprise Single Sign-On (SSO) server database. |
| [FindByContact(string)](AffiliateApplication.FindByContact(string).md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.FindByContact(string)') | Returns all the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')s which are associated to a given [contact](AffiliateApplication.FindByContact(string).md#Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.FindByContact(string).contact 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.FindByContact(string).contact') and that are currently deployed in the Enterprise Single Sign-On (SSO) server database. |
| [FindByName(string)](AffiliateApplication.FindByName(string).md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.FindByName(string)') | Finds and returns an [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') by name in the Enterprise Single Sign-On (SSO) server database. |
