#### [Be.Stateless.BizTalk.Dsl.Binding.Conventions](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention](Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention')

## CompositeEnvironmentSettings<T,TI> Class

Provides and enforces singleton instantiation and access to an [Be.Stateless.BizTalk.Dsl.Environment.Settings.IEnvironmentSettings](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Environment.Settings.IEnvironmentSettings 'Be.Stateless.BizTalk.Dsl.Environment.Settings.IEnvironmentSettings')-derived class and
allows for settings to be overridden by [TI](CompositeEnvironmentSettings_T,TI_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.TI 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.TI') through composition and delegation instead of
inheritance as it is the case when directly deriving from [Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings-1 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings`1').

```csharp
public abstract class CompositeEnvironmentSettings<T,TI> : Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>
    where T : Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T, TI>, TI, Be.Stateless.BizTalk.Dsl.Environment.Settings.IEnvironmentSettings, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.T'></a>

`T`

The type of the [CompositeEnvironmentSettings&lt;T,TI&gt;](CompositeEnvironmentSettings_T,TI_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>')-derived class that provides default settings value.

<a name='Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.TI'></a>

`TI`

The [TI](CompositeEnvironmentSettings_T,TI_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.TI 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.TI')-derived class that provides setting override values. As [T](CompositeEnvironmentSettings_T,TI_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.T 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.T') must
support it too, [TI](CompositeEnvironmentSettings_T,TI_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.TI 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.TI') must be an interface which acts as an extension point for setting overrides.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings-1 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings`1')[T](CompositeEnvironmentSettings_T,TI_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.T 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings-1 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings`1') &#129106; CompositeEnvironmentSettings<T,TI>

Derived  
&#8627; [Platform](Platform.md 'Be.Stateless.BizTalk.Factory.Platform')

### See Also
- [Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings-1 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings`1')

| Properties | |
| :--- | :--- |
| [EnvironmentSettingOverrides](CompositeEnvironmentSettings_T,TI_.EnvironmentSettingOverrides.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.EnvironmentSettingOverrides') | |
| [Settings](CompositeEnvironmentSettings_T,TI_.Settings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.Settings') | Singleton instance. |

| Methods | |
| :--- | :--- |
| [GetOverriddenOrDefaultValue&lt;TV&gt;(TV, string)](CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.GetOverriddenOrDefaultValue<TV>(TV, string)') | Returns either the default or overridden value for a given settings property named [propertyName](CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).propertyName 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.GetOverriddenOrDefaultValue<TV>(TV, string).propertyName'). |
