#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding').[ISendPort&lt;TNamingConvention&gt;](ISendPort_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>')

## ISendPort<TNamingConvention>.State Property

The state of the send port.

```csharp
Be.Stateless.BizTalk.Dsl.Binding.ServiceState State { get; set; }
```

#### Property Value
[ServiceState](ServiceState.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceState')

### Remarks
A send port can be in either one of the following state:
- [Unenlisted](ServiceState.md#Be.Stateless.BizTalk.Dsl.Binding.ServiceState.Unenlisted 'Be.Stateless.BizTalk.Dsl.Binding.ServiceState.Unenlisted');
- [Enlisted](ServiceState.md#Be.Stateless.BizTalk.Dsl.Binding.ServiceState.Enlisted 'Be.Stateless.BizTalk.Dsl.Binding.ServiceState.Enlisted'), or equivalently, [Stopped](ServiceState.md#Be.Stateless.BizTalk.Dsl.Binding.ServiceState.Stopped 'Be.Stateless.BizTalk.Dsl.Binding.ServiceState.Stopped');
- [Started](ServiceState.md#Be.Stateless.BizTalk.Dsl.Binding.ServiceState.Started 'Be.Stateless.BizTalk.Dsl.Binding.ServiceState.Started')