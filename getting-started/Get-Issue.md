---
external help file: PSGemini-help.xml
online version: 
schema: 2.0.0
---

# Get-Issue

## SYNOPSIS
Obtiene la información de un requerimiento en el sistema Gemini.

## SYNTAX

```
Get-Issue [-InputObject] <Int32>
```

## DESCRIPTION
Obtiene la información de un requerimiento en el sistema Gemini, adicionando sus campos personalizados y comentarios en el objeto de salida.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Issue -InputObject 12345
```

Obtiene la información del requerimiento asociado con el identificador 12345.

### -------------------------- EXAMPLE 2 --------------------------
```
Get-Issue -InputObject 12345 | Select-Object -ExpandProperty Comment
```

Obtiene la información del requerimiento asociado con el identificador 12345 y luego "expande" sus comentarios.

### -------------------------- EXAMPLE 3 --------------------------
```
Get-Issue -InputObject 12345 | Select-Object -ExpandProperty CustomField
```

Obtiene la información del requerimiento asociado con el identificador 12345 y luego "expande" sus campos personalizados.


## PARAMETERS

### -InputObject
Identificador del requerimiento en el sistema Gemini.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: IssueId, Id

Required: True
Position: 1
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

None

## OUTPUTS

Processa.Management.Automation.Gemini.IssueInfo

## NOTES
Autor: Atorres

## RELATED LINKS

