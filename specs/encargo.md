# Encargo

> **Propuesta redactada por la aprendiz** (Luisa Rossete) a falta del texto
> original del cliente. Debe validarse con el docente antes de escribir la
> especificación (`specs/spec.md`).

## Cliente y contexto

Una institución educativa de básica primaria quiere que sus estudiantes
practiquen **Lógica y programación** fuera del aula de forma divertida. Hoy los
docentes dejan ejercicios en papel y les cuesta saber quién avanzó y quién se
quedó atrás. Los niños pierden el interés porque las tareas se sienten
repetitivas.

## Lo que se pide

Una plataforma web lúdica de cursos para niños, con dos roles: **docente** y
**niño**.

### Docente

- El docente se registra e inicia sesión en la plataforma.
- El docente crea una clase y la plataforma le entrega un **código de clase**
  para compartir con sus estudiantes.
- El docente organiza el curso en **misiones**; cada misión agrupa varias
  actividades.
- El docente ve el avance de cada niño de su clase: qué misiones completó y qué
  insignias ganó.

### Niño

- El niño entra con el **código de clase** y eligiendo un **avatar**, sin
  correo ni contraseña.
- El niño ve las misiones disponibles y resuelve las actividades del curso.
- Al completar una misión, el niño gana una **insignia**.
- El niño puede ver su colección de insignias.

## Mecánica lúdica

Misiones e insignias. El detalle está en `specs/ficha-mecanica.md`.

## Condiciones

- Debe funcionar en el navegador de computadores y tabletas del colegio.
- Debe ser fácil de usar para niños pequeños.
- No se deben pedir datos personales de los niños.
- La aplicación debe estar publicada en internet para que los niños la usen
  desde casa.

## Restricciones técnicas (del proyecto)

- Python >= 3.11, FastAPI, Jinja2 y SQLModel.
- SQLite en desarrollo y PostgreSQL al publicar; despliegue en Render.
- Claves y contraseñas solo en variables de entorno.
- Interfaz y código en español.

## Entrega esperada

Un prototipo funcional publicado, con una clase de ejemplo y al menos un curso
con misiones de muestra.
