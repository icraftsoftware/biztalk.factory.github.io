# BizTalk.Factory Application

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

[![][package.badge]][package]

</div>
</div>

## Overview

This Application is the `BizTalk.Factory`'s **core** Microsoft BizTalk Server® application. `BizTalk.Factory` Application Package is part of the larger [BizTalk.Factory](./../../../README.md) SDK and is made of the following components:

- [Be.Stateless.BizTalk.Pipeline.Components](./../../Pipeline/Components/README.md) provides very lightweight yet tremendously helpful Microsoft BizTalk Server® pipeline components;

- [Be.Stateless.BizTalk.Pipelines](./../../Pipelines/README.md) provides versatile _"one-size-fits-all"_ pipelines for general purpose Microsoft BizTalk Server® development;

- [Be.Stateless.BizTalk.Schemas](./../../Schemas/README.md) provides `BizTalk.Factory`'s document and property schemas for general purpose Microsoft BizTalk Server® development.

## Installation

### Environment Settings Overrides

<!--
Custom databases
    BizTalkFactoryMgmtDb installed on $ManagementServer `
    BizTalkFactoryTransientStateDb installed on $ProcessingServer `
SsoConfigStore
    Be.Stateless.BizTalk.Factory.Settings
-->

<!-- links -->

[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Application "Be.Stateless.BizTalk.Factory.Application GitHub Repository"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Factory.Application&logo=github
[package]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Application/releases/latest/download/Be.Stateless.BizTalk.Factory.Application.Deployment.zip "Be.Stateless.BizTalk.Factory.Application Deployment Package"
[package.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Factory.Application?label=Be.Stateless.BizTalk.Factory.Application.Deployment.zip&style=flat&logo=github
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=85&branchName=master "Azure DevOps Continuous Integration Build Pipeline"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Factory.Application%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=86&branchName=master "Azure DevOps Release Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Factory.Application%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Application/releases/latest "Be.Stateless.BizTalk.Factory.Application GitHub Release"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Factory.Application?label=Release&logo=github

<!--
cSpell:ignore BizTalkFactoryMgmtDb
-->
