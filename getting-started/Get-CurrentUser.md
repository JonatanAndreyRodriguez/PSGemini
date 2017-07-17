---
external help file: PSGemini-help.xml
online version: 
schema: 2.0.0
---

# Get-CurrentUser

## SYNOPSIS
Obtiene la información del usuario utilizado para conectar con el API de Gemini.

## SYNTAX

```
Get-CurrentUser
```

## DESCRIPTION
Obtiene la información del usuario utilizado para conectar con el API de Gemini.
Puede ser el usuario en el archivo PSGemini.config
o el utilizado en la función New-Credential (si se especificó alguno).

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
New-Credential | Initialize-Session
```

Get-CurrentUser

## PARAMETERS

## INPUTS

### None

## OUTPUTS

### System.Object

## NOTES
Autor: Atorres

## RELATED LINKS

[[New-Credential](New-Credential.md)]()

[[Initialize-Session](Initialize-Session.md)]()

