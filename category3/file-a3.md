---
id: Get-IniValue
title: Get-IniValue
description: Help page for the "Get-IniValue" command
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

Parses an INI file and returns the value of the specified section and key.

## SYNTAX

```powershell
Get-IniValue [-FilePath] <String> [-Section] <String> [-Key] <String> [[-ContinueOnError] <Boolean>]
 [<CommonParameters>]
```

## DESCRIPTION

Parses an INI file and returns the value of the specified section and key.

## EXAMPLES

### EXAMPLE 1

```powershell
Get-IniValue -FilePath "$envProgramFilesX86\IBM\Notes\notes.ini" -Section 'Notes' -Key 'KeyFileName'
```

## PARAMETERS

### -FilePath

Path to the INI file.

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

### -Section

Section within the INI file.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Key

Key within the section of the INI file.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
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
Position: 4
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

### Returns the value of the specified section and key.
## NOTES

## RELATED LINKS

[https://psappdeploytoolkit.com](https://psappdeploytoolkit.com)

