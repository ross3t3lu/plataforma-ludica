
# AGENTS.md

Instrucciones para agentes OpenCode en este repositorio. Léalo antes de cambiar código.

## Proyecto
Plataforma web lúdica de cursos para niños con FastAPI. Roles: docente y niño; el niño entra con código de clase y avatar, sin correo. Los datos del proyecto viven en `app/proyecto.py`.
Plataforma web lúdica de cursos para niños. Curso: Ciencias. Mecánica: Estrellas. Roles: docente y niño. El niño entra con código de clase y avatar, sin correo.

## Stack y estructura
- Python >=3.11, FastAPI, Jinja2 y SQLModel.
- SQLite en desarrollo y PostgreSQL al publicar.
- Entrada principal: `app/main.py`.
- Rutas HTML: `app/rutas/paginas.py`; API: `app/rutas/api.py`.
- Reglas de negocio: `app/servicios/`; modelos: `app/modelos/`.
- Plantillas y archivos estáticos: `app/templates/` y `app/static/`.
- Pruebas: `tests/`; aceptación: `tests/aceptacion/`.

## Comandos
- Instalar: `python -m pip install -r requirements-dev.txt`.
- Ejecutar: `uvicorn app.main:app --reload`.
- Pruebas: `python -m pytest -v`.
- Estilo: `ruff check .`.
- PDF: `python entregar.py N`.
- Salud: abrir `http://127.0.0.1:8000/salud`.

## Reglas de trabajo
- Escriba en español y use nombres claros.
- Haga cambios pequeños y pruebe antes de entregar.
- Lea `STATE.md` al iniciar y actualícelo al cerrar la sesión.

## Qué no hacer
- No escriba claves ni contraseñas en el código; use variables de entorno.
- No instale dependencias sin verificar que existen en PyPI.
- No modifique ni borre pruebas para que pasen.
- No use datos personales reales en pruebas ni ejemplos.
- No suba archivos `.env` ni contraseñas al repositorio.
- No hacer commit ni push: los hace el desarrollador.
## Lecciones aprendidas
Registre aquí cada error importante y la regla para evitar repetirlo.
## Convenciones
- Al iniciar cada sesión, leer STATE.md.