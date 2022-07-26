#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings.Sso](Be.Stateless.BizTalk.Settings.Sso.md 'Be.Stateless.BizTalk.Settings.Sso')

## ConfigStore Class

```csharp
public sealed class ConfigStore
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ConfigStore

| Properties | |
| :--- | :--- |
| [Age](ConfigStore.Age.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore.Age') | Elapsed time since the application settings were last refreshed or, more generally, synchronized with the Enterprise Single Sign-On (SSO) Config Store. |
| [Identifier](ConfigStore.Identifier.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore.Identifier') | |
| [Properties](ConfigStore.Properties.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore.Properties') | |

| Methods | |
| :--- | :--- |
| [AgedLessThan(TimeSpan)](ConfigStore.AgedLessThan(TimeSpan).md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore.AgedLessThan(System.TimeSpan)') | |
| [Delete()](ConfigStore.Delete().md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore.Delete()') | Deletes the application settings, i.e the Enterprise Single Sign-On (SSO) Config Store. |
| [Reload()](ConfigStore.Reload().md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore.Reload()') | Reloads the Config Store with fresh values from the Enterprise Single Sign-On (SSO). |
| [Save()](ConfigStore.Save().md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore.Save()') | Saves the application settings, i.e the Enterprise Single Sign-On (SSO) Config Store. |
