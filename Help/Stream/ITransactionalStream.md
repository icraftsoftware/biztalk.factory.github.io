#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO')

## ITransactionalStream Interface

Represents a transaction to be performed at a transactional stream, like [TransactionalFileStream](TransactionalFileStream.md 'Be.Stateless.IO.TransactionalFileStream').

```csharp
public interface ITransactionalStream
```

Derived  
&#8627; [TransactionalFileStream](TransactionalFileStream.md 'Be.Stateless.IO.TransactionalFileStream')

| Methods | |
| :--- | :--- |
| [Commit()](ITransactionalStream.Commit().md 'Be.Stateless.IO.ITransactionalStream.Commit()') | Commits the stream transaction. |
| [Rollback()](ITransactionalStream.Rollback().md 'Be.Stateless.IO.ITransactionalStream.Rollback()') | Rolls back a stream transaction from a pending state. |
