#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[TransactionalFile](TransactionalFile.md 'Be.Stateless.IO.TransactionalFile')

## TransactionalFile.Create(string, int, IKernelTransaction) Method

Creates a new file in the specified path.

```csharp
public static System.IO.FileStream Create(string path, int bufferSize=4096, Be.Stateless.IO.IKernelTransaction transaction=null);
```
#### Parameters

<a name='Be.Stateless.IO.TransactionalFile.Create(string,int,Be.Stateless.IO.IKernelTransaction).path'></a>

`path` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The path and name of the file to create.

<a name='Be.Stateless.IO.TransactionalFile.Create(string,int,Be.Stateless.IO.IKernelTransaction).bufferSize'></a>

`bufferSize` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The number of bytes buffered for writes to the file. It defaults to 4KB.

<a name='Be.Stateless.IO.TransactionalFile.Create(string,int,Be.Stateless.IO.IKernelTransaction).transaction'></a>

`transaction` [IKernelTransaction](IKernelTransaction.md 'Be.Stateless.IO.IKernelTransaction')

An [IKernelTransaction](IKernelTransaction.md 'Be.Stateless.IO.IKernelTransaction') transaction that is already enlisted with a DTC, or `null` otherwise. It
defaults to `null`.

#### Returns
[System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream')  
A [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') or [TransactionalFileStream](TransactionalFileStream.md 'Be.Stateless.IO.TransactionalFileStream'), depending on whether the transaction has to be
explicitly (i.e. not DTC enlisted) managed or not, with the specified buffer size that provides write access to the
file specified in path.

### Remarks

Notice that a [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') can only be transactional if both the file system supports transaction —
[OperatingSystemExtensions.SupportTransactionalFileSystem](OperatingSystemExtensions.SupportTransactionalFileSystem(thisOperatingSystem).md 'Be.Stateless.Extensions.OperatingSystemExtensions.SupportTransactionalFileSystem(this System.OperatingSystem)')
— and the file is not created in a network volume — [Path.IsNetworkPath](Path.IsNetworkPath(string).md 'Be.Stateless.IO.Path.IsNetworkPath(string)'). For these reasons, the [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') created may not
be transactional at all if one of these transactional requirements is not met.

If both transactional requirements are met and a `null`[transaction](TransactionalFile.Create(string,int,IKernelTransaction).md#Be.Stateless.IO.TransactionalFile.Create(string,int,Be.Stateless.IO.IKernelTransaction).transaction 'Be.Stateless.IO.TransactionalFile.Create(string, int, Be.Stateless.IO.IKernelTransaction).transaction') has been passed, the
stream created will be a [TransactionalFileStream](TransactionalFileStream.md 'Be.Stateless.IO.TransactionalFileStream') instance. In this case, the client will be in charge
of <i>explicitly</i> managing the transaction outcome, that is either [Commit()](TransactionalFileStream.Commit().md 'Be.Stateless.IO.TransactionalFileStream.Commit()') or
[Rollback()](TransactionalFileStream.Rollback().md 'Be.Stateless.IO.TransactionalFileStream.Rollback()').

If both transactional requirements are met and a non `null`[transaction](TransactionalFile.Create(string,int,IKernelTransaction).md#Be.Stateless.IO.TransactionalFile.Create(string,int,Be.Stateless.IO.IKernelTransaction).transaction 'Be.Stateless.IO.TransactionalFile.Create(string, int, Be.Stateless.IO.IKernelTransaction).transaction') has been passed, the
stream created will be a regular [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') instance. However it will have been created in such a way
that the [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') piggybacks the [transaction](TransactionalFile.Create(string,int,IKernelTransaction).md#Be.Stateless.IO.TransactionalFile.Create(string,int,Be.Stateless.IO.IKernelTransaction).transaction 'Be.Stateless.IO.TransactionalFile.Create(string, int, Be.Stateless.IO.IKernelTransaction).transaction') already enlisted with a DTC. <b>It is
therefore the responsibility of the client to ensure that the non <c>null</c><paramref name="transaction"/> is
indeed correctly enlisted with a DTC; the client would have no way to determine the outcome of the transaction
otherwise.</b>

If not both transactional requirements are met, and irrelevantly of the passed [transaction](TransactionalFile.Create(string,int,IKernelTransaction).md#Be.Stateless.IO.TransactionalFile.Create(string,int,Be.Stateless.IO.IKernelTransaction).transaction 'Be.Stateless.IO.TransactionalFile.Create(string, int, Be.Stateless.IO.IKernelTransaction).transaction'), the
stream created will always be a regular [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') instance with no underlying transaction. The client
has therefore no way of distinguishing a transactional [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') enlisted with a DTC from non
transactional one.

### See Also
- [OperatingSystemExtensions](OperatingSystemExtensions.md 'Be.Stateless.Extensions.OperatingSystemExtensions')
- [SupportTransactionalFileSystem(this OperatingSystem)](OperatingSystemExtensions.SupportTransactionalFileSystem(thisOperatingSystem).md 'Be.Stateless.Extensions.OperatingSystemExtensions.SupportTransactionalFileSystem(this System.OperatingSystem)')