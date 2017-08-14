---
external help file: PSGemini-help.xml
online version: 
schema: 2.0.0
---

# Get-CustomField

## SYNOPSIS
Obtiene la información de los campos personalizados configurados para cada proyecto.

## SYNTAX

```powershell
Get-CustomField [-InputObject] <ProjectInfo>
```

## DESCRIPTION
Obtiene la información de los campos personalizados configurados para cada proyecto de acuerdo con la plantilla asignada al mismo.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
Get-Project | Get-CustomField
```

Obtiene los campos personalizados de todos los proyectos.

### -------------------------- EXAMPLE 2 --------------------------
```powershell
Get-Project -Id 44 | Get-CustomField
```

Obtiene los campos personalizados del proyecto con identificador 44.

### -------------------------- EXAMPLE 3 --------------------------
```powershell
Get-Project | Where-Object -Property Name -eq 'Mi nombre' | Get-CustomField
```

Obtiene los campos personalizados del proyecto con nombre 'Mi nombre'

## PARAMETERS

### -InputObject
Información de los proyectos para los que se obtienen los campos personalizados.

```yaml
Type: ProjectInfo
Parameter Sets: (All)
Aliases: ProjectId, Id

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

## INPUTS

Puede canalizar el valor de InputObject desde la función [Get-Project](Get-Project.md).

## OUTPUTS

Processa.Management.Automation.Gemini.CustomFieldInfo

## NOTES
Autor: Atorres

## RELATED LINKS

[Get-Project](Get-Project.md)

