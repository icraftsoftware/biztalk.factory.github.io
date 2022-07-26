#### [Be.Stateless.Stream](README.md 'README')

## Be.Stateless.IO Namespace

| Classes | |
| :--- | :--- |
| [BufferController](BufferController.md 'Be.Stateless.IO.BufferController') | Control operations on a temporary buffer. |
| [EnumerableStream](EnumerableStream.md 'Be.Stateless.IO.EnumerableStream') | Transform an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of either [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')s or arrays of [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')s into a readonly, non-seekable [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') of [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')s. |
| [Path](Path.md 'Be.Stateless.IO.Path') | |
| [StringStream](StringStream.md 'Be.Stateless.IO.StringStream') | Stream-derived class meant to minimize the amount of overhead required to wrap a string as a stream. |
| [TransactionalFile](TransactionalFile.md 'Be.Stateless.IO.TransactionalFile') | Provides static methods for the creation of transactional [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') or [TransactionalFileStream](TransactionalFileStream.md 'Be.Stateless.IO.TransactionalFileStream') objects. |
| [TransactionalFileStream](TransactionalFileStream.md 'Be.Stateless.IO.TransactionalFileStream') | [System.IO.FileStream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.FileStream 'System.IO.FileStream') subclass to be used when the underlying stream is transacted and its scoping transaction             requires and explicit commit because it is not DTC enlisted. |

| Interfaces | |
| :--- | :--- |
| [IKernelTransaction](IKernelTransaction.md 'Be.Stateless.IO.IKernelTransaction') | |
| [ITransactionalStream](ITransactionalStream.md 'Be.Stateless.IO.ITransactionalStream') | Represents a transaction to be performed at a transactional stream, like [TransactionalFileStream](TransactionalFileStream.md 'Be.Stateless.IO.TransactionalFileStream'). |
