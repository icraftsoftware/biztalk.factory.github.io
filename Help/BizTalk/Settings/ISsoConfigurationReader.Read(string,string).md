#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings](Be.Stateless.BizTalk.Settings.md 'Be.Stateless.BizTalk.Settings').[ISsoConfigurationReader](ISsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader')

## ISsoConfigurationReader.Read(string, string) Method

Read the value of the individual configuration property [configPropertyName](ISsoConfigurationReader.Read(string,string).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string,string).configPropertyName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string, string).configPropertyName') for the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication')[affiliateApplicationName](ISsoConfigurationReader.Read(string,string).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string,string).affiliateApplicationName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string, string).affiliateApplicationName') from its default [ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore').

```csharp
object Read(string affiliateApplicationName, string configPropertyName);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string,string).affiliateApplicationName'></a>

`affiliateApplicationName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') for which to return the value of the [configPropertyName](ISsoConfigurationReader.Read(string,string).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string,string).configPropertyName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string, string).configPropertyName') configuration property from its default [ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore').

<a name='Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string,string).configPropertyName'></a>

`configPropertyName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the configuration property to return the value of.

#### Returns
[System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')  
The value of the configuration property.

#### Exceptions

[System.ArgumentException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentException 'System.ArgumentException')  
The configuration property has not been defined for the [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication') named [affiliateApplicationName](ISsoConfigurationReader.Read(string,string).md#Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string,string).affiliateApplicationName 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader.Read(string, string).affiliateApplicationName') or does not provide a non `null` value.