#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigPerformanceCounters](IAdapterConfigPerformanceCounters.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigPerformanceCounters')

## IAdapterConfigPerformanceCounters.EnablePerformanceCounters Property

Specifies whether to enable the WCF LOB Adapter SDK performance counters and the LOB Latency performance counter. The
LOB Latency performance counter measures the total time spent by the adapter in making calls to the system.

```csharp
bool EnablePerformanceCounters { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

EnablePerformanceCounters is a static property within an application domain for the WCF LOB Adapter SDK performance
counters, but it is an instance property for the adapter's LOB Latency performance counter. This means that changing
EnablePerformanceCounters for a binding instance in an application domain will:
- enable or disable the WCF LOB Adapter SDK performance counters for all objects created from all binding instances
  within the same app domain.
- enable or disable the adapter's LOB Latency performance counter only for objects created from that binding instance
  after the change is made.

It defaults to `False`.