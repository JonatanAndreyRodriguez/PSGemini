## ¿Cómo funciona?

Antes de utilizar alguna de las funciones del módulo debe establecer la configuración e iniciar una conexión con el sistema remoto:

### 1. Conectar con Gemini
---

* [Establecer los valores de conexión](Set-Configuration.md)
* [Iniciar una conexión](Initialize-Session.md)

```
Import-Module PSGemini
New-Credential | Initialize-Session
```

### 2. Interactuar con Gemini
---

* [Obtener la información de los usuarios](Get-User.md)
* [Obtener la información de los grupos de usuarios](Get-Group.md)
* [Obtener la información de los proyectos](Get-Project.md)
* [Obtener la información de los campos personalizados por proyecto](Get-CustomField.md)
* [Obtener la información de un requerimiento](Get-Issue.md)
* [Obtener la información de los tipos de requerimiento por proyecto](Get-IssueType.md)

### 3. Agregar un requerimiento
---

* [Agregar un requerimiento simple](New-Issue.md)
* Agregar un requerimiento con campos personalizados
    * [Obtener la lista de campos que se pueden utlizar al crear un requerimiento](Get-AvailabilityField.md)
    * [Obtener la información de los campos personalizados por proyecto](Get-CustomField.md)
    * [Inicializar un campo personalizado](New-CustomFieldData.md)    
* [Agregar un comentario a un requerimiento](New-Comment.md)


