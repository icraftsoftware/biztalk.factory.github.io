#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[ReplicatingReadStream](ReplicatingReadStream.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream')

## ReplicatingReadStream(Stream, Stream) Constructor

Construct a [ReplicatingReadStream](ReplicatingReadStream.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream') instance.

```csharp
public ReplicatingReadStream(System.IO.Stream source, System.IO.Stream target);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.ReplicatingReadStream.ReplicatingReadStream(System.IO.Stream,System.IO.Stream).source'></a>

`source` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') to replicate to [target](ReplicatingReadStream.ReplicatingReadStream(Stream,Stream).md#Be.Stateless.BizTalk.Stream.ReplicatingReadStream.ReplicatingReadStream(System.IO.Stream,System.IO.Stream).target 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.ReplicatingReadStream(System.IO.Stream, System.IO.Stream).target') while being read.

<a name='Be.Stateless.BizTalk.Stream.ReplicatingReadStream.ReplicatingReadStream(System.IO.Stream,System.IO.Stream).target'></a>

`target` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') to replicate [source](ReplicatingReadStream.ReplicatingReadStream(Stream,Stream).md#Be.Stateless.BizTalk.Stream.ReplicatingReadStream.ReplicatingReadStream(System.IO.Stream,System.IO.Stream).source 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.ReplicatingReadStream(System.IO.Stream, System.IO.Stream).source') to while being read.