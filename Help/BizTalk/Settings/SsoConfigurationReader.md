#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings](Be.Stateless.BizTalk.Settings.md 'Be.Stateless.BizTalk.Settings')

## SsoConfigurationReader Class

[ISsoConfigurationReader](ISsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader') implementation that guarantees fresh readings, or not older than 60 seconds, from
            the default [ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore') of a given [AffiliateApplication](AffiliateApplication.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication').

```csharp
public class SsoConfigurationReader :
Be.Stateless.BizTalk.Settings.ISsoConfigurationReader
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; SsoConfigurationReader

Implements [ISsoConfigurationReader](ISsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader')

### See Also
- [ConfigStores](AffiliateApplication.ConfigStores.md 'Be.Stateless.BizTalk.Settings.Sso.AffiliateApplication.ConfigStores')
- [ConfigStores.Default](ConfigStoreCollection.Default.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStoreCollection.Default')

| Properties | |
| :--- | :--- |
| [Instance](SsoConfigurationReader.Instance.md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader.Instance') | [SsoConfigurationReader](SsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader') singleton instance. |

| Methods | |
| :--- | :--- |
| [Read(string, string)](SsoConfigurationReader.Read(string,string).md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader.Read(string, string)') | |
| [TryRead(string, string, object)](SsoConfigurationReader.TryRead(string,string,object).md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader.TryRead(string, string, object)') | |
