#### [Be.Stateless.BizTalk.Dsl.Environment.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings](Be.Stateless.BizTalk.Dsl.Environment.Settings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings')

## SsoSettingAttribute Class

Attribute identifying individual [EnvironmentSettings&lt;T&gt;](EnvironmentSettings_T_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>') properties that need to be deployed in an SSO
affiliate application store in order to be available at runtime to the BizTalk application.

```csharp
public sealed class SsoSettingAttribute : System.Attribute
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Attribute](https://docs.microsoft.com/en-us/dotnet/api/System.Attribute 'System.Attribute') &#129106; SsoSettingAttribute

### Remarks
This attribute is meant to be used to qualify individual application setting properties that one developer typically
writes in order to generate application bindings.

### See Also
- [EnvironmentSettings&lt;T&gt;](EnvironmentSettings_T_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>')