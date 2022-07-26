#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings](Be.Stateless.BizTalk.Settings.md 'Be.Stateless.BizTalk.Settings')

## ISsoConfigurationReader Interface

Client interface to read individual configuration properties from an [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')'s default [ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore') stored by the Enterprise Single Sign-On (SSO) server database.

```csharp
public interface ISsoConfigurationReader
```

Derived  
&#8627; [SsoConfigurationReader](SsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader')

### Remarks
This interface essentially exists to provide the ability to inject an [ISsoConfigurationReader](ISsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader') mock for the
sake of unit testing; see [SsoConfigurationReader.Instance](SsoConfigurationReader.Instance.md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader.Instance').

### See Also
- [AffiliateApplication.ConfigStores](AffiliateApplication.ConfigStores.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.ConfigStores')
- [ConfigStoreCollection.Default](ConfigStoreCollection.Default.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStoreCollection.Default')
- [SsoConfigurationReader.Instance](SsoConfigurationReader.Instance.md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader.Instance')

| Methods | |
| :--- | :--- |
| [Read(string, string)](ISsoConfigurationReader.Read(string,string).md 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string, string)') | Read the value of the individual configuration property [configPropertyName](ISsoConfigurationReader.Read(string,string).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string,string).configPropertyName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string, string).configPropertyName') for the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')[affiliateApplicationName](ISsoConfigurationReader.Read(string,string).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string,string).affiliateApplicationName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string, string).affiliateApplicationName') from its default [ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore'). |
| [TryRead(string, string, object)](ISsoConfigurationReader.TryRead(string,string,object).md 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string, string, object)') | Try to read the value of the individual configuration property [configPropertyName](ISsoConfigurationReader.TryRead(string,string,object).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string,string,object).configPropertyName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string, string, object).configPropertyName') for the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')[affiliateApplicationName](ISsoConfigurationReader.TryRead(string,string,object).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string,string,object).affiliateApplicationName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string, string, object).affiliateApplicationName') from its default [ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore'). |
