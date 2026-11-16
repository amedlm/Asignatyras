# U1 — Análisis formal (ISBD / UNIMARC / MARC 21)

| | |
|---|---|
| Horas | 12 |
| Sesiones | 4 |
| Prerrequisitos | Ninguno (asignatura base) |
| Práctica evaluable | **P1-MARC21** (individual, autograding PyMARC + CompMARC) |

## Objetivos

1. Aplicar la normativa ISBD a la descripción formal de monografías.
2. Comprender la correspondencia ISBD → UNIMARC → MARC 21.
3. Identificar los campos obligatorios de un registro MARC 21 (Leader, 001, 008, 1XX, 245, 260, 650).
4. Construir un registro MARC 21 completo para una monografía real.
5. Verificar la calidad del registro con CompMARC.

## Lecturas obligatorias

- IFLA (2011). *International Standard Bibliographic Description (ISBD)*. https://www.ifla.org/isbd
- Library of Congress. *MARC 21 Format for Bibliographic Data*. https://www.loc.gov/marc/bibliographic/
- Maxwell, R. L. (2004). *Maxwell's Handbook for MARC 21*. ALA Editions.

## Lecturas complementarias

- Marcos de Cabezón, B. (2018). *Catalogación*. Trea.
- Library of Congress. *MARC 21 Concise Format*.

## Actividades

### Antes de la sesión 1
- Video H5P «Las 8 áreas ISBD» (10 min).
- Cuestionario H5P U1 parte 1 (8 preguntas).

### Sesión 1 — ISBD
- Las 8 áreas: título y mención de responsabilidad, edición, publicación,
  descripción física, serie, notas, ISBN, adquisiciones.
- Puntuación ISBD (`.`, `;`, `:`, `/`, `,`).

### Sesión 2 — UNIMARC vs MARC 21
- Historia y diferencia entre formatos.
- Estructura de un registro: Leader, directorio, campos de control (00X),
  campos de datos (1XX-9XX), indicadores, subcampos (`$a`, `$b`).

### Sesión 3 — MARC 21 esenciales
- `001` control number, `008` fixed-length data.
- `100` autor principal, `245` título, `260` publicación.
- `650` materia, `020` ISBN, `090` signatura local.

### Sesión 4 — Práctica P1-MARC21
- Enunciado: catalogar 3 monografías en MARC 21.
- Entrega vía GitHub Classroom: archivos `.mrc` (binario) y `.xml` (MARCXML).
- Autograding: `pymarc` valida sintaxis y `compmarc.py` calcula score.

## Evaluación — Práctica P1-MARC21

| Criterio | Peso |
|---|---|
| Sintaxis MARC 21 válida (PyMARC parse OK) | 30 % |
| Campos obligatorios presentes (001, 100, 245, 260, 650) | 25 % |
| Score CompMARC ≥ 70 % | 25 % |
| Subcampos correctos en cada campo | 10 % |
| Indicadores correctos (1XX, 245) | 10 % |

## Recursos adicionales

- Registros ejemplo en [`../../marcos-catalograficos/marc21/ejemplos/`](../../marcos-catalograficos/marc21/ejemplos/)
- CompMARC: [`../../herramientas/compmarc/`](../../herramientas/compmarc/)
- ABCD-UCLV: [`../../herramientas/abcd-uclv/`](../../herramientas/abcd-uclv/)
- Library of Congress MARC: https://www.loc.gov/marc/

## Glosario clave

- **ISBD**: International Standard Bibliographic Description.
- **MARC 21**: Machine-Readable Cataloging, formato del LC.
- **Leader**: primeros 24 caracteres del registro MARC (control).
- **Campo de control**: campo 00X sin indicadores ni subcampos.
- **Campo de datos**: campo 1XX-9XX con indicadores (2) y subcampos (`$a`).
