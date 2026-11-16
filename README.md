# Análisis Documental I — Programa de Formación Continua (UCLV)

![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-blue)
![Course](https://img.shields.io/badge/course-An%C3%A1lisis%20Documental%20I-2026-green)
![UCLV](https://img.shields.io/badge/UCLV-Ciencias%20de%20la%20Informaci%C3%B3n-red)
![Status](https://img.shields.io/badge/status-activo%20desde%202012-success)

Materiales docentes de la asignatura **Análisis Documental I**, impartida
desde el 8 de febrero de 2012 en el Departamento de Ciencias de la Información
de la Universidad Central «Marta Abreu» de Las Villas (UCLV), Santa Clara,
Cuba.

---

## Descripción

La asignatura forma en **análisis formal y de contenido**, **control de
autoridades** y **uso de lenguajes documentales**, con énfasis en MARC 21,
Dublin Core y MODS. Se imparte con un enfoque teórico-práctico, interactivo y
competencial, basado en **aula invertida**, **aprendizaje basado en
proyectos** y **H5P**, con talleres prácticos de indización, resumen y
elaboración de metadatos sobre corpus reales cedidos por la Biblioteca Central
de la UCLV.

## Objetivos de aprendizaje

Al finalizar la asignatura, el estudiante será capaz de:

1. Aplicar las normas ISBD, UNIMARC y RDA al análisis formal de documentos.
2. Indizar documentos con precisión utilizando tesauros y listas de
   encabezamientos.
3. Elaborar resúmenes informativos e indicativos siguiendo pautas
   internacionales.
4. Crear registros MARC 21 completos y verificar su calidad con CompMARC.
5. Diseñar metadatos Dublin Core para repositorios institucionales.

## Prerrequisitos

- Conceptos básicos de organización de la información.
- Cuenta activa en GitHub (solicítala con tu correo `@uclv.cu`).
- Un editor MARC 21: MARCEdit (recomendado) o el plugin MARC de VS Code.
- Un editor XML para los ejercicios de Dublin Core y MODS.

## Contenidos por unidad

| Unidad | Tema                                  | Horas |
|--------|---------------------------------------|-------|
| 1      | Análisis formal (ISBD / UNIMARC)      | 12    |
| 2      | Análisis de contenido                 | 10    |
| 3      | Indización                            | 12    |
| 4      | Resumen documental                    | 8     |
| 5      | Metadatos: Dublin Core                | 8     |
| 6      | Control de autoridades               | 8     |
| 7      | Lenguajes documentales                | 6     |

## Estructura del repositorio

```
analisis-documental/
├── README.md                   ← Estás aquí
├── LICENSE                     ← CC BY-SA 4.0
├── CONTRIBUTING.md             ← Cómo contribuir
├── CODE_OF_CONDUCT.md
├── programa/                   ← Guía docente, cronograma, competencias
├── unidades/                   ← Materiales por unidad temática
│   └── uN-<tema>/
│       ├── teoria/             ← PDF, slides HTML, apuntes
│       ├── practicas/          ← Enunciados, registros ejemplo y soluciones
│       │   └── registros-ejemplo/   ← .mrc (binario) y .xml (MARCXML)
│       ├── h5p/                ← Actividades interactivas
│       └── evaluacion/         ← Rúbricas validadas
├── marcos-catalograficos/      ← MARC 21, Dublin Core y MODS
│   ├── mara21/                 ← Plantillas y ejemplos
│   ├── dublin-core/
│   └── mods/
├── lenguajes-documentales/     ← Tesauros SKOS, listas de encabezamientos
├── herramientas/               ← CompMARC y configuración local ABCD
├── classroom/                 ← Plantillas para GitHub Classroom
└── recursos/                  ← Libros, enlaces, glosario
```

## Metodología

**Aprendizaje basado en proyectos + aula invertida + H5P.**

Cada unidad culmina con un **taller práctico** de indización, resumen o
elaboración de metadatos sobre corpus reales cedidos por la Biblioteca Central
de la UCLV. Antes de cada sesión, el estudiante revisa el material de
`teoria/` y completa el cuestionario H5P. Durante la sesión, se resuelve en
grupo la práctica correspondiente.

## Evaluación

La evaluación es **formativa y continua**, con las siguientes ponderaciones:

| Componente                          | Peso |
|-------------------------------------|------|
| Prácticas individuales (P1, P2)     | 30 % |
| Práctica en pareja (P3)             | 20 % |
| Proyecto final (catalogación completa) | 30 % |
| Participación (Issues, PRs, H5P)    | 10 % |
| Autoevaluación                      | 10 % |

Cada práctica se entrega mediante **GitHub Classroom**. El autograding valida
la estructura MARC 21 con `pymarc` y la completitud del registro con
**CompMARC**, la herramienta certificada por la UCLV en 2022.

## Cómo clonar este repositorio

```bash
# Si eres estudiante del curso, usa el enlace que te proporcionará GitHub Classroom.
# Si quieres solo consultar el material:

git clone https://github.com/uclv-cinfo/analisis-documental.git
cd analisis-documental
```

## Cómo contribuir

¡Las contribuciones son bienvenidas! Lee [CONTRIBUTING.md](CONTRIBUTING.md)
para conocer el flujo de trabajo (fork → branch → PR), las convenciones de
commits y el código de conducta. También puedes reportar errores abriendo
un [Issue](../../issues/new/choose).

## Recursos destacados

- **CompMARC**: herramienta para la medición de completitud de registros
  MARC 21, certificada por la Dirección de Propiedad Intelectual de la UCLV
  en marzo de 2022. Referencia en `herramientas/compmarc/`.
- **ABCD 3.0 (adaptación UCLV)**: primera adaptación integral de un sistema
  de gestión bibliotecaria de código abierto a MARC 21 en Cuba, certificada
  en julio de 2014. Configuración local en `herramientas/abcd-uclv/`.
- **Registros de ejemplo**: corpus reales cedidos por la Biblioteca Central
  de la UCLV, anonimizados, en
  `unidades/uN/practicas/registros-ejemplo/`.

## Citación académica

Si utilizas estos materiales en tu docencia o investigación, cita así:

> Leiva-Mederos, Amed (2026). *Análisis Documental I — Licenciatura en
> Ciencias de la Información, UCLV*. Repositorio GitHub.
> <https://github.com/uclv-cinfo/analisis-documental>. Licencia CC BY-SA 4.0.

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
publiques las obras derivadas bajo la misma licencia.
