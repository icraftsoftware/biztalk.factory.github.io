#### [Be.Stateless.BizTalk.Build.Tasks](README.md 'README')
### [Be.Stateless.BizTalk.Reflection.Extensions](Be.Stateless.BizTalk.Reflection.Extensions.md 'Be.Stateless.BizTalk.Reflection.Extensions').[BizTalkAssemblyExtensions](BizTalkAssemblyExtensions.md 'Be.Stateless.BizTalk.Reflection.Extensions.BizTalkAssemblyExtensions')

## BizTalkAssemblyExtensions.GetOrchestrationTypes(this Assembly) Method

Returns the BizTalk Server Orchestrations' types, i.e. types derived from [Microsoft.BizTalk.XLANGs.BTXEngine.BTXService](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.XLANGs.BTXEngine.BTXService 'Microsoft.BizTalk.XLANGs.BTXEngine.BTXService'), defined in the
[assembly](BizTalkAssemblyExtensions.GetOrchestrationTypes(thisAssembly).md#Be.Stateless.BizTalk.Reflection.Extensions.BizTalkAssemblyExtensions.GetOrchestrationTypes(thisSystem.Reflection.Assembly).assembly 'Be.Stateless.BizTalk.Reflection.Extensions.BizTalkAssemblyExtensions.GetOrchestrationTypes(this System.Reflection.Assembly).assembly').

```csharp
public static System.Type[] GetOrchestrationTypes(this System.Reflection.Assembly assembly);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Reflection.Extensions.BizTalkAssemblyExtensions.GetOrchestrationTypes(thisSystem.Reflection.Assembly).assembly'></a>

`assembly` [System.Reflection.Assembly](https://docs.microsoft.com/en-us/dotnet/api/System.Reflection.Assembly 'System.Reflection.Assembly')

The assembly to introspect for [Microsoft.BizTalk.XLANGs.BTXEngine.BTXService](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.XLANGs.BTXEngine.BTXService 'Microsoft.BizTalk.XLANGs.BTXEngine.BTXService')-derived types.

#### Returns
[System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')  
The [System.Array](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array') of [Microsoft.BizTalk.XLANGs.BTXEngine.BTXService](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.XLANGs.BTXEngine.BTXService 'Microsoft.BizTalk.XLANGs.BTXEngine.BTXService')-derived types defined in the [assembly](BizTalkAssemblyExtensions.GetOrchestrationTypes(thisAssembly).md#Be.Stateless.BizTalk.Reflection.Extensions.BizTalkAssemblyExtensions.GetOrchestrationTypes(thisSystem.Reflection.Assembly).assembly 'Be.Stateless.BizTalk.Reflection.Extensions.BizTalkAssemblyExtensions.GetOrchestrationTypes(this System.Reflection.Assembly).assembly').