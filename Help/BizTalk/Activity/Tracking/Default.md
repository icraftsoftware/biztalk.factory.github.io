#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Factory.Areas](Be.Stateless.BizTalk.Factory.Areas.md 'Be.Stateless.BizTalk.Factory.Areas')

## Default Class

Default names for the messaging-only processes/flows tracked by BizTalk Factory.

```csharp
public class Default : Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName<Be.Stateless.BizTalk.Factory.Areas.Default>
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName&lt;](ProcessName_T_.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName<T>')[Default](Default.md 'Be.Stateless.BizTalk.Factory.Areas.Default')[&gt;](ProcessName_T_.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName<T>') &#129106; Default

### Remarks

By convention, the token that precedes the 'Areas' or the 'Orchestrations' token of the CLR namespace denotes the
LOB/project to which a process belongs. The area is represented by the token that follows 'Areas' or
'Orchestrations', and the process name itself is the next token. For instance
`Be.Stateless.ECommerce.Areas.Shopping.CustomerRegistration`,
`Be.Stateless.ECommerce.Areas.Shopping.Invoicing`, and `Be.Stateless.ECommerce.Areas.Shopping.Shipping`
cover 3 different business processes (`CustomerRegistration`, `Invoicing`, and `Shipping`) in the
`Shopping` area if the `ECommerce` LOB/project.

These tokens are of importance for the monitoring web site accompanying BizTalk Factory. An area named [Default](Default.md 'Be.Stateless.BizTalk.Factory.Areas.Default') can be used when one does not wish to use areas to partition processes. The default area will not
appear in the monitoring site.

| Properties | |
| :--- | :--- |
| [Failed](Default.Failed.md 'Be.Stateless.BizTalk.Factory.Areas.Default.Failed') | Default name for failed messaging-only flows. |
| [Unidentified](Default.Unidentified.md 'Be.Stateless.BizTalk.Factory.Areas.Default.Unidentified') | Default name for unidentified messaging-only flows. |
