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
Get-User [[-InputObject] <Object>] [-Force]
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

### -------------------------- EXAMPLE 2 --------------------------
```powershell
New-Credential | Initialize-Session
Get-User -Force
```

Obtiene la lista de todos los usuarios registrados.

### -------------------------- EXAMPLE 3 --------------------------
```powershell
Get-Group -Name 'IT' | Get-User
```

Obtiene la lista de usuarios en el grupo 'IT'

## PARAMETERS
### -InputObject
Establece los grupos de usuarios para los que se obtiene la información.

### -Force
Cuando se establece, se obtiene la lista de todos los usuarios, incluidos los deshabilitados y los marcados para eliminar.


## INPUTS
Puede canalizar el valor de InputObject desde la función `Get-Group` para filtrar solo los usuarios de uno o más grupos.

## OUTPUTS

Processa.Management.Automation.Gemini.UserInfo

## NOTES
Autor: Atorres

## RELATED LINKS

[Get-Project](Get-Project.md)

[Get-Group](Get-Group.md)
