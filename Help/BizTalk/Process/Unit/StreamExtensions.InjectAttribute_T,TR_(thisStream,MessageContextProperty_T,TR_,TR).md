#### [Be.Stateless.BizTalk.Process.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.IO.Extensions](Be.Stateless.BizTalk.Unit.IO.Extensions.md 'Be.Stateless.BizTalk.Unit.IO.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions')

## StreamExtensions.InjectAttribute<T,TR>(this Stream, MessageContextProperty<T,TR>, TR) Method

```csharp
public static System.IO.Stream InjectAttribute<T,TR>(this System.IO.Stream stream, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR> property, TR value)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T,TR_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).T'></a>

`T`

<a name='Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T,TR_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).TR'></a>

`TR`
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T,TR_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

<a name='Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T,TR_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[T](StreamExtensions.InjectAttribute_T,TR_(thisStream,MessageContextProperty_T,TR_,TR).md#Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T,TR_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).T 'Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute<T,TR>(this System.IO.Stream, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR).T')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[TR](StreamExtensions.InjectAttribute_T,TR_(thisStream,MessageContextProperty_T,TR_,TR).md#Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T,TR_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).TR 'Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute<T,TR>(this System.IO.Stream, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR).TR')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')

<a name='Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T,TR_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).value'></a>

`value` [TR](StreamExtensions.InjectAttribute_T,TR_(thisStream,MessageContextProperty_T,TR_,TR).md#Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute_T,TR_(thisSystem.IO.Stream,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).TR 'Be.Stateless.BizTalk.Unit.IO.Extensions.StreamExtensions.InjectAttribute<T,TR>(this System.IO.Stream, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR).TR')

#### Returns
[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')