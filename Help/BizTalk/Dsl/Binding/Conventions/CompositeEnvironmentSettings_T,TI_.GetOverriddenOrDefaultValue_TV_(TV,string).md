#### [Be.Stateless.BizTalk.Dsl.Binding.Conventions](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention](Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention').[CompositeEnvironmentSettings&lt;T,TI&gt;](CompositeEnvironmentSettings_T,TI_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>')

## CompositeEnvironmentSettings<T,TI>.GetOverriddenOrDefaultValue<TV>(TV, string) Method

Returns either the default or overridden value for a given settings property named [propertyName](CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).propertyName 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.GetOverriddenOrDefaultValue<TV>(TV, string).propertyName').

```csharp
protected TV GetOverriddenOrDefaultValue<TV>(TV value, string propertyName=null);
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).TV'></a>

`TV`

The [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') of the property [propertyName](CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).propertyName 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.GetOverriddenOrDefaultValue<TV>(TV, string).propertyName').
#### Parameters

<a name='Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).value'></a>

`value` [TV](CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).TV 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.GetOverriddenOrDefaultValue<TV>(TV, string).TV')

The default value of the property [propertyName](CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).propertyName 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.GetOverriddenOrDefaultValue<TV>(TV, string).propertyName').

<a name='Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).propertyName'></a>

`propertyName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the property.

#### Returns
[TV](CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).TV 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.GetOverriddenOrDefaultValue<TV>(TV, string).TV')  
The value of the property to be used.

### Remarks

This method returns either the value provided by the [TI](CompositeEnvironmentSettings_T,TI_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.TI 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.TI')-derived setting overrides instance if
this instance was declared via [DeploymentContext.EnvironmentSettingOverridesType](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType 'Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType') or
the default [value](CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.GetOverriddenOrDefaultValue_TV_(TV,string).value 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.GetOverriddenOrDefaultValue<TV>(TV, string).value') if it was not, i.e. the value provided by [T](CompositeEnvironmentSettings_T,TI_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.T 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.T').

The [CompositeEnvironmentSettings&lt;T,TI&gt;](CompositeEnvironmentSettings_T,TI_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>')-derived [T](CompositeEnvironmentSettings_T,TI_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings_T,TI_.T 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>.T') class must call this method
should it be willing to allow for a setting property to be overridden. Failure to do so will prevent the property to
be overridden at deployment time.