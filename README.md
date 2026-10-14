# GeoInstituciones Colombia

Visor web para explorar instituciones en un mapa de Colombia. La interfaz compilada incluye búsqueda de lugares, consulta de detalles, rutas y herramientas de análisis espacial.

## Funciones presentes en la interfaz

- Búsqueda y selección de instituciones.
- Visualización de lugares y rutas en el mapa.
- Herramientas de buffer, centroide, proximidad y medición.
- Figuras dibujadas y mapa de intensidad.
- Formularios de acceso, registro y programación de visitas.

Estas funciones dependen de los servicios que utiliza la aplicación; servir los archivos estáticos no garantiza disponer de todas ellas.

## Contenido de este repositorio

Actualmente se versionan el frontend compilado en `frontend/dist/` y una carpeta de dependencias en `frontend/node_modules/`.

**No se incluyen el código fuente de la aplicación, un manifiesto `package.json` propio ni el backend.** Por ese motivo, este repositorio permite inspeccionar y servir el artefacto existente, pero no reproducir su compilación ni preparar un entorno completo de desarrollo.

## Vista previa local

Con Python instalado, ejecuta desde la raíz:

```bash
python -m http.server 8080 --directory frontend/dist
```

Abre `http://localhost:8080`. Los recursos de mapa, consultas y acciones que dependen de una API necesitan que los servicios correspondientes estén disponibles.

## Estructura

| Ruta | Contenido |
| --- | --- |
| `frontend/dist/index.html` | Entrada del sitio compilado |
| `frontend/dist/assets/` | JavaScript, estilos y recursos compilados |
| `frontend/node_modules/` | Dependencias versionadas |

## Para continuar el desarrollo

Incorpora el código fuente, el manifiesto y archivo de bloqueo de dependencias, la configuración del backend y un ejemplo de variables de entorno sin credenciales. Con esos archivos será posible documentar una instalación y compilación reproducibles.
