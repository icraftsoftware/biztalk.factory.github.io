#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FileAdapter](FileAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter')

## FileAdapter.Outbound Class

The File adapter transfers files into and out of Microsoft BizTalk Server.

```csharp
public class FileAdapter.Outbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [FileAdapter](FileAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter') &#129106; Outbound

Implements [IOutboundAdapter](IOutboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

### Remarks

The File send adapter transmits messages from the MessageBox database to a specified destination address (URL). You
define the URL, which is a file path and file name, by using wildcard characters related to the message context
properties. The File send adapter resolves the wildcard characters to the actual file name before writing the message
to the file.
            When writing a message to a file, the File send adapter gets the message content from the body part of the BizTalk
            Message object. The File send adapter ignores other message parts in the BizTalk Message object. After the File
            adapter writes the message to a file, it deletes the message from the MessageBox database. The File adapter writes
            files to the file system either directly or by using the file system cache, which can improve performance,
            particularly for large files.
            

<b>File Send Adapter Batching Support</b>

The File send adapter gets batches of messages from the MessageBox database and writes them to files in destination
locations on the file system or the network share. The size of File send adapter batches is not configurable and is
preset to 20. If BizTalk Server fails to write some of the messages within a batch to files, the system resubmits
those messages to the MessageBox database for retry processing. You can configure the retry interval and retry count
by using the BizTalk Server Administration console.

### See Also
- [File Adapter](https://docs.microsoft.com/en-us/biztalk/core/file-adapter 'https://docs.microsoft.com/en-us/biztalk/core/file-adapter')
- [File Send Adapter](https://docs.microsoft.com/en-us/biztalk/core/file-adapter#file-send-adapter 'https://docs.microsoft.com/en-us/biztalk/core/file-adapter#file-send-adapter')
- [Configure the File adapter](https://docs.microsoft.com/en-us/biztalk/core/configure-the-file-adapter 'https://docs.microsoft.com/en-us/biztalk/core/configure-the-file-adapter')

| Constructors | |
| :--- | :--- |
| [Outbound()](FileAdapter.Outbound.Outbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.Outbound()') | |
| [Outbound(Action&lt;Outbound&gt;)](FileAdapter.Outbound.Outbound(Action_Outbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.Outbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound>)') | |

| Properties | |
| :--- | :--- |
| [AllowCacheOnWrite](FileAdapter.Outbound.AllowCacheOnWrite.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.AllowCacheOnWrite') | Allow cache on write. |
| [DestinationFolder](FileAdapter.Outbound.DestinationFolder.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.DestinationFolder') | Destination folder. |
| [FileName](FileAdapter.Outbound.FileName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.FileName') | Destination file name. |
| [Mode](FileAdapter.Outbound.Mode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.Mode') | File content writing mode. |
| [UseTempFileOnWrite](FileAdapter.Outbound.UseTempFileOnWrite.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.UseTempFileOnWrite') | Use temporary file while writing. |

| Methods | |
| :--- | :--- |
| [GetAddress()](FileAdapter.Outbound.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.GetAddress()') | |
| [Save(IPropertyBag)](FileAdapter.Outbound.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
| [Validate()](FileAdapter.Outbound.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.Validate()') | |
