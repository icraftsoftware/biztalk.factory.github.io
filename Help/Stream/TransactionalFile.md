#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO')

## TransactionalFile Class

Provides static methods for the creation of transactional [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') or [TransactionalFileStream](TransactionalFileStream.md 'Be.Stateless.IO.TransactionalFileStream')
objects.

```csharp
public static class TransactionalFile
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; TransactionalFile

### Remarks

Microsoft strongly recommends developers utilize alternative means to achieve your application's needs. Many scenarios
that TxF was developed for can be achieved through simpler and more readily available techniques. Furthermore, TxF may
not be available in future versions of Microsoft Windows. For more information, and alternatives to TxF, please see <a href="https://docs.microsoft.com/en-us/windows/win32/fileio/deprecation-of-txf">Alternatives to using
Transactional NTFS</a>.

[.NET Transactional File Manager](https://transactionalfilemgr.codeplex.com/ 'https://transactionalfilemgr.codeplex.com/').

| Methods | |
| :--- | :--- |
| [Create(string, int, IKernelTransaction)](TransactionalFile.Create(string,int,IKernelTransaction).md 'Be.Stateless.IO.TransactionalFile.Create(string, int, Be.Stateless.IO.IKernelTransaction)') | Creates a new file in the specified path. |
| [Move(string, string, IKernelTransaction)](TransactionalFile.Move(string,string,IKernelTransaction).md 'Be.Stateless.IO.TransactionalFile.Move(string, string, Be.Stateless.IO.IKernelTransaction)') | Moves an existing file or a directory, including its children, as a transacted operation. |
