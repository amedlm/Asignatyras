# Guía de contribución — Web Semántica (UCLV)

¡Gracias por tu interés en contribuir a este repositorio! Esta guía describe
cómo estudiantes, profesores y colaboradores externos pueden proponer mejoras,
reportar errores o añadir materiales al curso.

## Código de conducta

La participación en este repositorio implica aceptar y respetar nuestro
[Código de Conducta](CODE_OF_CONDUCT.md). Por favor, léelo antes de contribuir.

## Roles

- **Estudiantes**: leen el material, entregan prácticas vía GitHub Classroom y
  pueden reportar errores o proponer mejoras.
- **Maintainers**: profesores del Grupo de Web Semántica de la UCLV. Revisan
  Pull Requests, gestionan Issues y mantienen la coherencia del repositorio.
- **Collaborators externos**: profesores de otras instituciones (VLIR-UOS,
  Universidad de Hasselt, Iberoamérica) que proponen contribuciones vía PR.

## Flujo de trabajo

### 1. Fork y clonado

```bash
# 1. Haz fork desde la web de GitHub (botón Fork arriba a la derecha)
# 2. Clona tu fork localmente
git clone https://github.com/TU_USUARIO/web-semantica.git
cd web-semantica

# 3. Añade el repositorio upstream para sincronizar cambios
git remote add upstream https://github.com/uclv-cinfo/web-semantica.git
```

### 2. Crea una rama descriptiva

```bash
git checkout -b fix/u3-typo-sparql
# o
git checkout -b feat/u5-nueva-practica-wikidata
```

### 3. Realiza los cambios y haz commit

Seguimos la especificación **Conventional Commits**:

| Tipo      | Uso                                            |
|-----------|------------------------------------------------|
| `feat:`   | Nueva práctica, diapositiva o dataset          |
| `fix:`    | Corrección de error en material existente      |
| `docs:`   | Cambio en documentación (README, apuntes)      |
| `style:`  | Formato, sin cambio de contenido               |
| `refactor:`| Reorganización de carpetas o archivos          |
| `test:`   | Nuevos tests de consultas o validaciones      |

Ejemplos:

```bash
git commit -m "feat(u3): añade práctica sobre ontologías OWL"
git commit -m "fix(u5): corrige typo en consulta SPARQL"
git commit -m "docs: actualiza cronograma del semestre"
```

### 4. Push y Pull Request

```bash
git push origin fix/u3-typo-sparql
```

Abre el Pull Request desde GitHub. Se cargará automáticamente la plantilla
`.github/PULL_REQUEST_TEMPLATE.md`: complétala con cuidado, especialmente el
checklist de autoevaluación.

### 5. Revisión y fusión

- Al menos **un maintainer** debe aprobar el PR.
- Los PR propuestos por estudiantes deben además ser revisados por **un par**
  (otro estudiante).
- Se usa **squash merge** para mantener un historial limpio.

## Convenciones de estructura

- Las prácticas van en `unidades/uN/practicas/` con nombre `practica-N.md`.
- Los datasets RDF van en `unidades/uN/datasets/` con extensión `.ttl`.
- Las ontologías OWL van en `ontologias-ejemplo/` o en la unidad correspondiente.
- Las consultas SPARQL van en `endpoints-sparql/` con extensión `.rq`.
- Las diapositivas se publican en `teoria/` tanto en PDF como en HTML
  (reveal.js).

## Reportar errores sin programar

Si no quieres enviar un PR pero detectaste un error, abre un Issue usando la
plantilla **"Error en el material"**. Está perfectamente bien reportar sin
corregir; el equipo docente lo atenderá.

## Reconocimiento

Cada Pull Request aceptado queda registrado en el historial del repositorio y
en la lista de contribuyentes de GitHub. Si eres estudiante, este historial es
evidencia verificable de tu participación, útil para cartas de recomendación y
expedientes académicos.

## ¿Dudas?

- Para preguntas sobre el contenido del curso: abre un Issue con la plantilla
  **"Duda sobre el contenido"**.
- Para preguntas sobre la infraestructura (Git, GitHub, Classroom): escribe a
  `amedcuba73@gmail.com` o consulta las [Discusiones](../../discussions) del repo.

¡Bienvenido/a y gracias por contribuir!
