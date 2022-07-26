#### [Be.Stateless.Stream.Unit](README.md 'README')
### [Be.Stateless.Unit.Resources](Be.Stateless.Unit.Resources.md 'Be.Stateless.Unit.Resources')

## ResourceManagerFactory Class

```csharp
public static class ResourceManagerFactory
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ResourceManagerFactory

| Methods | |
| :--- | :--- |
| [Create(Assembly)](ResourceManagerFactory.Create(Assembly).md 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create(System.Reflection.Assembly)') | Instantiate an [IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager') providing access to the resources embedded in [assembly](ResourceManagerFactory.Create(Assembly).md#Be.Stateless.Unit.Resources.ResourceManagerFactory.Create(System.Reflection.Assembly).assembly 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create(System.Reflection.Assembly).assembly'). |
| [Create&lt;T&gt;()](ResourceManagerFactory.Create_T_().md 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create<T>()') | Instantiate an [IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager') providing access to the resources embedded in the assembly to which belongs [T](ResourceManagerFactory.Create_T_().md#Be.Stateless.Unit.Resources.ResourceManagerFactory.Create_T_().T 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create<T>().T'), and scoped by the namespace of the specified type [T](ResourceManagerFactory.Create_T_().md#Be.Stateless.Unit.Resources.ResourceManagerFactory.Create_T_().T 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create<T>().T'). |
