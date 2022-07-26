#### [Be.Stateless.BizTalk.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Settings](Be.Stateless.BizTalk.Settings.md 'Be.Stateless.BizTalk.Settings').[SsoConfigurationReader](SsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader')

## SsoConfigurationReader.Instance Property

[SsoConfigurationReader](SsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader') singleton instance.

```csharp
public static Be.Stateless.BizTalk.Settings.ISsoConfigurationReader Instance { get; set; }
```

#### Property Value
[ISsoConfigurationReader](ISsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader')

### Remarks

Provides an internal property setter for the sake of mocking and unit testing.

Notice that to circumvent the internal visibility of the [Instance](SsoConfigurationReader.Instance.md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader.Instance') property setter for clients outside
of the realm of BizTalk.Factory, the `Be.Stateless.BizTalk.Unit` assembly, which is not GAC deployed, provides a
public setter for the [Instance](SsoConfigurationReader.Instance.md 'Be.Stateless.BizTalk.Settings.SsoConfigurationReader.Instance') property that allows clients of this library to safely inject an [ISsoConfigurationReader](ISsoConfigurationReader.md 'Be.Stateless.BizTalk.Settings.ISsoConfigurationReader') mock for the only sake of unit testing.