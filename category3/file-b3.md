
---
sidebar_position: 1
title: '💈 How to Deploy'
description: 'How to leverage the zero-configuration feature for zero-effort deployments.'
slug: /usage/how-to-deploy
hide_title: true
tags:
  - Usage
  - How to Deploy
---

# How to Deploy

There are two ways to launch the PSAppDeployToolkit for deployment of applications.

- Launch ```Deploy-Application.ps1``` PowerShell script as administrator.

- Launch ```Deploy-Application.exe``` as administrator. This will launch the ```Deploy-Application.ps1``` PowerShell script without opening a PowerShell command window. Note, if the x86 PowerShell is required (for example, if CAPICOM or another x86 library is needed), launch `Deploy-Application.exe /32`.

Deploy an application for installation

```powershell
Deploy-Application.ps1
```

Deploy an application for uninstallation in silent mode

```powershell
Deploy-Application.ps1 -DeploymentType 'Uninstall' -DeployMode 'Silent'
```

Deploy an application for uninstallation using PowerShell x86, suppressing the PowerShell console window and deploying in silent mode.

```powershell
Deploy-Application.exe /32 -DeploymentType 'Uninstall' -DeployMode 'Silent'
```

Deploy an application for installation, suppressing the PowerShell console window and allowing reboot codes to be returned to the parent process.

```powershell
Deploy-Application.exe -AllowRebootPassThru
```

Deploy an application with a custom name instead of ```Deploy-Application.ps1```.

```powershell
Deploy-Application.exe 'Custom-Script.ps1'
```

Remove an application with a custom name and custom location for the script file.

```powershell
Deploy-Application.exe -Command 'C:\Testing\Custom-Script.ps1' -DeploymentType 'Uninstall'
```

#### Toolkit Parameters

The following parameters are accepted by ```Deploy-Application.ps1```:

##### -DeploymentType

Specify whether to install or uninstall the application.

```powershell
-DeploymentType 'Install' ## default
```

```powershell
-DeploymentType 'Uninstall'
```

##### -DeployMode

Specify the installation will be run in Interactive, Silent or NonInteractive mode:

- Interactive = Shows dialogs
- NonInteractive = Very silent, i.e. no blocking apps. This is automatically set if it is detected that the process is not running in the user session and it is not possible for anyone to provide input using a mouse or keyboard.
- Silent = No dialogs (progress and balloon tip notifications are suppressed)

```powershell
-DeployMode 'Interactive' ## default
```

```powershell
-DeployMode 'Silent'
```

```powershell
-DeployMode 'NonInteractive'
```

##### -AllowRebootPassthru

Specify whether to allow the 3010 exit code (reboot required) to be passed back to the parent process (e.g. MEMCM) if detected during an installation. If a 3010 code is passed to MEMCM, the MEMCM client will display a reboot prompt. If set to false, the 3010 return code will be replaced by a "0" (successful, no restart required).

```powershell
-AllowRebootPassThru $true ## default
```

```powershell
-AllowRebootPassThru $false
```

##### -TerminalServerMode

Changes to user install mode and back to user execute mode for installing/uninstalling applications on Remote Desktop Session Host/Citrix servers

```powershell
-TerminalServerMode $true ## default
```

```powershell
-TerminalServerMode $false
```

##### -DisableLogging

Disables logging to file for the script.

```powershell
-DisableLogging
```

This is a switch parameter, so setting this enables it. When not present, the default is false.
