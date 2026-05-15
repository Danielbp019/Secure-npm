# secure-npm.ps1

Script de PowerShell para aplicar configuraciones de seguridad recomendadas en `npm` de forma automática y segura.

El script:

- Crea `~/.npmrc` si no existe
- Reemplaza configuraciones existentes
- Evita líneas duplicadas
- Conserva configuraciones no relacionadas
- Agrega opciones faltantes automáticamente

# Objetivo

Este proyecto busca endurecer la configuración de `npm` para reducir riesgos comunes relacionados con:

- Dependencias maliciosas
- Versiones cambiantes inesperadas
- Ejecución automática de scripts durante instalación
- Publicación prematura de paquetes potencialmente inseguros

# Configuraciones aplicadas

El script configura las siguientes opciones:

```ini
save-exact=true
ignore-scripts=true
min-release-age=7
```
