#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Inbound](HttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound')

## HttpAdapter.Inbound.Path Property

Specify the name of the virtual directory where you post the messages received by the HTTP/HTTPS receive location.
The virtual directory includes the name of the receive location DLL and an optional query string.

```csharp
public string Path { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Example

Examples of virtual directory names are:

/<virtual directory>/BTSHTTPReceive.dll

/<virtual directory>/BTSHTTPReceive.dll?Purchase%20Order

### Remarks
This location must not contain more than one BTSHTTPReceive.dll ISAPI extension, including all subfolders.