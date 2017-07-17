---
external help file: PSGemini-help.xml
online version: 
schema: 2.0.0
---

# Get-Project

## SYNOPSIS
Obtiene la lista de proyectos a los que tiene acceso el usuario que se utilizó en New-Credential.

## SYNTAX

```
Get-Project [[-InputObject] <Int32>]
```

## DESCRIPTION
Obtiene la lista de proyectos a los que tiene acceso el usuario que se utilizó en New-Credential.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Project
```

Obtiene la lista de todos los proyectos en el sistema Gemini.

## PARAMETERS

### -InputObject
Identificador del proyecto para el que se obtiene la información.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: 0
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## INPUTS

### None

## OUTPUTS

### Processa.Management.Automation.Gemini.ProjectInfo

## NOTES
Autor: Atorres

## RELATED LINKS

[New-Credential]()

