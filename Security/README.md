# Be.Stateless.Security

[![][github.badge]][github]

##### Build Pipelines

[![][pipeline.mr.badge]][pipeline.mr]

[![][pipeline.ci.badge]][pipeline.ci]

##### Latest Release

[![][nuget.badge]][nuget]

[![][release.badge]][release]

##### Release Preview

[![][nuget.preview.badge]][nuget.preview]

## Overview

`Be.Stateless.Security` is part of the [BizTalk.Factory Runtime](./../BizTalk/Factory/Runtime/README.md) Package. This component provides a security helper class, [Delegate][delegate], allowing to impersonate a Windows identity &mdash;whose `username` and `password` are given as arguments&mdash; when invoking a .NET `delegate`.

> **Remark** The only reasons and places this class is used so far is to create a folder ahead of time in a Microsoft BizTalk Server® send pipeline; thus allowing the File adapter to drop the message at the expected runtime-computed location, see [DirectoryCreator][directory-creator].

## Developer Help

Detailed developer help has been provided as `XML` comments directly embedded in source code. Though developers usually browse through this documentation while developing thanks to, for instance, JetBrains [ReSharper][resharper] quick help &mdash;<kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>F1</kbd>, an online version of this inlined help has also been provided here for greater reachability:

[![][help.badge]][help]

<!-- badges -->

[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=Be.Stateless.Security&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/Security "Be.Stateless.Security User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.Security&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.Security "Be.Stateless.Security GitHub Repository"
[help.badge]: https://img.shields.io/static/v1?label=Be.Stateless.Security&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/Security/README.md "Be.Stateless.Security Developer Help"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.Security.svg?label=Be.Stateless.Security&style=flat&logo=nuget
[nuget]: https://www.nuget.org/packages/Be.Stateless.Security "Be.Stateless.Security NuGet Package"
[nuget.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.Security?logo=nuget
[nuget.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.Security&protocolType=NuGet "Be.Stateless.Security Preview NuGet Package"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.Security%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=92&branchName=master "Be.Stateless.Security Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.Security%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=93&branchName=master "Be.Stateless.Security Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.Security?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.Security/releases/latest "Be.Stateless.Security GitHub Release"

<!-- links -->

[delegate]: https://github.com/icraftsoftware/Be.Stateless.Security/blob/master/src/Be.Stateless.Security/Delegate.cs
[directory-creator]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/936a6130f8238a7e243829e97c923fa35a3feba3/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/DirectoryCreator.cs#L40
[resharper]: https://www.jetbrains.com/resharper/
