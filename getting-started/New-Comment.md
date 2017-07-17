---
external help file: PSGemini-help.xml
online version: 
schema: 2.0.0
---

# New-Comment

## SYNOPSIS
Agrega un comentario a un requerimiento.

## SYNTAX

```
New-Comment [-IssueId] <Int32> [-Text] <String> [[-UserId] <Int32>]
```

## DESCRIPTION
Agrega un comentario a un requerimiento estableciendo el usuario en UserId como el "publicador".

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
New-Comment -IssueId 12345 -Text 'Lorem Ipsum'
```

Crea un comentario con el texto 'Lorem Ipsum' en el requerimiento 12345.

### -------------------------- EXAMPLE 2 --------------------------
```
New-Comment -IssueId 12345 -Text 'Lorem Ipsum' -IsuerId 1
```

Crea un comentario con el texto 'Lorem Ipsum' en el requerimiento 12345, y establece como "publicador" al usuario con identificador 1.

## PARAMETERS

### -IssueId
Identificador del requerimiento en el sistema Gemini.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: Id

Required: True
Position: 1
Default value: 0
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Text
Texto del comentario.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Comment

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UserId
Identificador del usuario que agrega el comentario.
Si no se establece se utiliza el valor configurado en el archivo PSGemini.config.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: User

Required: False
Position: 3
Default value: -1
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

### None

## OUTPUTS

### System.Void

## NOTES
Autor: Atorres

## RELATED LINKS

[[New-Issue](New-Issue.md)]()

