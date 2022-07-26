#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Configuration](Be.Stateless.Runtime.Configuration.md 'Be.Stateless.Runtime.Configuration').[StartupServiceConfigurationElementCollection](StartupServiceConfigurationElementCollection.md 'Be.Stateless.Runtime.Configuration.StartupServiceConfigurationElementCollection')

## StartupServiceConfigurationElementCollection.GetElementKey(ConfigurationElement) Method

Gets the element key for a specified configuration element when overridden in a derived class.

```csharp
protected override object GetElementKey(System.Configuration.ConfigurationElement element);
```
#### Parameters

<a name='Be.Stateless.Runtime.Configuration.StartupServiceConfigurationElementCollection.GetElementKey(System.Configuration.ConfigurationElement).element'></a>

`element` [System.Configuration.ConfigurationElement](https://docs.microsoft.com/en-us/dotnet/api/System.Configuration.ConfigurationElement 'System.Configuration.ConfigurationElement')

The [System.Configuration.ConfigurationElement](https://docs.microsoft.com/en-us/dotnet/api/System.Configuration.ConfigurationElement 'System.Configuration.ConfigurationElement')-derived [StartupServiceConfigurationElement](StartupServiceConfigurationElement.md 'Be.Stateless.Runtime.Configuration.StartupServiceConfigurationElement') to return the key for.

#### Returns
[System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')