---
external help file: PSGemini-help.xml
online version: 
schema: 2.0.0
---

# Get-User

## SYNOPSIS
Obtiene la lista de usuarios registrados en el sistema Gemini.

## SYNTAX

```powershell
Get-User
```

## DESCRIPTION
Obtiene la lista de usuarios registrados en el sistema Gemini.
Los usuarios se administran desde la UI de Gemini bajo la opción Customize \>\> People \>\> Users.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```powershell
New-Credential | Initialize-Session
Get-User
```

Obtiene la lista de todos los usuarios registrados.

## PARAMETERS

## INPUTS
None

## OUTPUTS

Processa.Management.Automation.Gemini.UserInfo

## NOTES
Autor: Atorres

## RELATED LINKS

[Get-Project](Get-Project.md)

