
# 🔁 Actualización automática de Atenea

Este repositorio gestiona el sistema de actualizaciones automáticas de la aplicación **Atenea**.

Cada vez que se lanza una nueva versión del software, se actualiza un archivo `version.json` que contiene la versión más reciente disponible y un enlace al instalador correspondiente.


## 🛠️ ¿Cómo funciona?

Al iniciar la aplicación, esta consulta el archivo JSON para comprobar si hay una nueva versión. Si la versión disponible es mayor que la instalada localmente, el usuario podrá descargarla e instalarla automáticamente.


## 📄 Estructura del archivo `version.json`

```json
{
  "version": "1.0.0",
  "url": "https://github.com/grupoosg-it/Atenea-Setup/releases/download/v1.0.0/Atenea_Setup_v1.0.0.msi",
  "descripcion": "La nueva versión 1.0.0 trae..."
}
```
-   `version`: versión más reciente del software (formato semántico).
-   `url`: enlace directo al archivo `.msi` publicado en la sección de Releases del repositorio de instalación.


## 🌐 URL del archivo JSON

Este archivo está disponible públicamente gracias a **GitHub Pages**:

[`https://grupoosg-it.github.io/Atenea-Setup/version.json`](https://grupoosg-it.github.io/Atenea-Setup/version.json)

La aplicación WPF accede a esta URL para consultar automáticamente si hay nuevas versiones disponibles.


## ✅ Repositorio de instalación

Puedes encontrar los instaladores en la sección de [Releases](https://github.com/grupoosg-it/Atenea-Setup/releases).


## 🔒 Seguridad

Este sistema está pensado para distribuir actualizaciones a través de GitHub. No requiere autenticación porque el archivo `version.json` y los releases son públicos.

Para una solución privada o con control de acceso, se recomienda alojar el JSON e instaladores en un servidor propio o utilizar tokens de acceso.


## 💡 Créditos

Sistema de actualización desarrollado por el departamento de IT de **OSG - Operber Sitalu Group S. L.** Para más información, contacta con el autor.
