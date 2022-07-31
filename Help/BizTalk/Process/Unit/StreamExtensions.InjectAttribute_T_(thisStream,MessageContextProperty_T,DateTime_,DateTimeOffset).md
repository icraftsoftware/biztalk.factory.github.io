#### [Be.Stateless.BizTalk.Process.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.IO.Extensions](Be.Stateless.BizTalk.Unit.IO.Extensions.md 'Be.Stateless.BizTalk.Unit.IO.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions')

## StreamExtensions.InjectAttribute<T>(this Stream, MessageContextProperty<T,DateTime>, DateTimeOffset) Method

```csharp
public static System.IO.Stream InjectAttribute<T>(this System.IO.Stream stream, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,System.DateTime> property, System.DateTimeOffset value)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,System.DateTime_,System.DateTimeOffset).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,System.DateTime_,System.DateTimeOffset).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

<a name='Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,System.DateTime_,System.DateTimeOffset).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[T](StreamExtensions.InjectAttribute_T_(thisStream,MessageContextProperty_T,DateTime_,DateTimeOffset).md#Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,System.DateTime_,System.DateTimeOffset).T 'Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute<T>(this System.IO.Stream, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,System.DateTime>, System.DateTimeOffset).T')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[System.DateTime](https://docs.microsoft.com/en-us/dotnet/api/System.DateTime 'System.DateTime')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')

<a name='Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,System.DateTime_,System.DateTimeOffset).value'></a>

`value` [System.DateTimeOffset](https://docs.microsoft.com/en-us/dotnet/api/System.DateTimeOffset 'System.DateTimeOffset')

#### Returns
[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')