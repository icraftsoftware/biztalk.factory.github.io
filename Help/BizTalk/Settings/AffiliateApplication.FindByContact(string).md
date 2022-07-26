#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings.Sso](Be.Stateless.BizTalk.Settings.Sso.md 'Be.Stateless.BizTalk.Settings.Sso').[AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')

## AffiliateApplication.FindByContact(string) Method

Returns all the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')s which are associated to a given [contact](AffiliateApplication.FindByContact(string).md#Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.FindByContact(string).contact 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.FindByContact(string).contact') and
that are currently deployed in the Enterprise Single Sign-On (SSO) server database.

```csharp
public static System.Collections.Generic.IEnumerable<Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication> FindByContact(string contact="icraftsoftware@stateless.be");
```
#### Parameters

<a name='Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.FindByContact(string).contact'></a>

`contact` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

Name of the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')s' contact that will be used as filter. It defaults to [Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.DEFAULT_CONTACT_INFO](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.DEFAULT_CONTACT_INFO 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.DEFAULT_CONTACT_INFO').

#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
The [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')s currently deployed in the Enterprise Single Sign-On (SSO) server database.

### Remarks
By default, only the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')s that have been associated to [Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.DEFAULT_CONTACT_INFO](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.DEFAULT_CONTACT_INFO 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.DEFAULT_CONTACT_INFO') will be retrieved. If [contact](AffiliateApplication.FindByContact(string).md#Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.FindByContact(string).contact 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.FindByContact(string).contact') is [ANY_CONTACT_INFO](AffiliateApplication.ANY_CONTACT_INFO.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.ANY_CONTACT_INFO') all
the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')s will be returned, regardless of whether they have been created by
BizTalk.Factory's [AffiliateApplication.Create](AffiliateApplication.Create(string,string[],string[],string).md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Create(string, string[], string[], string)') factory method; that is to say, regardless of
their [Contact](AffiliateApplication.Contact.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.Contact').