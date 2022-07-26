#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[ReplicatingReadStream](ReplicatingReadStream.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream')

## ReplicatingReadStream.SetLength(long) Method

When overridden in a derived class, sets the length of the current stream.

```csharp
public override void SetLength(long value);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.ReplicatingReadStream.SetLength(long).value'></a>

`value` [System.Int64](https://docs.microsoft.com/en-us/dotnet/api/System.Int64 'System.Int64')

The desired length of the current stream in bytes.

#### Exceptions

[System.NotSupportedException](https://docs.microsoft.com/en-us/dotnet/api/System.NotSupportedException 'System.NotSupportedException')  
The stream does not support both writing and seeking, such as if the stream is constructed from a pipe or console
output.