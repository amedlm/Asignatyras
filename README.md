# U6 — Control de autoridades

| | |
|---|---|
| Horas | 8 |
| Sesiones | 2 |
| Prerrequisitos | U1 + U3 aprobadas |
| Práctica | H5P U6 + ejercicio de enlaces a VIAF |

## Objetivos

1. Comprender el concepto de control de autoridades en catalogación.
2. Construir registros MARC 21 de autoridades (campos 1XX, 4XX, 5XX).
3. Establecer referencias («see» / «see also») entre formas de nombre.
4. Enlazar autoridades locales con VIAF y Wikidata.
5. Conectar el control de autoridades con la Web Semántica (Authoris).

## Lecturas obligatorias

- Maxwell, R. L. (2008). *Maxwell's Guide to Authority Work*. ALA Editions.
- Library of Congress. *MARC 21 Format for Authority Data*. https://www.loc.gov/marc/authority/
- Leiva-Mederos, A. et al. (2023). *Authoris: control de autoridades en la Web Semántica*. El Profesional de la Información.

## Lecturas complementarias

- VIAF: https://viaf.org/
- IFLA (2009). *Functional Requirements for Authority Data (FRAD)*.
- RDA Appendix N: **Access point**.

## Actividades

### Antes de la sesión 1
- Video H5P «Control de autoridades y referencias» (10 min).
- Cuestionario H5P U6 (5 preguntas).

### Sesión 1 — MARC 21 autoridades
- `100` nombre personal (autoridad), `110` corporativo, `111` reunión.
- `400` see-from tracing (variante), `500` see-also-from (relacionado).
- `370` lugar asociado, `372` campo de actividad, `375` género.
- Enlace a VIAF: campo `024` con identificador VIAF.

### Sesión 2 — Enlaces externos
- Cómo consultar VIAF para cada autor local.
- Alineación con Wikidata vía `owl:sameAs` (Web Semántica, ver Authoris).
- Estrategia para migrar autoridades en papel a identificadores persistentes.

### Práctica (no evaluable en Classroom)
- Para 5 autores del catálogo local, encontrar entrada VIAF y construir
  registro MARC 21 de autoridad con `024` y `370`.
- Entrega: PR al repo `marcos-catalograficos/marc21/plantillas/autoridades.mrc`.

## Evaluación

- Cuestionario H5P U6: 100 % de la nota.

## Recursos adicionales

- Authoris (herramienta del responsable): referencia en [`../../herramientas/`] y [`https://orcid.org/0009-0001-5050-5563`]
- VIAF: https://viaf.org/
- LC Authorities: https://authorities.loc.gov/

## Glosario clave

- **Autoridad**: forma autorizada de un nombre, título o tema.
- **See-from**: referencia desde una variante a la forma autorizada.
- **See-also-from**: referencia entre dos autoridades relacionadas.
- **VIAF**: Virtual International Authority File, agregador internacional.
- **FRAD**: Functional Requirements for Authority Data (IFLA).
