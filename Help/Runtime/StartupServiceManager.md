#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime](Be.Stateless.Runtime.md 'Be.Stateless.Runtime')

## StartupServiceManager Class

This class participates in the creation of new application domains in a process in order to allow any custom
infrastructure code to be executed before other managed code runs.

```csharp
public class StartupServiceManager : System.AppDomainManager
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.AppDomainManager](https://docs.microsoft.com/en-us/dotnet/api/System.AppDomainManager 'System.AppDomainManager') &#129106; StartupServiceManager

### See Also
- [AppDomainManager Class](https://docs.microsoft.com/en-us/dotnet/api/system.appdomainmanager 'https://docs.microsoft.com/en-us/dotnet/api/system.appdomainmanager')
- [appDomainManagerAssembly Element](https://docs.microsoft.com/en-us/dotnet/framework/configure-apps/file-schema/runtime/appdomainmanagerassembly-element 'https://docs.microsoft.com/en-us/dotnet/framework/configure-apps/file-schema/runtime/appdomainmanagerassembly-element')

| Methods | |
| :--- | :--- |
| [InitializeNewDomain(AppDomainSetup)](StartupServiceManager.InitializeNewDomain(AppDomainSetup).md 'Be.Stateless.Runtime.StartupServiceManager.InitializeNewDomain(System.AppDomainSetup)') | |
