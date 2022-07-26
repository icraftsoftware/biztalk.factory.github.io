#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO')

## TransactionalFileStream Class

[System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') subclass to be used when the underlying stream is transacted and its scoping transaction
            requires and explicit commit because it is not DTC enlisted.

```csharp
public class TransactionalFileStream : System.IO.FileStream,
Be.Stateless.IO.ITransactionalStream
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') &#129106; [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') &#129106; TransactionalFileStream

Implements [ITransactionalStream](ITransactionalStream.md 'Be.Stateless.IO.ITransactionalStream')

| Methods | |
| :--- | :--- |
| [Commit()](TransactionalFileStream.Commit().md 'Be.Stateless.IO.TransactionalFileStream.Commit()') | |
| [Dispose(bool)](TransactionalFileStream.Dispose(bool).md 'Be.Stateless.IO.TransactionalFileStream.Dispose(bool)') | Note that because the base class does mix the Close() and Dispose() operations, one can commit the transaction if properly closed, and rollback it if disposed... |
| [Rollback()](TransactionalFileStream.Rollback().md 'Be.Stateless.IO.TransactionalFileStream.Rollback()') | |
