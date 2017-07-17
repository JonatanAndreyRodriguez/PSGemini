---
external help file: PSGemini-help.xml
online version: 
schema: 2.0.0
---

# Initialize-Session

## SYNOPSIS
Establece una conexión con el API de Gemini.

## SYNTAX

```
Initialize-Session [-InputObject] <Object>
```

## DESCRIPTION
Establece una conexión con el API de Gemini si no se ha establecido alguna, de lo contrario, utiliza la conexión existente.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
New-Credential | Initialize-Session
```

Conecta con el API de Gemini utilizando la información de credenciales en el archivo PSGemini.config

### -------------------------- EXAMPLE 2 --------------------------
```
New-Credential -ConnectionString 'url=http://processa6.ongemini.com;username=username;apikey=apikey' | Initialize-Session
```

Conecta con el API de Gemini utilizando la información de credenciales en el parámetro ConnectionString.

## PARAMETERS

### -InputObject
Información de credenciales para la conexión.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## INPUTS

### None

## OUTPUTS

### System.Void

## NOTES
Autor: Atorres

## RELATED LINKS

[[New-Credential](New-Credential.md)]()

