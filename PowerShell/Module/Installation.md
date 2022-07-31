# `PowerShell` Module Installation

Depending on the [execution policy][about_execution_policies] configuration level of your `PowerShell` &mdash;you can verify it with the [`Get-ExecutionPolicy`][get-executionpolicy] command,&mdash; you might have to trust the certificate that was used to sign the `BizTalk.Factory`'s `PowerShell` modules in order to install them right from the `PowerShell` Gallery.

Run the following `PowerShell` commands should the execution policy level be set to `RemoteSigned` &mdash;they merely download and install the certificate's public key in the `Trusted People` store underneath the `Local Machine` certificate store:

```PowerShell
Invoke-WebRequest -Uri https://github.com/icraftsoftware/Be.Stateless.Build.Scripts/raw/master/be.stateless.public.cer -OutFile "$($env:TEMP)\be.stateless.public.cer"

Import-Certificate -FilePath "$($env:TEMP)\be.stateless.public.cer" -CertStoreLocation Cert:\LocalMachine\TrustedPeople\
```

In addition to the previous ones, run the following `PowerShell` command should the execution policy level be set to `AllSigned` &mdash;it merely installs the certificate's public key in the `Trusted Publishers` store underneath the `Local Machine` certificate store:

```PowerShell
Import-Certificate -FilePath "$($env:TEMP)\be.stateless.public.cer" -CertStoreLocation Cert:\LocalMachine\TrustedPublisher\
```

> **Remark** You can delete the downloaded certificate's public key once you have successfully run the previous `PowerShell` commands:
>
> ```PowerShell
> Remove-Item -Path "$($env:TEMP)\be.stateless.public.cer"
> ```

<!-- links -->

[about_execution_policies]: https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies
[get-executionpolicy]: https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.security/get-executionpolicy
