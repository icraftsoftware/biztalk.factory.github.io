#### [Be.Stateless.Stream.Unit](README.md 'README')
### [Be.Stateless.Unit.Resources](Be.Stateless.Unit.Resources.md 'Be.Stateless.Unit.Resources').[ResourceManagerFactory](ResourceManagerFactory.md 'Be.Stateless.Unit.Resources.ResourceManagerFactory')

## ResourceManagerFactory.Create(Assembly) Method

Instantiate an [IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager') providing access to the resources embedded in [assembly](ResourceManagerFactory.Create(Assembly).md#Be.Stateless.Unit.Resources.ResourceManagerFactory.Create(System.Reflection.Assembly).assembly 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create(System.Reflection.Assembly).assembly').

```csharp
public static Be.Stateless.Unit.Resources.IResourceManager Create(System.Reflection.Assembly assembly);
```
#### Parameters

<a name='Be.Stateless.Unit.Resources.ResourceManagerFactory.Create(System.Reflection.Assembly).assembly'></a>

`assembly` [System.Reflection.Assembly](https://docs.microsoft.com/en-us/dotnet/api/System.Reflection.Assembly 'System.Reflection.Assembly')

The assembly whose embedded resources need to be accessed

#### Returns
[IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager')  
An [IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager') that provide access to the resources embedded in [assembly](ResourceManagerFactory.Create(Assembly).md#Be.Stateless.Unit.Resources.ResourceManagerFactory.Create(System.Reflection.Assembly).assembly 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create(System.Reflection.Assembly).assembly').