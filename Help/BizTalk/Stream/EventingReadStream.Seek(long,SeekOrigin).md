#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[EventingReadStream](EventingReadStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream')

## EventingReadStream.Seek(long, SeekOrigin) Method

When overridden in a derived class, sets the position within the current stream.

```csharp
public override long Seek(long offset, System.IO.SeekOrigin origin);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.EventingReadStream.Seek(long,System.IO.SeekOrigin).offset'></a>

`offset` [System.Int64](https://docs.microsoft.com/en-us/dotnet/api/System.Int64 'System.Int64')

A byte offset relative to the [origin](EventingReadStream.Seek(long,SeekOrigin).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Seek(long,System.IO.SeekOrigin).origin 'Be.Stateless.BizTalk.Stream.EventingReadStream.Seek(long, System.IO.SeekOrigin).origin') parameter.

<a name='Be.Stateless.BizTalk.Stream.EventingReadStream.Seek(long,System.IO.SeekOrigin).origin'></a>

`origin` [System.IO.SeekOrigin](https://docs.microsoft.com/en-us/dotnet/api/System.IO.SeekOrigin 'System.IO.SeekOrigin')

A value of type [System.IO.SeekOrigin](https://docs.microsoft.com/en-us/dotnet/api/System.IO.SeekOrigin 'System.IO.SeekOrigin') indicating the reference point used to obtain the new position.

#### Returns
[System.Int64](https://docs.microsoft.com/en-us/dotnet/api/System.Int64 'System.Int64')  
The new position within the current stream.