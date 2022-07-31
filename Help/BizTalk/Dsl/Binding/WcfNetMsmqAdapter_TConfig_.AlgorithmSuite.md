#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter&lt;TConfig&gt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>')

## WcfNetMsmqAdapter<TConfig>.AlgorithmSuite Property

Specify the message encryption and key-wrap algorithms. These algorithms map to those specified in the Security
Policy Language (WS-SecurityPolicy) specification.

```csharp
public Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue AlgorithmSuite { get; set; }
```

Implements [AlgorithmSuite](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.AlgorithmSuite 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.AlgorithmSuite'), [AlgorithmSuite](IAdapterConfigMessageSecurity_T_.AlgorithmSuite.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>.AlgorithmSuite')

#### Property Value
[Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue 'Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue')

### Remarks

For more information about the member names for the [Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue 'Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue') property, see the
Message client credential type property in [WCF-NetMsmq
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-receive-security-tab').

It defaults to [Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue.Basic256](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue.Basic256 'Microsoft.BizTalk.Adapter.Wcf.Config.SecurityAlgorithmSuiteValue.Basic256').