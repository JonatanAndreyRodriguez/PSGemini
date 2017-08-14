### [1.0.0] - 2017-jun-22 (Atorres)
- Versión inicial del módulo.

### [1.1] - 2017-jul-21
- Se agregó la función Get-IssueType

### [1.2] - 2017-ago-14
- Mejoras internas. Se ageraron sobrecargas y filtros en algunas funciones.
- Enhancement: Get-Issue ahora admite obtener los requerimientos de un grupo de usuarios.
- Breaking change: Se renombró el parámetro InputObject en Get-Issue por Id
- Enhancement: Get-User ahora solo muestra los usuarios activos. Si se desean todos los usuarios se debe utilizar el parámetro -Force
- Enhancement: Get-User ahora permite filtrar los usuarios de un grupo de usuarios a través del parámetro InputObject.
- Enhancement: Se agregó el filtro Name a la función Get-Group.
- Enhancement: Se agregó el filtro Name a la función Get-Project.
