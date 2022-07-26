# Be.Stateless.BizTalk.ServiceModel

<div class="badges">
<div>

[![][github.badge]][github]

[![][release.badge]][release]

</div>
<div>

[![][pipeline.ci.badge]][pipeline.ci]

[![][pipeline.mr.badge]][pipeline.mr]

</div>
<div>

[![][nuget.badge]][nuget]

[![][nuget.unit.badge]][nuget.unit]

[![][nuget.nunit.badge]][nuget.nunit]

</div>
</div>

## Overview

`Be.Stateless.BizTalk.ServiceModel` is part of the [BizTalk.Factory Runtime](./../../BizTalk/Factory/Runtime/README.md) Package. This component provides both `WCF` behavior extensions dedicated to Microsoft BizTalk Server®, and utility classes allowing to compose `WCF` relays using Microsoft BizTalk Server® schema and map artifacts.

## Running the Unit Tests

You will first need to execute the following commands in an `PowerShell` elevated session in order to be able to run all the unit tests:

```powershell
netsh http add urlacl url=http://+:8000/soap-stub/ user=$env:USERDOMAIN\$env:USERNAME
netsh http add urlacl url=http://+:8001/calculator/ user=$env:USERDOMAIN\$env:USERNAME
```

## Developer Help

Detailed developer help has been provided as `XML` comments directly embedded in source code. Though developers usually browse through this documentation while developing thanks to, for instance, JetBrains [ReSharper][resharper] quick help &mdash;<kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>F1</kbd>, an online version of this inlined help has also been provided here for greater reachability:

[![][help.badge]][help]

[![][help.unit.badge]][help.unit]

[![][help.nunit.badge]][help.nunit]

<!-- links -->

[help]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/ServiceModel/README.md "Be.Stateless.BizTalk.ServiceModel Developer Help"
[help.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.ServiceModel&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help.nunit]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/ServiceModel/NUnit/README.md "Be.Stateless.BizTalk.ServiceModel.NUnit Developer Help"
[help.nunit.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.ServiceModel.NUnit&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help.unit]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/ServiceModel/Unit/README.md "Be.Stateless.BizTalk.ServiceModel.Unit Developer Help"
[help.unit.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.ServiceModel.Unit&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.ServiceModel "Be.Stateless.BizTalk.ServiceModel GitHub Repository"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.ServiceModel&logo=github
[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.ServiceModel "Be.Stateless.BizTalk.ServiceModel NuGet Package"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.ServiceModel.svg?label=Be.Stateless.BizTalk.ServiceModel&style=flat&logo=nuget
[nuget.unit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.ServiceModel.Unit "Be.Stateless.BizTalk.ServiceModel.Unit NuGet Package"
[nuget.unit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.ServiceModel.Unit.svg?label=Be.Stateless.BizTalk.ServiceModel.Unit&style=flat&logo=nuget
[nuget.nunit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.ServiceModel.NUnit "Be.Stateless.BizTalk.ServiceModel.NUnit NuGet Package"
[nuget.nunit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.ServiceModel.NUnit.svg?label=Be.Stateless.BizTalk.ServiceModel.NUnit&style=flat&logo=nuget
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=64&branchName=master "Azure DevOps Continuous Integration Build Pipeline"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.ServiceModel%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=65&branchName=master "Azure DevOps Release Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.ServiceModel%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.ServiceModel/releases/latest "Be.Stateless.BizTalk.ServiceModel GitHub Release"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.ServiceModel?label=Release&logo=github

<!--  -->

[resharper]: https://www.jetbrains.com/resharper/

<!--
cSpell:ignore edoc
-->
