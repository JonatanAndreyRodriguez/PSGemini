# ¿Cómo instalar el módulo PSGemini?

1. Abra una ventana de PowerShell como usuario administrador y registre el repositorio de Gerencia Técnica.

```
Register-PSRepository -Name 'Processa GT' -SourceLocation 'http://proget:8020/nuget/PowerShell' -InstallationPolicy Trusted
```

2. Instale el módulo desde el Repositorio

```
Install-Module -Name 'PSGemini' -Repository 'Processa GT' -AllowClobber
```

### RELATED LINKS

[Get-PSRepository](https://msdn.microsoft.com/en-us/powershell/reference/5.1/powershellget/get-psrepository)

[Register-PSRepository](https://msdn.microsoft.com/en-us/powershell/reference/5.0/powershellget/register-psrepository)

[Install-Module](https://msdn.microsoft.com/en-us/powershell/reference/5.1/powershellget/install-module)
