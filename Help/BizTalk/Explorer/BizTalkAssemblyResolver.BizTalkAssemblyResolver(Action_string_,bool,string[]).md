#### [Be.Stateless.BizTalk.Explorer](README.md 'README')
### [Be.Stateless.BizTalk.Reflection](Be.Stateless.BizTalk.Reflection.md 'Be.Stateless.BizTalk.Reflection').[BizTalkAssemblyResolver](BizTalkAssemblyResolver.md 'Be.Stateless.BizTalk.Reflection.BizTalkAssemblyResolver')

## BizTalkAssemblyResolver(Action<string>, bool, string[]) Constructor

```csharp
public BizTalkAssemblyResolver(System.Action<string> logAppender, bool skipResourceAssemblies, params string[] probingFolderPaths);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Reflection.BizTalkAssemblyResolver.BizTalkAssemblyResolver(System.Action_string_,bool,string[]).logAppender'></a>

`logAppender` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')

<a name='Be.Stateless.BizTalk.Reflection.BizTalkAssemblyResolver.BizTalkAssemblyResolver(System.Action_string_,bool,string[]).skipResourceAssemblies'></a>

`skipResourceAssemblies` [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

Whether to skip resolution for resource assemblies.

<a name='Be.Stateless.BizTalk.Reflection.BizTalkAssemblyResolver.BizTalkAssemblyResolver(System.Action_string_,bool,string[]).probingFolderPaths'></a>

`probingFolderPaths` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

### Remarks

Beginning with the .NET Framework 4, the [System.ResolveEventHandler](https://docs.microsoft.com/en-us/dotnet/api/System.ResolveEventHandler 'System.ResolveEventHandler') event is raised for all assemblies,
including resource assemblies. In earlier versions, the event was not raised for resource assemblies. If the
operating system is localized, the handler might be called multiple times: once for each culture in the fallback
chain.

### See Also
- [AppDomain.AssemblyResolve Event](https://docs.microsoft.com/en-us/dotnet/api/system.appdomain.assemblyresolve 'https://docs.microsoft.com/en-us/dotnet/api/system.appdomain.assemblyresolve')