#### [Be.Stateless.BizTalk.Process.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Process](Be.Stateless.BizTalk.Unit.Process.md 'Be.Stateless.BizTalk.Unit.Process').[ProcessFixtureBase](ProcessFixtureBase.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase')

## ProcessFixtureBase.SystemOutputFolders Property

Output system (e.g. Claim Check) folders where output files are dropped.

```csharp
protected virtual System.Collections.Generic.IEnumerable<string> SystemOutputFolders { get; }
```

#### Property Value
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

### Remarks

All folders, whether [SystemInputFolders](ProcessFixtureBase.SystemInputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.SystemInputFolders'), [SystemOutputFolders](ProcessFixtureBase.SystemOutputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.SystemOutputFolders'), [InputFolders](ProcessFixtureBase.InputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.InputFolders'),
or [OutputFolders](ProcessFixtureBase.OutputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.OutputFolders') will always be created if necessary. Besides all output folders, that is [SystemOutputFolders](ProcessFixtureBase.SystemOutputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.SystemOutputFolders') and [OutputFolders](ProcessFixtureBase.OutputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.OutputFolders'), will be emptied immediately before each test is run,
while all input folders, that is [SystemInputFolders](ProcessFixtureBase.SystemInputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.SystemInputFolders') and [InputFolders](ProcessFixtureBase.InputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.InputFolders'), will be emptied
immediately after each test has run.

Any override must call its base class overridden [SystemOutputFolders](ProcessFixtureBase.SystemOutputFolders.md 'Be.Stateless.BizTalk.Unit.Process.ProcessFixtureBase.SystemOutputFolders') member so that not any system
folder is ever missing in the list.