
---
id: Get-FreeDiskSpace
title: Get-FreeDiskSpace
description: Help page for the "Get-FreeDiskSpace" command
keywords:
  - PSAppDeployToolkit
  - PowerShell
  - Help
  - Documentation
hide_title: false
hide_table_of_contents: false
custom_edit_url: null
---

## SYNOPSIS

Retrieves the free disk space in MB on a particular drive (defaults to system drive)

## SYNTAX

```powershell
Get-FreeDiskSpace [[-Drive] <String>] [[-ContinueOnError] <Boolean>] [<CommonParameters>]
```

## DESCRIPTION

Retrieves the free disk space in MB on a particular drive (defaults to system drive)

## EXAMPLES

### EXAMPLE 1

```powershell
Get-FreeDiskSpace -Drive 'C:'
```

## PARAMETERS

### -Drive

Drive to check free disk space on

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: $envSystemDrive
Accept pipeline input: False
Accept wildcard characters: False
```

### -ContinueOnError

Continue if an error is encountered.
Default is: $true.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: True
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

### You cannot pipe objects to this function.
## OUTPUTS

### System.Double

### Returns the free disk space in MB
## NOTES

## RELATED LINKS

[https://psappdeploytoolkit.com](https://psappdeploytoolkit.com)
