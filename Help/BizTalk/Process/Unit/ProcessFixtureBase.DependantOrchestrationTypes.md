#### [Be.Stateless.BizTalk.Process.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Process](Be.Stateless.BizTalk.Unit.Process.md 'Be.Stateless.BizTalk.Unit.Process').[ProcessFixtureBase](ProcessFixtureBase.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase')

## ProcessFixtureBase.DependantOrchestrationTypes Property

Ordered list of orchestration types that this process depends upon.

```csharp
protected virtual System.Collections.Generic.IEnumerable<System.Type> DependantOrchestrationTypes { get; }
```

#### Property Value
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

### Remarks

Dependant orchestrations will be started before any test method of this process is run; notice that they will be
started in the order in which they were given. Likewise, dependant orchestrations will be unenlisted after all of the
test methods of this process has run; notice that they will be unenlisted in the reverse order in which they were
given.

Any service instance of any one of the dependant orchestrations will be terminated after each test method of this
process has run should the service instance be suspended or still be running.