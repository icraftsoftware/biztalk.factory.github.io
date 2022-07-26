#### [Be.Stateless.Stream.Unit](README.md 'README')
### [Be.Stateless.Unit.Resources](Be.Stateless.Unit.Resources.md 'Be.Stateless.Unit.Resources').[ResourceManagerFactory](ResourceManagerFactory.md 'Be.Stateless.Unit.Resources.ResourceManagerFactory')

## ResourceManagerFactory.Create<T>() Method

Instantiate an [IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager') providing access to the resources embedded in the assembly to which
belongs [T](ResourceManagerFactory.Create_T_().md#Be.Stateless.Unit.Resources.ResourceManagerFactory.Create_T_().T 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create<T>().T'), and scoped by the namespace of the specified type [T](ResourceManagerFactory.Create_T_().md#Be.Stateless.Unit.Resources.ResourceManagerFactory.Create_T_().T 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create<T>().T').

```csharp
public static Be.Stateless.Unit.Resources.IResourceManager Create<T>();
```
#### Type parameters

<a name='Be.Stateless.Unit.Resources.ResourceManagerFactory.Create_T_().T'></a>

`T`

The type whose namespace scope is to be used to access the embedded resources in its containing assembly.

#### Returns
[IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager')  
An [IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager') that provides access to the resources scoped by the namespace of the specified type
[T](ResourceManagerFactory.Create_T_().md#Be.Stateless.Unit.Resources.ResourceManagerFactory.Create_T_().T 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create<T>().T') and embedded in the containing assembly of [T](ResourceManagerFactory.Create_T_().md#Be.Stateless.Unit.Resources.ResourceManagerFactory.Create_T_().T 'Be.Stateless.Unit.Resources.ResourceManagerFactory.Create<T>().T').