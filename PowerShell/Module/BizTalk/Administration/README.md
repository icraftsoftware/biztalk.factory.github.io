# BizTalk.Administration PowerShell Module

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

[![][module.badge]][module]

[![][module.preview.badge]][module.preview]

</div>
</div>

## Overview

`BizTalk.Administration` is a `PowerShell` utility module providing commands to administrate, configure, and explore Microsoft BizTalk Server®. For a detailed understanding of the commands, you are redirected to the `PowerShell` inline help that provides a comprehensive documentation.

For the `PowerShell` newbies, you can get a list of all the commands available via the following `PowerShell` command:

```PowerShell
Get-Command -Module BizTalk.Administration
```

You can then get detailed help on an individual command via a `PowerShell` command similar to what follows:

```PowerShell
Get-Help -Name New-BizTalkHandler -Detailed
```

## Installation

In order to be able to install the `PowerShell` module, you might have to trust the `be.stateless`'s certificate public key beforehand; see these [instructions](../../Installation.md) for details on how to proceed.

<!-- links -->

[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK"
[doc.this]: https://www.stateless.be/PowerShell/Module/BizTalk/Administration/ "BizTalk.Administration PowerShell Module"
[doc.install]: https://www.stateless.be/PowerShell/Module/Installation.html "PowerShell Module Installation"
[github]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Administration "Be.Stateless.PowerShell.Module.BizTalk.Administration GitHub Repository"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.PowerShell.Module.BizTalk.Administration&logo=github
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=27&branchName=master "Azure DevOps Continuous Integration Build Pipeline"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.PowerShell.Module.BizTalk.Administration%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=28&branchName=master "Azure DevOps Release Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.PowerShell.Module.BizTalk.Administration%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[module.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=BizTalk.Administration&protocolType=NuGet "BizTalk.Administration PowerShell Module Preview"
[module.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/BizTalk.Administration?logo=powershell
[module]: https://www.powershellgallery.com/packages/BizTalk.Administration "BizTalk.Administration Module"
[module.badge]: https://img.shields.io/powershellgallery/v/BizTalk.Administration.svg?label=BizTalk.Administration&style=flat&logo=powershell
[release]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Administration/releases/latest "Be.Stateless.PowerShell.Module.BizTalk.Administration Release"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Administration?label=Release&logo=github
