# Enabling PowerShell Remoting Locally

Enabling `PowerShell` remoting locally is not necessarily trivial. There are numerous documents that explain how to do it across different machines, but very few, if any, that explain how to do it on the same machine. `BizTalk.Factory` suggests the following set of commands, which have been validated to successfully enable `PowerShell` remoting on a local machine, whether it is being part or not of a domain:

```PowerShell
Enable-PSRemoting
Add-LocalGroupMember -Group 'Remote Management Users' -Member "$env:USERDOMAIN\$env:USERNAME"

Set-Item -Path WSMan:\localhost\Client\AllowUnencrypted -Value false
Set-Item -Path WSMan:\localhost\Client\Auth\Certificate -Value true

Set-Item -Path WSMan:\localhost\Service\AllowUnencrypted -Value false
Set-Item -Path WSMan:\localhost\Service\Auth\Certificate -Value true

$cert = New-SelfSignedCertificate -CertStoreLocation Cert:\LocalMachine\My -DnsName $env:COMPUTERNAME
Export-Certificate -Cert $cert -FilePath "$($env:TEMP)\$($env:COMPUTERNAME).sst"
Import-Certificate -FilePath "$($env:TEMP)\$($env:COMPUTERNAME).sst" -CertStoreLocation Cert:\LocalMachine\Root

Get-ChildItem WSMan:\localhost\listener | Where-Object -Property Keys -eq 'Transport=HTTP' | Remove-Item -Recurse

New-Item -Path WSMan:\localhost\Listener -Transport HTTPS -Address * -CertificateThumbPrint $cert.Thumbprint –Force
Disable-NetFirewallRule -DisplayName 'Windows Remote Management (HTTP-In)'

Remove-Item -Path "$($env:TEMP)\$($env:COMPUTERNAME).sst"
```

If successfully enabled, then the following two commands must succeed:

```PowerShell
> Test-WSMan -ComputerName $env:COMPUTERNAME -UseSSL

wsmid           : http://schemas.dmtf.org/wbem/wsman/identity/1/wsmanidentity.xsd
ProtocolVersion : http://schemas.dmtf.org/wbem/wsman/1/wsman.xsd
ProductVendor   : Microsoft Corporation
ProductVersion  : OS: 0.0.0 SP: 0.0 Stack: 3.0

> Invoke-Command -ComputerName $env:COMPUTERNAME -UseSSL -ScriptBlock { $true }
True
```

<!--
cSpell:ignore Unencrypted USERDOMAIN wsmid
-->
