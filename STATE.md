# STATE.md

Estado del proyecto. Léalo al iniciar cada sesión de trabajo y actualícelo al cerrarla.

## Estado actual

Plantilla creada y desplegada. Página de inicio "https://plataforma-ludica-abcd.onrender.com"
, /salud y /docs en funcionamiento.
 Se agregó GET /api/version; devuelve la versión configurada en `app/proyecto.py` y cuenta con una prueba automatizada.

 ## Decisiones

 | Fecha | Decisión | Motivo |
 | 16 | Despliegue en Render vía Blueprint | Automatizar la integración continua desde GitHub  |
 | 16 | Reestructuración a la raíz | Permitir que Render detecte correctamente el build
 |
 | 2026-11-10 | Exponer GET /api/version con respuesta `{"version": ...}` | Consultar la versión de forma independiente, usando `proyecto.VERSION` como fuente única y validando el contrato con una prueba. |

 ## Siguiente paso

 Desplegar esta versión y comprobar GET /api/version en el entorno público.
