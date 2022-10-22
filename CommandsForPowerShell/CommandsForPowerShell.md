# UwU's

###### This commands are for windows 10 powershell with administrator

# Software on windows

### See some software on windows

```txt
Get-AppxPackage | Select Name, PackageFullName;
```

### To remove a software

```txt
Get-appxpackage -allusers *Software Name* | Remove-AppxPackage;
```

### Some commands to remove some unnecessary software and gain some time

```txt
Get-appxpackage -allusers Microsoft.XboxGamingOverlay | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.LanguageExperiencePackes-MX  | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.XboxIdentityProvider | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.WindowsMaps | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.YourPhone | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.WindowsAlarms | Remove-AppxPackage;
Get-AppxPackage -allusers Microsoft.People | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.XboxGameOverlay  | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.XboxGamingOverlay  | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.XboxSpeechToTextOverlay  | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.GetHelp  | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.WindowsSoundRecorder | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.WebpImageExtension | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.Wallet | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.HEIFImageExtension | Remove-AppxPackage;
```


# Services on windows

### See services

```txt
Get-service;
```

### Disable some service

```txt
Set-service -Name *Service Name* -StartupType Disable;
```

### Some commands to disable some unnecessary services and gain some time

```txt
Set-service -Name DiagTrack -StartupType Disable;
set-service -Name WSearch -StartupType Disable;
Set-service -Name MapsBroker -StartupType Disable;
Set-service -Name lmhosts -StartupType Disable;
Set-service -Name NaturalAuthentication -StartupType Disable;
Set-service -Name PeerDistSvc -StartupType Disable;
Set-service -Name SNMPTRAP -StartupType Disable;
Set-service -Name LanmanWorkstation -StartupType Disable;
Set-service -Name Fax -StartupType Disable;
Set-service -Name autotimesvc -StartupType Disable;
Set-service -Name dmwappushservice -StartupType Disable;
Set-service -Name XboxGipSvc -StartupType Disable;
Set-service -Name WalletService -StartupType Disable;
Set-service -Name TapiSrv -StartupType Disable;
Set-service -Name SysMain -StartupType Disable;
Set-service -Name PhoneSvc -StartupType Disable;
Set-service -Name FrameServer -StartupType Disable;
Set-service -Name SmsRouter -StartupType Disable;
Set-service -Name wisvc -StartupType Disable;
Set-service -Name WMPNetworkSvc -StartupType Disable;
Set-service -Name TroubleshootingSvc -StartupType Disable;
Set-service -Name icssvc -StartupType Disable;
Set-service -Name XboxNetApiSvc -StartupType Disable;
Set-service -Name RetailDemo -StartupType Disable;
Set-service -Name lfsvc -StartupType Disable;
Set-service -Name LxpSvc -StartupType Disable;
Set-service -Name DPS -StartupType Disable;
Set-service -Name WpcMonSvc -StartupType Disable;
Set-service -Name WbioSrvc -StartupType Disable;
Set-service -Name wcncsvc -StartupType Disable;
Set-service -Name SEMgrSvc -StartupType Disable;
Set-service -Name CscService -StartupType Disable;
Set-service -Name Netlogon -StartupType Disable;
Set-service -Name XblGameSave -StartupType Disable;
Set-service -Name WdiServiceHost -StartupType Disable;
Set-service -Name WdiSystemHost -StartupType Disable;
Set-service -Name XblAuthManager -StartupType Disable;
```
