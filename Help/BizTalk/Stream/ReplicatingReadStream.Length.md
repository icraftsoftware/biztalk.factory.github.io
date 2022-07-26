#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[ReplicatingReadStream](ReplicatingReadStream.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream')

## ReplicatingReadStream.Length Property

This property exposes the inner stream length in bytes.

```csharp
public override long Length { get; }
```

#### Property Value
[System.Int64](https://docs.microsoft.com/en-us/dotnet/api/System.Int64 'System.Int64')

#### Exceptions

[System.InvalidOperationException](https://docs.microsoft.com/en-us/dotnet/api/System.InvalidOperationException 'System.InvalidOperationException')  
The inner stream has not been read to its end yet.

### Remarks
[Length](ReplicatingReadStream.Length.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Length') property getter will throw unless the end of the inner stream has been reached.