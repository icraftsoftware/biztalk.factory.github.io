#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FileAdapter](FileAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter')

## FileAdapter.Inbound Class

The File adapter transfers files into and out of Microsoft BizTalk Server.

```csharp
public class FileAdapter.Inbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [FileAdapter](FileAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter') &#129106; Inbound

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

### Remarks

Use the File receive adapter to read messages from files, and submit them to the server. The receive adapter reads
the file, and creates a BizTalk Message object, so that BizTalk Server can process the message. While reading from
the file, the adapter locks the file to ensure that no modifications can be made to the file content

The File receive adapter reads the messages from files on local file systems or on network shares. When the specified
location on a network share is unavailable due to network problems, the receive adapter retries the read operation
(the number of retries is configurable in the BizTalk Server Administration console). After the message has been read
and successfully accepted by the BizTalk Messaging Engine, the receive adapter deletes the file from the file system
or network share. If the message was read but the pipeline did not successfully process the message, the adapter puts
the message in the suspended queue and then deletes the file from the file system or network share. If the File
receive adapter cannot submit or suspend the message to the MessageBox database, it does not delete the original file
from the file system or network share.

You can also configure the File receive adapter to rename files when processing them. You should rename files to
ensure that the receive adapter does not generate duplicate messages if the receive location is shut down and
restarted. This is a configurable option for File receive locations. By default, renaming is disabled. When renaming
is enabled, the File receive adapter appends the extension .BTS-WIP to the file. The receive adapter then reads the
messages from the renamed file in the receive location and submits it to the server. After the receive adapter has
successfully submitted a file, the receive adapter deletes the renamed file from the file system or network share. If
a message has been read but failed processing in the pipeline, the receive adapter places the message in the
MessageBox database suspended queue, and deletes the renamed file from the network share.

If the File receive adapter successfully reads the message but did not successfully store the message in the
MessageBox database, the renamed file reverts to its original name, without the .BTS-WIP extension. Note that the
receive adapter does not read files with the extension .BTS-WIP if the renaming option is turned on.

<b>Using file change notifications and polling</b>

The File receive adapter relies on Windows File Change Notifications to determine when to pick up a file from the
specified directory or share. If the File receive adapter receives a Windows File Change Notification before the file
has been completely written to the specified directory or share then the file will be locked and the File receive
adapter will not retrieve the file. In this scenario, the File receive adapter will actively poll the specified
directory or share at the Polling interval (ms) specified on the Advanced settings dialog box available when
configuring a File receive location. When the File receive adapter polls a directory or share it retrieves unlocked
files from the share and submits the files to the MessageBox database.

<b>File Receive Adapter Batching Support</b>

The File receive adapter submits messages to the server in batches. The File receive adapter starts by building a
single batch per receive location by collecting all the readable files available in the receive location. Batches are
submitted to the MessageBox database by the receive adapter when all the available files have been collected or when
the amount of files collected exceeds the maximum batch size.

After all the messages within the batch have been successfully read and submitted into the MessageBox database, the
File receive adapter deletes the corresponding files from the receive location. If some of the messages within the
batch failed processing, the File receive adapter suspends them and deletes the corresponding files from the receive
location. If some or all of the messages fail to be stored in the MessageBox database, the entire batch operation is
rolled back and all corresponding files are left unchanged in the receive location.

### See Also
- [File Adapter](https://docs.microsoft.com/en-us/biztalk/core/file-adapter 'https://docs.microsoft.com/en-us/biztalk/core/file-adapter')
- [File receive adapter](https://docs.microsoft.com/en-us/biztalk/core/file-adapter#file-receive-adapter 'https://docs.microsoft.com/en-us/biztalk/core/file-adapter#file-receive-adapter')
- [Using file change notifications and polling](https://docs.microsoft.com/en-us/biztalk/core/file-adapter#using-file-change-notifications-and-polling 'https://docs.microsoft.com/en-us/biztalk/core/file-adapter#using-file-change-notifications-and-polling')
- [File Receive Adapter Batching Support](https://docs.microsoft.com/en-us/biztalk/core/file-adapter#file-receive-adapter-batching-support 'https://docs.microsoft.com/en-us/biztalk/core/file-adapter#file-receive-adapter-batching-support')
- [Configure the File adapter](https://docs.microsoft.com/en-us/biztalk/core/configure-the-file-adapter 'https://docs.microsoft.com/en-us/biztalk/core/configure-the-file-adapter')

| Constructors | |
| :--- | :--- |
| [Inbound()](FileAdapter.Inbound.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.Inbound()') | |
| [Inbound(Action&lt;Inbound&gt;)](FileAdapter.Inbound.Inbound(Action_Inbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound>)') | |

| Properties | |
| :--- | :--- |
| [BatchMessagesCount](FileAdapter.Inbound.BatchMessagesCount.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.BatchMessagesCount') | Specify the maximum number of messages to be submitted in a batch. |
| [BatchSize](FileAdapter.Inbound.BatchSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.BatchSize') | Specify the maximum total bytes for a batch. |
| [FileMask](FileAdapter.Inbound.FileMask.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.FileMask') | Source file mask. |
| [FileRemovingSettings](FileAdapter.Inbound.FileRemovingSettings.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.FileRemovingSettings') | |
| [PollingInterval](FileAdapter.Inbound.PollingInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.PollingInterval') | Receive location polling interval. |
| [ReceiveFolder](FileAdapter.Inbound.ReceiveFolder.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.ReceiveFolder') | Source folder. |
| [RenameReceivedFiles](FileAdapter.Inbound.RenameReceivedFiles.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.RenameReceivedFiles') | Renames files while reading. |
| [RetryCountOnNetworkFailure](FileAdapter.Inbound.RetryCountOnNetworkFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.RetryCountOnNetworkFailure') | Specify the number of attempts to access the receive location on a network share if it is temporarily unavailable. |
| [RetryIntervalOnNetworkFailure](FileAdapter.Inbound.RetryIntervalOnNetworkFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.RetryIntervalOnNetworkFailure') | Specify the retry interval time (in minutes) between attempts to access the receive location on the network share if it is temporarily unavailable. |

| Methods | |
| :--- | :--- |
| [GetAddress()](FileAdapter.Inbound.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.GetAddress()') | |
| [Save(IPropertyBag)](FileAdapter.Inbound.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
| [Validate()](FileAdapter.Inbound.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound.Validate()') | |
