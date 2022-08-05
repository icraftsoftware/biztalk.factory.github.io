#### [Be.Stateless.BizTalk.Process.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Process](Be.Stateless.BizTalk.Unit.Process.md 'Be.Stateless.BizTalk.Unit.Process')

## ProcessFixtureBase Class

```csharp
public abstract class ProcessFixtureBase
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ProcessFixtureBase

Derived  
&#8627; [OrchestrationFixtureBase&lt;T&gt;](OrchestrationFixtureBase_T_.md 'Be.Stateless.BizTalk.Unit.Process.OrchestrationFixtureBase<T>')

| Properties | |
| :--- | :--- |
| [AllDependantOrchestrationTypes](ProcessFixtureBase.AllDependantOrchestrationTypes.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.AllDependantOrchestrationTypes') | |
| [BizTalkServiceInstances](ProcessFixtureBase.BizTalkServiceInstances.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.BizTalkServiceInstances') | |
| [DependantOrchestrationTypes](ProcessFixtureBase.DependantOrchestrationTypes.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.DependantOrchestrationTypes') | Ordered list of orchestration types that this process depends upon. |
| [InputFolders](ProcessFixtureBase.InputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.InputFolders') | Input folders where input files are dropped. |
| [OutputFolders](ProcessFixtureBase.OutputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.OutputFolders') | Output folders where output files are dropped. |
| [StartTime](ProcessFixtureBase.StartTime.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.StartTime') | |
| [SystemInputFolders](ProcessFixtureBase.SystemInputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.SystemInputFolders') | Input system (e.g. Claim Check) folders where input files are dropped. |
| [SystemOutputFolders](ProcessFixtureBase.SystemOutputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.SystemOutputFolders') | Output system (e.g. Claim Check) folders where output files are dropped. |

| Methods | |
| :--- | :--- |
| [Initialize()](ProcessFixtureBase.Initialize().md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.Initialize()') | |
| [InitializeFixture()](ProcessFixtureBase.InitializeFixture().md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.InitializeFixture()') | |
| [Terminate()](ProcessFixtureBase.Terminate().md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.Terminate()') | |
| [TerminateFixture()](ProcessFixtureBase.TerminateFixture().md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.TerminateFixture()') | |
| [TerminateUncompletedBizTalkServiceInstances()](ProcessFixtureBase.TerminateUncompletedBizTalkServiceInstances().md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.TerminateUncompletedBizTalkServiceInstances()') | Terminate all BizTalk service instances that are still running or that have been suspended. |
