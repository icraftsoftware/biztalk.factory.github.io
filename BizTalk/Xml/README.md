# Be.Stateless.BizTalk.Xml

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

`Be.Stateless.BizTalk.Xml` is part of the [BizTalk.Factory Runtime](./../../BizTalk/Factory/Runtime/README.md) Package. This component essentially is an `XML` class library for general purpose Microsoft BizTalk Server® development.

## Compiled `XSLT` Transforms on Steroids

Since its inception in the days of Microsoft BizTalk Server® 2009, `BizTalk.Factory` has always supported and encouraged the use of compiled `XSLT` transforms for obvious reasons. Even though Microsoft BizTalk Server® 2010 finally did the shift too, `BizTalk.Factory` kept its own `XslCompiledTransform`-wrapping `API` due the following two unique features:

- An `XSLT` stylesheet can combine multiple `XSLT` stylesheets via `xsl:import` or `xsl:include` top-level elements, see the dummy [CompoundMapTransform][dummy-compound-map-transform] for an example, or [XslMapUrlResolver][xsl-map-url-resolver] for some background information;

- An `XSLT` stylesheet that is executing in a pipeline can require access to the context of the message by simply declaring the distinguished `XML` [namespace][extension-object-namespaces-context] of the [MessageContext][base-message-context-functions] pseudo extension object, see the dummy [CompoundContextMapTransform][dummy-compound-context-map-transform] for an example, or [XslCompiledTransformDescriptor][xsl-compiled-transform-descriptor], [XslCompiledTransformDescriptorBuilder][xsl-compiled-transform-descriptor-builder], and [Transformer][transformer] for some background information.

Back in those days, even though it was made of a bunch of distinct assemblies, `BizTalk.Factory` 1.0 was both a giant monolithic repository and deployment package. With the advent of `BizTalk.Factory` 2.0, the monolith has been split into a bunch of repositories, individual deployment packages, and `PowerShell` modules &mdash; nearly 40 `GitHub` repositories, 4 deployment packages, 6 `PowerShell` modules, and nearly 60 `NuGet` packages. This is only relevant insofar as it is to be understood that currently the `XslCompiledTransform`-wrapping `API`, though rooted in `Be.Stateless.BizTalk.Xml`, is also spread across the following other repositories and `NuGet` packages:

- [`Be.Stateless.BizTalk.Stream`](../Stream/README.md), which sits on top of `Be.Stateless.BizTalk.Xml` to deliver all these features through a streaming `API`, see [Transformer][transformer];

- [`Be.Stateless.BizTalk.Pipeline.MicroComponents`](../Pipeline/MicroComponents/README.md), whose [`XsltRunner`][xslt-runner] component consumes the latter streaming `API`;

- [`Be.Stateless.BizTalk.XLang`](../XLang/README.md), whose [TransformHelper][transform-helper] ensures that composite `XSLT` stylesheets are supported while the [MessageContext][base-message-context-functions] pseudo extension object is not;

- [`Be.Stateless.BizTalk.Transforms`](../Transforms/README.md), and specifically the `Be.Stateless.BizTalk.Transform.Unit` `NuGet` package, which provides extended `XSLT` stylesheet debugging support, see [Debugging Composite Microsoft BizTalk Server® Maps with Extension Objects](../Transforms/README.md#debugging-composite-microsoft-biztalk-server®-maps-with-extension-objects).

### Accessing Message Context through `XSLT`

Accessing the context of the current message through `XSLT` requires that a different [MessageContext][base-message-context-functions] pseudo extension object be injected into the `XSLT` with each message. And that is why the [MessageContext][base-message-context-functions] is a **pseudo** extension object, because it is a mediator between the `XSLT` and the actual context of the message being transformed. Injecting the right pseudo extension object is the responsibility of the [Transformer][transformer] class.

As the dummy [CompoundContextMapTransform][dummy-compound-context-map-transform] illustrates, reading properties from the context of a message can be written in `XSLT` as simply as `ctx:Read('bf:EnvironmentTag')` where `ctx` and `Read` denote the pseudo extension object and its operation, and `bf` and `EnvironmentTag` the property schema &mdash;whose namespace has to be declared by the `XSLT`&mdash; and the property to get access to.

## Developer Help

Detailed developer help has been provided as `XML` comments directly embedded in source code. Though developers usually browse through this documentation while developing thanks to, for instance, JetBrains [ReSharper][resharper] quick help &mdash;<kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>F1</kbd>, an online version of this inlined help has also been provided here for greater reachability:

[![][help.badge]][help]

<!-- badges -->

[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Xml&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/BizTalk/Xml "Be.Stateless.BizTalk.Xml User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Xml&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Xml "Be.Stateless.BizTalk.Xml GitHub Repository"
[help.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Xml&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Xml/README.md "Be.Stateless.BizTalk.Xml Developer Help"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Xml.svg?label=Be.Stateless.BizTalk.Xml&style=flat&logo=nuget
[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Xml "Be.Stateless.BizTalk.Xml NuGet Package"
[nuget.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.BizTalk.Xml?logo=nuget
[nuget.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.BizTalk.Xml&protocolType=NuGet "Be.Stateless.BizTalk.Xml Preview NuGet Package"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Xml%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=41&branchName=master "Be.Stateless.BizTalk.Xml Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Xml%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=42&branchName=master "Be.Stateless.BizTalk.Xml Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Xml?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Xml/releases/latest "Be.Stateless.BizTalk.Xml GitHub Release"

<!-- links -->

[base-message-context-functions]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Xml/blob/4c66c44ba928d84a35d6be61ab2d06bdbd13d727/src/Be.Stateless.BizTalk.Xml/Message/ExtensionObjects/BaseMessageContextFunctions.cs
[dummy-compound-context-map-transform]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Xml/blob/4c66c44ba928d84a35d6be61ab2d06bdbd13d727/src/Be.Stateless.BizTalk.Xml.Tests/Dummies/Transform/CompoundContextMapTransform.cs#L29
[dummy-compound-map-transform]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Xml/blob/4c66c44ba928d84a35d6be61ab2d06bdbd13d727/src/Be.Stateless.BizTalk.Xml.Tests/Dummies/Transform/CompoundMapTransform.cs#L29
[extension-object-namespaces-context]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/Namespaces/ExtensionObjectNamespaces.cs#L38
[resharper]: https://www.jetbrains.com/resharper/
[transform-helper]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.XLang/blob/master/src/Be.Stateless.BizTalk.XLang/XLang/TransformHelper.cs#L213
[transformer]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Stream/blob/335606875a59fe84422f924c42d25281ade7365e/src/Be.Stateless.BizTalk.Stream/Stream/Extensions/Transformer.cs#L104
[xsl-compiled-transform-descriptor-builder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Xml/blob/4c66c44ba928d84a35d6be61ab2d06bdbd13d727/src/Be.Stateless.BizTalk.Xml/Xml/Xsl/XslCompiledTransformDescriptorBuilder.cs
[xsl-compiled-transform-descriptor]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Xml/blob/4c66c44ba928d84a35d6be61ab2d06bdbd13d727/src/Be.Stateless.BizTalk.Xml/Xml/Xsl/XslCompiledTransformDescriptor.cs
[xsl-map-url-resolver]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Xml/XslMapUrlResolver.md#xslmapurlresolver-class
[xslt-runner]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/XsltRunner.cs#L70

<!--
cSpell:ignore biztalk
-->
