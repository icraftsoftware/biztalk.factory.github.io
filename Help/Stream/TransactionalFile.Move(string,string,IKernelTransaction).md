#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[TransactionalFile](TransactionalFile.md 'Be.Stateless.IO.TransactionalFile')

## TransactionalFile.Move(string, string, IKernelTransaction) Method

Moves an existing file or a directory, including its children, as a transacted operation.

```csharp
public static void Move(string sourceFilePath, string targetFilePath, Be.Stateless.IO.IKernelTransaction transaction);
```
#### Parameters

<a name='Be.Stateless.IO.TransactionalFile.Move(string,string,Be.Stateless.IO.IKernelTransaction).sourceFilePath'></a>

`sourceFilePath` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The current name of the existing file or directory on the local computer.

<a name='Be.Stateless.IO.TransactionalFile.Move(string,string,Be.Stateless.IO.IKernelTransaction).targetFilePath'></a>

`targetFilePath` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The new name for the file or directory. The new name must not already exist. A new file may be on a different
file system or drive. A new directory must be on the same drive.

<a name='Be.Stateless.IO.TransactionalFile.Move(string,string,Be.Stateless.IO.IKernelTransaction).transaction'></a>

`transaction` [IKernelTransaction](IKernelTransaction.md 'Be.Stateless.IO.IKernelTransaction')

A handle to the transaction.

### See Also
- [https://docs.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-movefiletransacteda](https://docs.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-movefiletransacteda 'https://docs.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-movefiletransacteda')