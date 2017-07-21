---
external help file: PSGemini-help.xml
online version: https://github.com/RD-Processa/PSGemini/blob/master/getting-started/Get-Issue.md
schema: 2.0.0
---

# Get-IssueType

## SYNOPSIS
Obtiene la información de los tipos de requerimientos configurados para cada proyecto.

## SYNTAX

```
Get-IssueType [-InputObject] <Object>
```

## DESCRIPTION
Obtiene la información de los tipos de requerimientos configurados para cada proyecto, de acuerdo con la plantilla asignada al mismo.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Project -InputObject 46 | Get-IssueType
```

Obtene la información de los tipos de requerimientos para el proyecto con el código 46.

### -------------------------- EXAMPLE 2 --------------------------
```
Get-Project | Get-IssueType
```

Obtene la información de los tipos de requerimientos para todos los proyectos.

## PARAMETERS

### -InputObject
Información de los proyectos para los que se obtienen los tipos de requerimientos.

```yaml
Type: Object
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

System.Management.Automation.PSObject

## NOTES
Autor: Atorres

## RELATED LINKS

