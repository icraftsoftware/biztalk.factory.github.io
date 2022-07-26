#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.Resources](Be.Stateless.Resources.md 'Be.Stateless.Resources').[ResourceManager](ResourceManager.md 'Be.Stateless.Resources.ResourceManager')

## ResourceManager.Load<T>(Assembly, string, Func<Stream,T>) Method

```csharp
public static T Load<T>(System.Reflection.Assembly assembly, string name, System.Func<System.IO.Stream,T> deserializer);
```
#### Type parameters

<a name='Be.Stateless.Resources.ResourceManager.Load_T_(System.Reflection.Assembly,string,System.Func_System.IO.Stream,T_).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.Resources.ResourceManager.Load_T_(System.Reflection.Assembly,string,System.Func_System.IO.Stream,T_).assembly'></a>

`assembly` [System.Reflection.Assembly](https://docs.microsoft.com/en-us/dotnet/api/System.Reflection.Assembly 'System.Reflection.Assembly')

<a name='Be.Stateless.Resources.ResourceManager.Load_T_(System.Reflection.Assembly,string,System.Func_System.IO.Stream,T_).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

<a name='Be.Stateless.Resources.ResourceManager.Load_T_(System.Reflection.Assembly,string,System.Func_System.IO.Stream,T_).deserializer'></a>

`deserializer` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[T](ResourceManager.Load_T_(Assembly,string,Func_Stream,T_).md#Be.Stateless.Resources.ResourceManager.Load_T_(System.Reflection.Assembly,string,System.Func_System.IO.Stream,T_).T 'Be.Stateless.Resources.ResourceManager.Load<T>(System.Reflection.Assembly, string, System.Func<System.IO.Stream,T>).T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

#### Returns
[T](ResourceManager.Load_T_(Assembly,string,Func_Stream,T_).md#Be.Stateless.Resources.ResourceManager.Load_T_(System.Reflection.Assembly,string,System.Func_System.IO.Stream,T_).T 'Be.Stateless.Resources.ResourceManager.Load<T>(System.Reflection.Assembly, string, System.Func<System.IO.Stream,T>).T')