# Web Semántica — Programa de Formación Continua (UCLV)

![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-blue)
![Course](https://img.shields.io/badge/course-Web%20Sem%C3%A1ntica-2026-green)
![UCLV](https://img.shields.io/badge/UCLV-Ciencias%20de%20la%20Informaci%C3%B3n-red)
![Status](https://img.shields.io/badge/status-activo%20desde%202016-success)

Materiales docentes de la asignatura **Web Semántica**, impartida desde el
14 de febrero de 2016 en el Departamento de Ciencias de la Información de la
Universidad Central «Marta Abreu» de Las Villas (UCLV), Santa Clara, Cuba,
como parte del Programa de Formación Continua.

---

## Descripción

La asignatura introduce al estudiante en las tecnologías semánticas aplicadas a
las Ciencias de la Información: ontologías OWL, vocabularios SKOS, RDF/Turtle,
SPARQL y datos enlazados. Se imparte con un enfoque teórico-práctico,
interactivo y competencial, basado en **aula invertida**, **H5P** y
**aprendizaje basado en proyectos**.

## Objetivos de aprendizaje

Al finalizar la asignatura, el estudiante será capaz de:

1. Modelar dominios de conocimiento mediante ontologías OWL en Protégé.
2. Serializar datos en RDF/Turtle y consultarlos mediante SPARQL.
3. Publicar datos enlazados siguiendo los cinco principios de Linked Data.
4. Diseñar vocabularios controlados con SKOS.
5. Aplicar tecnologías semánticas a problemas de Ciencias de la Información.

## Prerrequisitos

- Conceptos básicos de bases de datos y lenguajes de marcado (XML, HTML).
- Cuenta activa en GitHub (solicítala con tu correo `@uclv.cu`).
- Protégé instalado (<https://protege.stanford.edu/>).
- Editor RDF a elección: rdflib (Python), RDF Translator, EasyRDF.

## Contenidos por unidad

| Unidad | Tema                                          | Horas |
|--------|-----------------------------------------------|-------|
| 1      | Fundamentos de la Web Semántica               | 8     |
| 2      | RDF y Turtle                                  | 10    |
| 3      | Ontologías con OWL                            | 12    |
| 4      | Vocabularios SKOS                             | 8     |
| 5      | SPARQL                                        | 12    |
| 6      | Datos Enlazados (Linked Data)                 | 8     |
| 7      | Aplicaciones en Ciencias de la Información    | 6     |

## Estructura del repositorio

```
web-semantica/
├── README.md                  ← Estás aquí
├── LICENSE                    ← CC BY-SA 4.0
├── CONTRIBUTING.md            ← Cómo contribuir
├── CODE_OF_CONDUCT.md
├── programa/                  ← Guía docente, cronograma, competencias
├── unidades/                  ← Materiales por unidad temática
│   └── uN-<tema>/
│       ├── teoria/            ← PDF, slides HTML, apuntes
│       ├── practicas/         ← Enunciados y soluciones
│       ├── datasets/          ← RDF, Turtle, OWL de ejemplo
│       ├── h5p/               ← Cuestionarios interactivos
│       └── evaluacion/        ← Rúbricas validadas
├── ontologias-ejemplo/       ← VIVO-UCLV, Authoris y otras
├── endpoints-sparql/         ← Consultas reutilizables
├── classroom/                ← Plantillas para GitHub Classroom
└── recursos/                 ← Libros, enlaces, glosario
```

## Metodología

**Aula invertida + aprendizaje basado en proyectos.**

1. **Antes de cada sesión**: estudia los materiales de `teoria/` y completa el
   cuestionario H5P correspondiente.
2. **Durante la sesión**: resolvemos en grupo la práctica de `practicas/` con
   acompañamiento del profesor y de tus compañeros.
3. **Después de la sesión**: recibes retroalimentación mediante la rúbrica
   ubicada en `evaluacion/` y, si lo deseas, propones mejoras vía Pull Request.

## Evaluación

La evaluación es **formativa y continua**, con las siguientes ponderaciones:

| Componente                          | Peso |
|-------------------------------------|------|
| Prácticas individuales (P1, P3)     | 30 % |
| Práctica en pareja (P2)             | 20 % |
| Proyecto final (ontología de dominio) | 30 % |
| Participación (Issues, PRs, H5P)    | 10 % |
| Autoevaluación                      | 10 % |

Cada práctica se entrega mediante **GitHub Classroom**. El autograding valida
la sintaxis RDF/OWL con `robot` y la corrección de las consultas SPARQL contra
un endpoint Jena Fuseki de referencia.

## Cómo clonar este repositorio

```bash
# Si eres estudiante del curso, usa el enlace que te proporcionará GitHub Classroom.
# Si quieres solo consultar el material:

git clone https://github.com/uclv-cinfo/web-semantica.git
cd web-semantica
```

## Cómo contribuir

¡Las contribuciones son bienvenidas! Lee [CONTRIBUTING.md](CONTRIBUTING.md)
para conocer el flujo de trabajo (fork → branch → PR), las convenciones de
commits y el código de conducta. También puedes reportar errores abriendo
un [Issue](../../issues/new/choose).

## Recursos destacados

- **Ontología VIVO-UCLV**: en `ontologias-ejemplo/vivo-uclv.ttl`, derivada de
  las estancias de investigación en la Universidad de Hasselt (Bélgica)
  financiadas por VLIR-UOS.
- **Authoris**: herramienta para control de autoridades en la Web Semántica,
  referencia en `ontologias-ejemplo/authoris.owl`.
- **Consultas SPARQL de ejemplo**: `endpoints-sparql/` incluye consultas
  probadas contra Wikidata y DBpedia.

## Citación académica

Si utilizas estos materiales en tu docencia o investigación, cita así:

> Leiva-Mederos, Amed (2026). *Web Semántica — Programa de Formación
> Continua, UCLV*. Repositorio GitHub.
> <https://github.com/uclv-cinfo/web-semantica>. Licencia CC BY-SA 4.0.

## Contacto

- **Profesor responsable**: Amed Leiva-Mederos · Profesor Titular, UCLV
- **Correo**: amedcuba73@gmail.com
- **ORCID**: <https://orcid.org/0009-0001-5050-5563>
- **Discusiones del repo**: para preguntas abiertas, usa la pestaña
  [Discussions](../../discussions).

## Licencia

Este repositorio se distribuye bajo licencia
[Creative Commons Atribución-CompartirIgual 4.0 Internacional (CC BY-SA 4.0)](LICENSE).
Eres libre de compartir y adaptar el material, siempre que des atribución y
publishes las obras derivadas bajo la misma licencia.
