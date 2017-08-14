---
external help file: PSGemini-help.xml
online version: 
schema: 2.0.0
---

# New-CustomFieldData

## SYNOPSIS
Crea un objeto que representa la información del valor de un campo personalizado en el sistema Gemini.

## SYNTAX

```powershell
New-CustomFieldData [-Id] <Int32> [-Value] <String> [[-UserId] <Int32>]
```

## DESCRIPTION
Crea un objeto que representa la información del valor de un campo personalizado en un requerimiento en el sistema Gemini.
En el API de Gemini se representa con una instancia
de un objeto de tipo Countersoft.Gemini.Commons.Entity.CustomFieldData.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
New-CustomFieldData -Id 20 -Value 'Mi valor'
```

Establece el valor del campo personalizado con el identificador 20 al texto 'Mi valor'

### -------------------------- EXAMPLE 2 --------------------------
```powershell
New-CustomFieldData -Id 20 -Value 'Mi valor' -UserId 2
```

Establece el valor del campo personalizado con el identificador 20 al texto 'Mi valor', asociando al usuario con el identificador 2 como "publicante" del valor del campo.

### -------------------------- EXAMPLE 3 --------------------------
```powershell
$CustomFieldId = Get-Project 46 | Get-CustomField | Where-Object -Property CustomFieldName -eq 'EpicorJobNum' | Select-Object -ExpandProperty CustomFieldId
New-CustomFieldData -Id $CustomFieldId -Value 'Mi valor'
```

Establece el valor del campo personalizado con nombre 'EpicorJobNum' en el proyecto 46, al valor 'Mi texto'

## PARAMETERS

### -Id
Identificador del campo personalizado en el sistema.
Puede obtener este valor utilizando la función Get-CustomField.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Value
Valor que se desea asignar al campo personalizado en el requerimiento.

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

### -UserId
Identificador del usuario que establece el valor del campo personalizadp.
Por defecto se utiliza el valor configurado en el archivo PSGemini.config.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: -1
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

None

## OUTPUTS

Processa.Management.Automation.Gemini.CustomFieldDataInfo

## NOTES
Autor: Atorres

## RELATED LINKS

[Get-CustomField](Get-CustomField.md)

[New-Issue](New-Issue.md)

