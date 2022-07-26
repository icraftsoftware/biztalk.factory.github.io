#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[TransactionalFileStream](TransactionalFileStream.md 'Be.Stateless.IO.TransactionalFileStream')

## TransactionalFileStream.Dispose(bool) Method

Note that because the base class does mix the Close() and Dispose() operations, one can commit the transaction
if properly closed, and rollback it if disposed...

```csharp
protected override void Dispose(bool disposing);
```
#### Parameters

<a name='Be.Stateless.IO.TransactionalFileStream.Dispose(bool).disposing'></a>

`disposing` [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')