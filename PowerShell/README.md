# COMMANDS FOR POWERSHELL WITH ADMINISTRATOR

## Bloatware on windows

### See some software on windows:
```shell
Get-AppxPackage | Select Name, PackageFullName;
```

### Remove a software:
```shell
Get-appxpackage -allusers *Software Name* | Remove-AppxPackage;
```

### Some commands to remove some bloatware and gain some time:
```shell
Get-appxpackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.LanguageExperiencePackes-MX  | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.WindowsMaps | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.YourPhone | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.WindowsAlarms | Remove-AppxPackage;
Get-AppxPackage -allusers Microsoft.People | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.GetHelp  | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.WindowsSoundRecorder | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.WebpImageExtension | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.Wallet | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.HEIFImageExtension | Remove-AppxPackage;
Get-appxpackage -allusers Microsoft.MicrosoftEdge.Stable | Remove-AppxPackage;
Get-appxpackage -allusers *xbox* | Remove-AppxPackage;
```

## Services on windows

### See services:
```shell
Get-service;
```

### Disable a service:
```shell
Set-service -Name *Service Name* -StartupType Disable;
```

### Here some commands to disable some unnecessary services and gain some time:
```shell
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
Set-service -Name MixedRealityOpenXRSvc -StartupType Disable;
Set-service -Name RemoteRegistry -StartupType Disable;
Set-service -Name RemoteAccess -StartupType Disable;
```

### more code (more code, more risk):
```shell
Set-service -Name Spooler -StartupType Disable;
Set-service -Name BluetoothUserService_374bc -StartupType Disable;
Set-service -Name PimIndexMaintenanceSvc_374bc -StartupType Disable;
Set-service -Name BcastDVRUserService_374bc -StartupType Disable;
Set-service -Name PrintWorkflowUserSvc_374bc -StartupType Disable;
```

#### (some services are necesary for some programs, like Work Station (LanmanWorkstation) for Ryzen Master, if you have any issues, try to start the service you need in the services aplication, if you need it permanently started set it automatic).

#### Possible errors found:

* Ryzen masters requires Work Station (LanmanWorkstation)
* Desktop search for files and folders needs Windows Search (WSearch), but explorer search no need it

## bcdedit

### Platform configurations:
```shell
bcdedit /set useplatformtick yes;
bcdedit /set disabledynamictick yes;
bcdedit /set useplatformclock no;
```

### some extra if you don't use hypervisor:
```shell
bcdedit /set hypervisorlaunchtype Off;
```

## Task Scheduler

#### It depends on many factors, you can have different types of scheduled tasks, such as automatic program updates, custom rgb, etc. These tasks would have to be seen in each particular case for various reasons.

### In this case disables telemetry and some microsoft things:
```shell
Disable-ScheduledTask -TaskPath "\Microsoft\Windows\Application Experience" -TaskName "Microsoft Compatibility Appraiser";
Disable-ScheduledTask -TaskPath "\Microsoft\Windows\Application Experience" -TaskName "ProgramDataUpdater";
Disable-ScheduledTask -TaskPath "\Microsoft\Windows\Application Experience" -TaskName "StartupAppTask";
Disable-ScheduledTask -TaskPath "\Microsoft\Windows\Customer Experience Improvement Program" -TaskName "Consolidator";
Disable-ScheduledTask -TaskPath "\Microsoft\Windows\Customer Experience Improvement Program" -TaskName "UsbCeip";
Disable-ScheduledTask -TaskPath "\Microsoft\Windows\Offline Files" -TaskName "Background Synchronization";
Disable-ScheduledTask -TaskPath "\Microsoft\Windows\Offline Files" -TaskName "Logon Synchronization";
```

## Power plan ultimate perfomance

### After you run this command, set this power plan on in power options:
```shell
powercfg -duplicatescheme e9a42b02-d5df-448d-aa00-03f14749eb61;
```
