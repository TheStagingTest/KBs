---
id: Get-FileVersion
title: Get-FileVersion
description: Help page for the "Get-FileVersion" command
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

Gets the version of the specified file

## SYNTAX

```powershell
Get-FileVersion [-File] <String> [-ProductVersion] [[-ContinueOnError] <Boolean>] [<CommonParameters>]
```

## DESCRIPTION

Gets the version of the specified file

## EXAMPLES

### EXAMPLE 1

```powershell
Get-FileVersion -File "$envProgramFilesX86\Adobe\Reader 11.0\Reader\AcroRd32.exe"
```

## PARAMETERS

### -File

Path of the file

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProductVersion

Switch that makes the command return ProductVersion instead of FileVersion

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
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

### System.String

### Returns the version of the specified file.
## NOTES

## RELATED LINKS

[https://psappdeploytoolkit.com](https://psappdeploytoolkit.com)
