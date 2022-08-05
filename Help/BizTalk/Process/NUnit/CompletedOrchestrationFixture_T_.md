#### [Be.Stateless.BizTalk.Process.NUnit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Process](Be.Stateless.BizTalk.Unit.Process.md 'Be.Stateless.BizTalk.Unit.Process')

## CompletedOrchestrationFixture<T> Class

Process fixture base class that automatically asserts that there is no uncompleted BizTalk Service instance.

```csharp
public abstract class CompletedOrchestrationFixture<T> : Be.Stateless.BizTalk.Unit.Process.OrchestrationFixture<T>
    where T : Microsoft.BizTalk.XLANGs.BTXEngine.BTXService
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.Process.CompletedOrchestrationFixture_T_.T'></a>

`T`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase') &#129106; [Be.Stateless.BizTalk.Unit.Process.OrchestrationFixtureBase&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.Process.OrchestrationFixtureBase-1 'Be.Stateless.BizTalk.Unit.Process.OrchestrationFixtureBase`1')[T](CompletedOrchestrationFixture_T_.md#Be.Stateless.BizTalk.Unit.Process.CompletedOrchestrationFixture_T_.T 'Be.Stateless.BizTalk.Unit.Process.CompletedOrchestrationFixture<T>.T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.Process.OrchestrationFixtureBase-1 'Be.Stateless.BizTalk.Unit.Process.OrchestrationFixtureBase`1') &#129106; [Be.Stateless.BizTalk.Unit.Process.OrchestrationFixture&lt;](OrchestrationFixture_T_.md 'Be.Stateless.BizTalk.Unit.Process.OrchestrationFixture<T>')[T](CompletedOrchestrationFixture_T_.md#Be.Stateless.BizTalk.Unit.Process.CompletedOrchestrationFixture_T_.T 'Be.Stateless.BizTalk.Unit.Process.CompletedOrchestrationFixture<T>.T')[&gt;](OrchestrationFixture_T_.md 'Be.Stateless.BizTalk.Unit.Process.OrchestrationFixture<T>') &#129106; CompletedOrchestrationFixture<T>

Derived  
&#8627; [CompletedSoapedOrchestrationFixture&lt;T&gt;](CompletedSoapedOrchestrationFixture_T_.md 'Be.Stateless.BizTalk.Unit.Process.CompletedSoapedOrchestrationFixture<T>')