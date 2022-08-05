#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter&lt;TConfig&gt;](WcfSapAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<TConfig>')

## WcfSapAdapter<TConfig>.RfcAllowStartProgram Property

Specifies the external programs that the RFC client library can start, if required by an RFC partner. For example, if
you are invoking an RFC that internally invokes a program on the computer running the adapter client, you must
specify the name of that program for this binding property.

```csharp
public string RfcAllowStartProgram { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

If you are specifying multiple programs for this binding property, they must be separated by a semi-colon. For
example, if you want to specify the sapftp and saphttp programs, you must specify them as sapftp;saphttp. Also, make
sure the following conditions are met:
- The external program required by the RFC is available on the computer running the adapter client.
- The location of the external program is present in the PATH variable on the computer running the adapter client.
For example, BAPI_DOCUMENT_CHECKOUTVIEW2 internally executes a program, sapftp. So, while invoking this RFC, you must
set the RfcAllowStartProgram binding property to sapftp. You must also ensure that the sapftp program is available
locally, and the location of the sapftp program is added to the PATH variable on the computer running the adapter
client.

It defaults to <seealso cref="F:System.String.Empty"/>.