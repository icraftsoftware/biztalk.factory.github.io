#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigMaxConcurrentCalls](IAdapterConfigMaxConcurrentCalls.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxConcurrentCalls')

## IAdapterConfigMaxConcurrentCalls.MaxConcurrentCalls Property

Specify the number of concurrent calls to a single service instance. Calls in excess of the limit are queued.

```csharp
int MaxConcurrentCalls { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks

The range of this property is from 0 to [System.Int32.MaxValue](https://docs.microsoft.com/en-us/dotnet/api/System.Int32.MaxValue 'System.Int32.MaxValue'). Setting this value to 0 is equivalent to setting
it to [System.Int32.MaxValue](https://docs.microsoft.com/en-us/dotnet/api/System.Int32.MaxValue 'System.Int32.MaxValue').

It defaults to 200.