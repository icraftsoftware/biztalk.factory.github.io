#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings.Sso](Be.Stateless.BizTalk.Settings.Sso.md 'Be.Stateless.BizTalk.Settings.Sso').[ConfigStore](ConfigStore.md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore')

## ConfigStore.Save() Method

Saves the application settings, i.e the Enterprise Single Sign-On (SSO) Config Store.

```csharp
public void Save();
```

### Remarks
Save does not need to be thread-safe because only a process run by a BizTalk Administrator will be allowed to call
the [Save()](ConfigStore.Save().md 'Be.Stateless.BizTalk.Settings.Sso.ConfigStore.Save()') method, and this will/should occur at deployment time in a single process.