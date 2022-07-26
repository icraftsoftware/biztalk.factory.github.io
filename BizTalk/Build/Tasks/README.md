# Be.Stateless.BizTalk.Build.Tasks

Custom `MSBuild` tasks leveraging the artifacts written in either one of the `BizTalk.Factory`'s `DSL`s. The `Be.Stateless.BizTalk.Build.Tasks` assembly however provides only the `MSBuild` tasks, to actually integrate them into the `MSBuild` process, the developer has to reference the [BizTalk.Server.2020.Build][biztalk.server.2020.build] `NuGet` package, which tailors the `MSBuild` process to Microsoft BizTalk Server® 2020

<!--
TODO
- how native tasks are overridden, call patterns and sequences
 -->

<!-- links -->

[biztalk.server.2020.build]: https://www.nuget.org/packages/BizTalk.Server.2020.Build
