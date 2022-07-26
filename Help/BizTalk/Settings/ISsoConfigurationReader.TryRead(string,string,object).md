#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings](Be.Stateless.BizTalk.Settings.md 'Be.Stateless.BizTalk.Settings').[ISsoConfigurationReader](ISsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader')

## ISsoConfigurationReader.TryRead(string, string, object) Method

Try to read the value of the individual configuration property [configPropertyName](ISsoConfigurationReader.TryRead(string,string,object).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string,string,object).configPropertyName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string, string, object).configPropertyName') for the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')[affiliateApplicationName](ISsoConfigurationReader.TryRead(string,string,object).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string,string,object).affiliateApplicationName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string, string, object).affiliateApplicationName') from its default [ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore').

```csharp
bool TryRead(string affiliateApplicationName, string configPropertyName, out object value);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string,string,object).affiliateApplicationName'></a>

`affiliateApplicationName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') for which to read the value of the [configPropertyName](ISsoConfigurationReader.TryRead(string,string,object).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string,string,object).configPropertyName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string, string, object).configPropertyName') configuration property from its default [ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore').

<a name='Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string,string,object).configPropertyName'></a>

`configPropertyName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the configuration property whose value is to be read.

<a name='Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string,string,object).value'></a>

`value` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')

The value of the configuration property; it can be `null`.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the property [configPropertyName](ISsoConfigurationReader.TryRead(string,string,object).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string,string,object).configPropertyName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string, string, object).configPropertyName') was defined in the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')[affiliateApplicationName](ISsoConfigurationReader.TryRead(string,string,object).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string,string,object).affiliateApplicationName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.TryRead(string, string, object).affiliateApplicationName') from its default [ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore');
            `false` otherwise.