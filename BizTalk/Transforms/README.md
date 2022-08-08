# Be.Stateless.BizTalk.Transforms

[![][github.badge]][github]

##### Build Pipelines

[![][pipeline.mr.badge]][pipeline.mr]

[![][pipeline.ci.badge]][pipeline.ci]

##### Latest Release

[![][nuget.badge]][nuget]

[![][nuget.unit.badge]][nuget.unit]

[![][release.badge]][release]

##### Release Preview

[![][nuget.preview.badge]][nuget.preview]

[![][nuget.unit.preview.badge]][nuget.unit.preview]

## Overview

`Be.Stateless.BizTalk.Transforms` is part of the [BizTalk.Factory Runtime](./../Factory/Runtime/README.md) Package. This component provides a transform class library for general purpose Microsoft BizTalk Server® development.

## Debugging Composite Microsoft BizTalk Server® Maps with Extension Objects

Provided the map fixture class derives from [TransformFixture][transform-fixture] base class and that both [`Be.Stateless.BizTalk.Transform.Unit`][nuget.unit] and [`BizTalk.Server.2020.Utilities`][nuget.utilities] `NuGet` packages are referenced, it is possible to debug `XSLT` maps that make use of extension objects or combine other `XSLT` stylesheets through `xsl:include` or `xsl:import` top-level elements.

Notice that the `URI`s accepted by the `href` attribute of these top-level elements are resolved by the [`XslMapUrlResolver`][xsl-mapurl-resolver] class and must conform to its prescribed grammar. Technically though, during a Microsoft Visual Studio®'s debugging session, it is the [MapCustomXsltPathResolver][map-custom-xslt-path-resolver] helper class that will actually resolve these `URI`s, trying to locate an `XSLT` source file on disk instead of inlined in a [TransformBase][transform-base]-derived type or embedded as a resource. This resolution will only succeed provided that:

- The to-be-debugged `XSLT` stylesheet file is lying by convention next to the source `.btm` file &mdash;or equivalently, next to the generated `.btm.cs` file&mdash; in the case of a Microsoft BizTalk Server® map defined by a custom `XSLT`;

- The to-be-debugged `XSLT` stylesheet file included or imported through a `URI` of the form `map://type/<map strong type name>` is lying next to the source `.btm` file of the included or imported map type;

- The to-be-debugged `XSLT` stylesheet file included or imported through a `URI` of the form `map://resource/<embedded resource name>` is lying by convention in a folder, located relatively to the including or importing map, that corresponds to the resource name suffix starting right after what the resource name has in common with the including or importing map type's full name;

- The to-be-debugged `XSLT` stylesheet file included or imported through a `URI` of the form `c:\folder\file.xslt` exists on disk.

> **Tips** Run the following commands in an elevated session of the "Developer PowerShell for VS 2019" prompt should the error "Retrieving the COM class factory for component with CLSID {E6756135-1E65-4D17-8576-610761398C3C} failed due to the following error: 80040154 Class not registered." occurs while debugging map unit tests:
>
> ```PowerShell
> regsvr32 $(Join-Path $env:VSINSTALLDIR 'Common7\IDE\Remote Debugger\x64\msdia140.dll')
> regsvr32 $(Join-Path $env:VSINSTALLDIR 'Common7\IDE\Remote Debugger\x86\msdia140.dll')
> ```
>
> Do not forget to reference the [`BizTalk.Server.2020.Utilities`][nuget.utilities] `NuGet` package should the error "Could not load file or assembly Microsoft.VisualStudio.Dia.dll." occurs.

### Customizing To-Be-Debugged `XSLT` File Resolution

Should the default resolution of the `XSLT` source file not be conclusive, due to other file layout conventions for instance, the map fixture's developer can control the resolution mechanism by overriding the [TransformFixture.TryResolveXsltPath][transform-fixture.try-resolve-xslt-path] method, which will always have the precedence over the default resolution used during debugging sessions.

## Developer Help

Detailed developer help has been provided as `XML` comments directly embedded in source code. Though developers usually browse through this documentation while developing thanks to, for instance, JetBrains [ReSharper][resharper] quick help &mdash;<kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>F1</kbd>, an online version of this inlined help has also been provided here for greater reachability:

[![][help.badge]][help]

[![][help.unit.badge]][help.unit]

<!-- badges -->

[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Transforms&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/BizTalk/Transforms "Be.Stateless.BizTalk.Transforms User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Transforms&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Transforms "Be.Stateless.BizTalk.Transforms GitHub Repository"
[help.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Transform.ExtensionObjects&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Transform/ExtensionObjects/README.md "Be.Stateless.BizTalk.Transform.ExtensionObjects Developer Help"
[help.unit.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Transform.Unit&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help.unit]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Transform/Unit/README.md "Be.Stateless.BizTalk.Transform.Unit Developer Help"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Transform.ExtensionObjects.svg?label=Be.Stateless.BizTalk.Transform.ExtensionObjects&style=flat&logo=nuget
[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Transform.ExtensionObjects "Be.Stateless.BizTalk.Transform.ExtensionObjects NuGet Package"
[nuget.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.BizTalk.Transform.ExtensionObjects?logo=nuget
[nuget.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.BizTalk.Transform.ExtensionObjects&protocolType=NuGet "Be.Stateless.BizTalk.Transform.ExtensionObjects Preview NuGet Package"
[nuget.unit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Transform.Unit.svg?label=Be.Stateless.BizTalk.Transform.Unit&style=flat&logo=nuget
[nuget.unit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Transform.Unit "Be.Stateless.BizTalk.Transform.Unit NuGet Package"
[nuget.unit.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.BizTalk.Transform.Unit?logo=nuget
[nuget.unit.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.BizTalk.Transform.Unit&protocolType=NuGet "Be.Stateless.BizTalk.Transform.Unit Preview NuGet Package"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Transforms%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=47&branchName=master "Be.Stateless.BizTalk.Transforms Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Transforms%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=48&branchName=master "Be.Stateless.BizTalk.Transforms Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Transforms?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Transforms/releases/latest "Be.Stateless.BizTalk.Transforms Release"

<!-- links -->

[map-custom-xslt-path-resolver]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Transforms/blob/master/src/Be.Stateless.BizTalk.Transform.Unit/Unit/Transform/MapCustomXsltPathResolver.cs
[nuget.utilities]: https://www.nuget.org/packages/BizTalk.Server.2020.Utilities
[resharper]: https://www.jetbrains.com/resharper/
[transform-base]: https://docs.microsoft.com/en-us/dotnet/api/microsoft.xlangs.basetypes.transformbase
[transform-fixture.try-resolve-xslt-path]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Transform/Unit/TransformFixture_TTransform_.TryResolveXsltPath(string).md#transformfixturetryresolvexsltpathstring-method
[transform-fixture]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Transforms/blob/master/src/Be.Stateless.BizTalk.Transform.Unit/Unit/Transform/TransformFixture.cs
[xsl-mapurl-resolver]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Xml/XslMapUrlResolver.md#xslmapurlresolver-class

<!--
cSpell:ignore CLSID msdia140 regsvr32 VSINSTALLDIR
-->
