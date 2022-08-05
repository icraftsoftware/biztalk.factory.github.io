#### [Be.Stateless.BizTalk.Batching](README.md 'README')
### [Be.Stateless.BizTalk.Factory.Areas](Be.Stateless.BizTalk.Factory.Areas.md 'Be.Stateless.BizTalk.Factory.Areas')

## Batch Class

BizTalk Factory's process names.

```csharp
public class Batch : Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName<Be.Stateless.BizTalk.Factory.Areas.Batch>
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName-1 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName`1')[Batch](Batch.md 'Be.Stateless.BizTalk.Factory.Areas.Batch')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName-1 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName`1') &#129106; Batch

### Remarks

By convention, the token that precedes the 'Areas' or the 'Orchestrations' token of the CLR namespace denotes the
LOB/project to which a process belongs. The area is represented by the token that follows 'Areas' or
'Orchestrations', and the process name itself is the next token. For instance
`Be.Stateless.ECommerce.Areas.Shopping.CustomerRegistration`,
`Be.Stateless.ECommerce.Areas.Shopping.Invoicing`, and `Be.Stateless.ECommerce.Areas.Shopping.Shipping`
cover 3 different business processes (`CustomerRegistration`, `Invoicing`, and `Shipping`) in the
`Shopping` area if the `ECommerce` LOB/project.

These tokens are of importance for the monitoring web site accompanying BizTalk Factory.

### See Also
- [Be.Stateless.BizTalk.Factory.Areas.Default](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Factory.Areas.Default 'Be.Stateless.BizTalk.Factory.Areas.Default')

| Properties | |
| :--- | :--- |
| [Aggregate](Batch.Aggregate.md 'Be.Stateless.BizTalk.Factory.Areas.Batch.Aggregate') | Name of the batch aggregating messaging-only process/flow. |
| [Release](Batch.Release.md 'Be.Stateless.BizTalk.Factory.Areas.Batch.Release') | Name of the batch releasing messaging-only process/flow. |
