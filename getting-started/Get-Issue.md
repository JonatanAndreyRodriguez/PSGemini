---
external help file: PSGemini-help.xml
online version: https://github.com/RD-Processa/PSGemini/blob/master/getting-started/Get-Issue.md
schema: 2.0.0
---

# Get-Issue

## SYNOPSIS
Obtiene la información de un requerimiento en el sistema Gemini.

## SYNTAX

### ById (Default)
```powershell
Get-Issue -Id <Int32>
```

### ByUserInfo
```powershell
Get-Issue [-InputObject <Object>] [-Expand]
```

## DESCRIPTION
Obtiene la información de un requerimiento en el sistema Gemini, adicionando sus campos personalizados y comentarios en el objeto de salida.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
Get-Issue -Id 12345
```

Obtiene la información del requerimiento asociado con el identificador 12345.

### -------------------------- EXAMPLE 2 --------------------------
```powershell
Get-Issue -Id 12345 | Select-Object -ExpandProperty Comment
```

Obtiene la información del requerimiento asociado con el identificador 12345 y luego "expande" sus comentarios.

### -------------------------- EXAMPLE 3 --------------------------
```powershell
Get-Issue -Id 12345 | Select-Object -ExpandProperty CustomField
```

Obtiene la información del requerimiento asociado con el identificador 12345 y luego "expande" sus campos personalizados.

### -------------------------- EXAMPLE 4 --------------------------
```powershell
Get-Issue -Id 12345 | Select-Object -ExpandProperty StatusIsFinal
```

Determinar si un requerimiento esta cerrado.

### -------------------------- EXAMPLE 5 --------------------------
```powershell
Get-Group -Name 'IT' | Get-User | Get-Issue
```

Obtiene la infomación de los requerimientos asignados a todos los usuarios del grupo 'IT'

## PARAMETERS

### -Id
Identificador del requerimiento en el sistema Gemini.

```yaml
Type: Int32
Parameter Sets: ById
Aliases: IssueId

Required: True
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Información de los usuarios para los que se obtienen los requerimientos asignados.

```yaml
Type: Object
Parameter Sets: ByUserInfo
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Expand
Cuando se establece, se obtiene la información completa y detallada de cada requerimiento.

```yaml
Type: SwitchParameter
Parameter Sets: ByUserInfo
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

Puede canalizar el valor de InputObject desde la función `Get-User`.

## OUTPUTS

Processa.Management.Automation.Gemini.IssueInfo

## NOTES
Autor: Atorres

## RELATED LINKS

[Get-User](Get-User.md)

[Get-Group](Get-Group.md)
