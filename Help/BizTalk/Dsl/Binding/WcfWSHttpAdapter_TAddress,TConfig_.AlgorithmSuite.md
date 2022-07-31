#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWSHttpAdapter&lt;TAddress,TConfig&gt;](WcfWSHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>')

## WcfWSHttpAdapter<TAddress,TConfig>.AlgorithmSuite Property

Specify the message encryption and key-wrap algorithms. These algorithms map to those specified in the Security
Policy Language (WS-SecurityPolicy) specification.

```csharp
public Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue AlgorithmSuite { get; set; }
```

Implements [AlgorithmSuite](IAdapterConfigMessageSecurity_T_.AlgorithmSuite.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>.AlgorithmSuite')

#### Property Value
[Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue 'Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue')

### Remarks

For more information about the member names for the [AlgorithmSuite](WcfWSHttpAdapter_TAddress,TConfig_.AlgorithmSuite.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>.AlgorithmSuite') property, see the Algorithm suite
property in [WCF-WSHttp
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-receive-security-tab') and [WCF-WSHttp
            Transport Properties Dialog Box, Send, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-send-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-send-security-tab').

It defaults to [Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue.Basic256](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue.Basic256 'Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue.Basic256').