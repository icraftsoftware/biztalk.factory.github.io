#### [Be.Stateless.Stream.Unit](README.md 'README')
### [Be.Stateless.Unit.Resources](Be.Stateless.Unit.Resources.md 'Be.Stateless.Unit.Resources').[IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager')

## IResourceManager.Load<T>(string, Func<Stream,T>) Method

Loads and deserializes a resource embedded in the calling assembly.

```csharp
T Load<T>(string name, System.Func<System.IO.Stream,T> deserializer);
```
#### Type parameters

<a name='Be.Stateless.Unit.Resources.IResourceManager.Load_T_(string,System.Func_System.IO.Stream,T_).T'></a>

`T`

The type of the deserialized resource.
#### Parameters

<a name='Be.Stateless.Unit.Resources.IResourceManager.Load_T_(string,System.Func_System.IO.Stream,T_).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the resource.

<a name='Be.Stateless.Unit.Resources.IResourceManager.Load_T_(string,System.Func_System.IO.Stream,T_).deserializer'></a>

`deserializer` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[T](IResourceManager.Load_T_(string,Func_Stream,T_).md#Be.Stateless.Unit.Resources.IResourceManager.Load_T_(string,System.Func_System.IO.Stream,T_).T 'Be.Stateless.Unit.Resources.IResourceManager.Load<T>(string, System.Func<System.IO.Stream,T>).T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

A delegate to a method that can deserialize the resource from its stream.

#### Returns
[T](IResourceManager.Load_T_(string,Func_Stream,T_).md#Be.Stateless.Unit.Resources.IResourceManager.Load_T_(string,System.Func_System.IO.Stream,T_).T 'Be.Stateless.Unit.Resources.IResourceManager.Load<T>(string, System.Func<System.IO.Stream,T>).T')  
The deserialized resource.