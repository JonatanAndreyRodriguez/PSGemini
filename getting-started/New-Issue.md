---
external help file: PSGemini-help.xml
online version: 
schema: 2.0.0
---

# New-Issue

## SYNOPSIS
Registra un nuevo requerimiento en el sistema Gemini.

## SYNTAX

```
New-Issue [-InputObject] <PSObject> [[-CustomField] <CustomFieldDataInfo[]>]
```

## DESCRIPTION
Puede establecer los valores de las propiedades que desea inicializar en el requerimiento.
Para obtener la lista de propiedades que se pueden inicializar utilice la función Get-AvailabilityField.

> Puede utilizar el parámetro InformationVariable para obtener la información de los campos personalizados creados o de posibles errores generados al guardar.

## EXAMPLES

### -------------------------- REQUERIMIENTO SIMPLE --------------------------
```
@{Title='Lorem Ipsum'; ProjectId = 46; Description='Lorem'; ReportedBy = 11} | New-Issue
```
Crea un requerimiento con los campos especificados.

### ---------------- REQUERIMIENTO CON CAMPOS PERSONALIZADOS ----------------
```
$ReqData = @{Title='Lorem Ipsum'; ProjectId = 46; Description='Lorem'; ReportedBy = 11}
$CustomField = @(New-CustomFieldData -Id 207 -Value 'test value')
$ReqData | New-Issue -CustomField $CustomField -InformationVariable AdditionalInfo
$AdditionalInfo | Where-Object -Property Tags -Match 'Error' | Select-Object -ExpandProperty MessageData
$AdditionalInfo | Where-Object -Property Tags -Match 'CustomField' | Select-Object -ExpandProperty MessageData
```
Crea un requerimiento con los campos especificados y agrega el campo personalizado 207. 

:ballot_box_with_check: Puede utilizar el parámetro InformationVariable para obtener la información de los campos personalizados creados o de posibles errores generados al guardar.

## PARAMETERS

### -InputObject
Objeto con las propiedades que se deben establecer en el requerimiento.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CustomField
Array con la lista de campos personaliados que se deben asociar con el requerimiento.

```yaml
Type: Processa.Management.Automation.Gemini.CustomFieldDataInfo
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

Puede canalizar el valor de InputObject.

## OUTPUTS
System.Int32 con el identificador del requerimiento que se creó.


## NOTES
Autor: Atorres


## RELATED LINKS

[Get-AvailabilityField](Get-AvailabilityField.md)

[New-CustomFieldData](New-CustomFieldData.md)

