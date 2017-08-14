---
external help file: PSGemini-help.xml
online version: 
schema: 2.0.0
---

# New-Credential

## SYNOPSIS
Obtiene la información de los datos de conexión con el API de Gemini.

## SYNTAX

```powershell
New-Credential [[-ConnectionString] <String>]
```

## DESCRIPTION
La cadena de conexión debe tener la forma url=value;username=value;apikey=value (claves en minúscula separados por punto y coma)

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
New-Credential
```

Utiliza los valores de conexión establecidos en el archico PSGemini.config.

### -------------------------- EXAMPLE 2 --------------------------
```powershell
New-Credential -ConnectionString 'url=http://processa6.ongemini.com;username=999999999;apikey=miapikey'
```

Utiliza los valores de conexión establecidos en ConnectionString

## PARAMETERS

### -ConnectionString
Cadena de conexión en formato url=value;username=value;apikey=value (claves en minúscula separados por punto y coma)

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## INPUTS

None

## OUTPUTS

Processa.Management.Automation.Gemini.Credential

## NOTES
Autor: Atorres

## RELATED LINKS

[Initialize-Session](Initialize-Session.md)

[Set-Configuration](Set-Configuration.md)

