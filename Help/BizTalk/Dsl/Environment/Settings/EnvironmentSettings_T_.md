#### [Be.Stateless.BizTalk.Dsl.Environment.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings](Be.Stateless.BizTalk.Dsl.Environment.Settings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings')

## EnvironmentSettings<T> Class

Provides and enforces singleton instantiation and access to the [IEnvironmentSettings](IEnvironmentSettings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.IEnvironmentSettings')-derived classes
throughout an inheritance chain.

```csharp
public abstract class EnvironmentSettings<T> :
Be.Stateless.BizTalk.Dsl.Environment.Settings.IProvideSsoSettings
    where T : Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>, Be.Stateless.BizTalk.Dsl.Environment.Settings.IEnvironmentSettings, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings_T_.T'></a>

`T`

The [IEnvironmentSettings](IEnvironmentSettings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.IEnvironmentSettings')-derived class.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; EnvironmentSettings<T>

Implements [IProvideSsoSettings](IProvideSsoSettings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.IProvideSsoSettings')

### Remarks

[EnvironmentSettings&lt;T&gt;](EnvironmentSettings_T_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>') allows a class, [T](EnvironmentSettings_T_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings_T_.T 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>.T'), that directly derives from it to expose
            singleton semantics —i.e. regarding instantiation and access— while supporting environment setting overrides
            through inheritance.

Even though instantiation and access to environment setting overrides is offered by this class, the actual settings
class, [T](EnvironmentSettings_T_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings_T_.T 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>.T'), must allow for overrides via standard C# mechanisms, i.e. `abstract` or
`virtual` properties. [EnvironmentSettings&lt;T&gt;](EnvironmentSettings_T_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>') therefore is the base class for the first inheritance
level of an [IEnvironmentSettings](IEnvironmentSettings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.IEnvironmentSettings') inheritance chain. Further inheriting classes, i.e. environment setting
overrides, down the inheritance chain must consequently directly derive from the class they provide overrides for
—as one would typically do in C#— and not directly from this class.

| Constructors | |
| :--- | :--- |
| [EnvironmentSettings()](EnvironmentSettings_T_.EnvironmentSettings().md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>.EnvironmentSettings()') | Ensures singleton instantiation. |

| Properties | |
| :--- | :--- |
| [LazySingletonInstance](EnvironmentSettings_T_.LazySingletonInstance.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>.LazySingletonInstance') | |
| [Settings](EnvironmentSettings_T_.Settings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>.Settings') | Singleton instance. |
| [SingletonFactory](EnvironmentSettings_T_.SingletonFactory.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>.SingletonFactory') | |
| [SsoSettings](EnvironmentSettings_T_.SsoSettings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>.SsoSettings') | Dictionary of environment setting properties, together with their values, that must be deployed in an SSO affiliate application store in order to be available at runtime to the BizTalk application. |
