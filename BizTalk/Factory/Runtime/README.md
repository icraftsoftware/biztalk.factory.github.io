# BizTalk.Factory Runtime

[![GitHub](https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Factory.Runtime&logo=github)](https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime)

[![Build Status](https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Factory.Runtime%20Manual%20Release?branchName=master)](https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=89&branchName=master)

[![Deployment Package](https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime?label=Be.Stateless.BizTalk.Factory.Runtime.Deployment.zip&style=flat&logo=github)](https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime/releases/latest/download/Be.Stateless.BizTalk.Factory.Runtime.Deployment.zip)

## Overview

BizTalk.Factory Runtime Package is part of the larger [BizTalk.Factory](./../../../README.md) SDK. This package is made of the following .NET assemblies:

- [Be.Stateless.Extensions] provides general purpose extension methods for various .NET types as well as code accelerators such as the [LambdaComparer](https://github.com/icraftsoftware/Be.Stateless.Extensions/blob/master/src/Be.Stateless.Extensions/Linq/LambdaComparer.cs) class. Most of the documentation for these classes and methods is provided as embedded XML comments and should be rather self explanatory;

- [Be.Stateless.Reflection] provides one [Reflector](https://github.com/icraftsoftware/Be.Stateless.Reflection/blob/master/src/Be.Stateless.Reflection/Reflection/Reflector.cs) helper class that eases the rare occasions on which you have no other choice than to invoke methods via reflection. No documentation is provided so far but its usage, though discouraged, should be rather self explanatory;

- [Be.Stateless.Security] mainly provides one [Delegate](https://github.com/icraftsoftware/Be.Stateless.Security/blob/master/src/Be.Stateless.Security/Delegate.cs) helper class that allows one to invoke a `delegate`, or lambda, on behalf of the specific Windows identity that corresponds to the one whose `username` and `password` are given as arguments.\
For the record, the only reason why and place where this class is used so far is to create a folder ahead of time in a Microsoft BizTalk Server® send pipeline thus allowing the File adapter to drop the message at the expected runtime-computed location, see [DirectoryCreator](https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/936a6130f8238a7e243829e97c923fa35a3feba3/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/DirectoryCreator.cs#L40);

- [Be.Stateless.Stream];

- [Be.Stateless.Xml];

- [Be.Stateless.BizTalk.Abstractions] provides basic but fundamental abstractions that support all of the other BizTalk.Factory assemblies;

- [Be.Stateless.BizTalk.Messaging];

- [Be.Stateless.BizTalk.Pipeline.MicroComponents];

- [Be.Stateless.BizTalk.ServiceModel];

- [Be.Stateless.BizTalk.Settings];

- [Be.Stateless.BizTalk.Stream];

- [Be.Stateless.BizTalk.Transform.ExtensionObjects];

- [Be.Stateless.BizTalk.XLang];

- [Be.Stateless.BizTalk.Xml].

<br/>

> **Remark** The assemblies being named **Be.Stateless.BizTalk.\*** are assemblies depending on and made up for Microsoft BizTalk Server® and currently target the .NET Framework 4.8. The other assemblies are not tied to Microsoft BizTalk Server® and currently target multiple frameworks: .NET Standard 2.0, .NET Core 3.1, and .NET Framework 4.8.

<!-- links -->
[Be.Stateless.Extensions]:https://github.com/icraftsoftware/Be.Stateless.Extensions
[Be.Stateless.Reflection]:https://github.com/icraftsoftware/Be.Stateless.Reflection
[Be.Stateless.Security]:https://github.com/icraftsoftware/Be.Stateless.Security
[Be.Stateless.Stream]:https://github.com/icraftsoftware/Be.Stateless.Stream
[Be.Stateless.Xml]:https://github.com/icraftsoftware/Be.Stateless.Xml
[Be.Stateless.BizTalk.Abstractions]:./../../Abstractions/README.md "Be.Stateless.BizTalk.Abstractions Component"
[Be.Stateless.BizTalk.Messaging]:https://github.com/icraftsoftware/Be.Stateless.BizTalk.Messaging
[Be.Stateless.BizTalk.Pipeline.MicroComponents]:https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents
[Be.Stateless.BizTalk.ServiceModel]:https://github.com/icraftsoftware/Be.Stateless.BizTalk.ServiceModel
[Be.Stateless.BizTalk.Settings]:https://github.com/icraftsoftware/Be.Stateless.BizTalk.Settings
[Be.Stateless.BizTalk.Stream]:https://github.com/icraftsoftware/Be.Stateless.BizTalk.Stream
[Be.Stateless.BizTalk.Transform.ExtensionObjects]:https://github.com/icraftsoftware/Be.Stateless.BizTalk.Transform.ExtensionObjects
[Be.Stateless.BizTalk.XLang]:https://github.com/icraftsoftware/Be.Stateless.BizTalk.XLang
[Be.Stateless.BizTalk.Xml]:https://github.com/icraftsoftware/Be.Stateless.BizTalk.Xml
