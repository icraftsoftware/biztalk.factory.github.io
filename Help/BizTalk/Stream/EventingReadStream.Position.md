#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[EventingReadStream](EventingReadStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream')

## EventingReadStream.Position Property

When overridden in a derived class, gets or sets the position within the current stream.

```csharp
public override long Position { get; set; }
```

#### Property Value
[System.Int64](https://docs.microsoft.com/en-us/dotnet/api/System.Int64 'System.Int64')

#### Exceptions

[System.NotSupportedException](https://docs.microsoft.com/en-us/dotnet/api/System.NotSupportedException 'System.NotSupportedException')  
The stream does not support seeking.