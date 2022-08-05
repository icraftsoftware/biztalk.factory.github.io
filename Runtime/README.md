# Be.Stateless.Runtime

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

`Be.Stateless.Runtime` is part of the [BizTalk.Factory Runtime](./../BizTalk/Factory/Runtime/README.md) Package. This component provides service injection at the startup of any .NET Framework managed process and caching abstractions.

## Service Injection

Service injection relies on the [StartupServiceManager][startup-service-manager] class, which technically is a configurable [AppDomainManager][app-domain-manager] that injects services at the startup of any .NET Framework managed process, thus allowing any custom infrastructure code to be executed before any other managed code run &mdash;the `StartupServiceManager` injects services whenever an [AppDomain][app-domain] is created. To enable the `StartupServiceManager` for a .NET Framework process, one has to register it as an [AppDomainManager][app-domain-manager-assembly] in the `XML` configuration file of the process, as follows:

```xml
<configuration>
  ...
  <runtime>
    ...
    <appDomainManagerAssembly value="Be.Stateless.Runtime, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14" />
    <appDomainManagerType value="Be.Stateless.Runtime.StartupServiceManager" />
    ...
  </runtime>
    ...
</configuration>
```

The `StartupServiceManager` has its own `XML` configuration section, which must be declared as follows &mdash;notice that its important to respect the nesting of the `XML` elements, namely `be.stateless\runtime\startup`, or the `StartupServiceManager` will not be able to load its configuration:

```xml
<configuration>
  <configSections>
    ...
    <sectionGroup name="be.stateless">
      <sectionGroup name="runtime">
        <section name="startup"
                 type="Be.Stateless.Runtime.Configuration.StartupServiceManagerConfigurationSection, Be.Stateless.Runtime, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14" />
      </sectionGroup>
    </sectionGroup>
    ...
  </configSections>

  ...

</configuration>
```

Once loaded by the CLR, `StartupServiceManager` will immediately load its configuration to determine the services that need to be injected every time an `AppDomain` is created. To be successfully injected, a service must implement the [IStartupService][i-startup-service] interface; failure to do so will generate runtime errors that will be reported as Windows Event Logs. The following `XML` configuration excerpt demonstrates how to declare such a service.

```xml
<configuration>

  ...

  <be.stateless>
    <runtime>
      <startup>
        <services>
          <service type="Be.Stateless.BizTalk.Factory.Logging.LoggingConfigurationLoader, Be.Stateless.BizTalk.Factory.Logging, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14" />
        </services>
      </startup>
    </runtime>
  </be.stateless>

  ...

</configuration>
```

> **Remark** By injecting a [LoggingConfigurationLoader][logging-configuration-loader] startup service in `BTSNTSvc[64].exe` processes, the `BizTalk.Factory` runtime ensures that `log4net` has loaded its configuration before any attempt to create a `logger` is made.

## Caching Abstractions

Caching abstractions provide both absolute and sliding expiration caches that are used pervasively in `BizTalk.Factory` to cache things like schema metadata, compiled `XSLT`s, compiled regular expressions, and so on...

## Developer Help

Detailed developer help has been provided as `XML` comments directly embedded in source code. Though developers usually browse through this documentation while developing thanks to, for instance, JetBrains [ReSharper][resharper] quick help &mdash;<kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>F1</kbd>, an online version of this inlined help has also been provided here for greater reachability:

[![][help.badge]][help]

<!-- badges -->

[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=Be.Stateless.Runtime&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/Runtime "Be.Stateless.Runtime User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.Runtime&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.Runtime "Be.Stateless.Runtime GitHub Repository"
[help.badge]: https://img.shields.io/static/v1?label=Be.Stateless.Runtime&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/Runtime/README.md "Be.Stateless.Runtime Developer Help"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.Runtime.svg?label=Be.Stateless.Runtime&style=flat&logo=nuget
[nuget]: https://www.nuget.org/packages/Be.Stateless.Runtime "Be.Stateless.Runtime NuGet Package"
[nuget.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.Runtime?logo=nuget
[nuget.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.Runtime&protocolType=NuGet "Be.Stateless.Runtime Preview NuGet Package"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.Runtime%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=97&branchName=master "Be.Stateless.Runtime Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.Runtime%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=98&branchName=master "Be.Stateless.Runtime Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.Runtime?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.Runtime/releases/latest "Be.Stateless.Runtime GitHub Release"

<!-- links -->

[app-domain-manager-assembly]: https://docs.microsoft.com/en-us/dotnet/framework/configure-apps/file-schema/runtime/appdomainmanagerassembly-element
[app-domain-manager]: https://docs.microsoft.com/en-us/dotnet/api/system.appdomainmanager
[app-domain]: https://docs.microsoft.com/en-us/dotnet/api/system.appdomain
[i-startup-service]: https://github.com/icraftsoftware/Be.Stateless.Runtime/blob/master/src/Be.Stateless.Runtime/Runtime/IStartupService.cs
[logging-configuration-loader]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime/blob/master/src/Be.Stateless.BizTalk.Factory.Logging/Factory/Logging/LoggingConfigurationLoader.cs
[resharper]: https://www.jetbrains.com/resharper/
[startup-service-manager]: https://github.com/icraftsoftware/Be.Stateless.Runtime/blob/master/src/Be.Stateless.Runtime/Runtime/StartupServiceManager.cs

<!--
cSpell:ignore BTSNTSvc
-->
