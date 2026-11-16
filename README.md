# Listas de Encabezamientos de Materia (UCLV)

Las **listas de encabezamientos** son lenguajes documentales enumerativos que
establecen la forma autorizada de los temas (materias) en un catálogo.

## Listas de referencia

| Lista | Idioma | URL |
|---|---|---|
| LCSH — Library of Congress Subject Headings | inglés | https://www.loc.gov/aba/publications/FreeLCSH/ |
| Encabezamientos de materia BNE | español | http://catalogo.bne.es/ |
| Lista de encabezamientos de materia para bibliotecas (SB) | español | https://www.bne.es |
| Tesauro UNESCO | multilingüe | http://vocabularies.unesco.org/ |
| Lista local Biblioteca UCLV | español | [catálogo local] |

## Lista local de la Biblioteca UCLV

La Biblioteca Central de la UCLV mantiene una **lista local de encabezamientos
de materia**, derivada de la práctica catalográfica cubana. Esta lista es el
gold standard para la práctica P3-INDIZACION.

Para uso docente, los estudiantes acceden a una copia local facilitada en el
aula (no se publica íntegramente para respetar la titularidad de la Biblioteca).

## Cómo construir un encabezamiento

1. Identificar el concepto principal del documento (ver U2).
2. Buscar en LCSH o en la lista local la forma autorizada.
3. Si no existe, proponer encabezamiento siguiendo las reglas:
   - Forma directa: `Bibliotecas universitarias`
   - Forma invertida: `Cuba—Historia—1959-`
   - Subdivisión geográfica: `Bibliotecas—Cuba`
   - Subdivisión cronológica: `Literatura cubana—Siglo XX`
   - Subdivisión temática: `MARC 21—Estudio y enseñanza`
4. Asignar campo MARC 21 `650` con `ind2=0` (LCSH) o `ind2=7` + `2=local`.

## Encabezamientos frecuentes en el curso

| Encabezamiento | Subdivisiones típicas | LCSH/LC |
|---|---|---|
| Bibliotecas | universitarias, públicas, escolares | LCSH |
| Bibliotecología | estudio y enseñanza, Cuba | LCSH |
| Catalogación | descriptiva, por materia, MARC 21 | LCSH |
| Indización | tesauros, listas | LCSH |
| Análisis documental | metadatos, control de autoridades | LCSH/local |
| Web Semántica | RDF, OWL, SPARQL | LCSH/local |
| Metadata | Dublin Core, MODS | LCSH |

## Recursos externos

- ClassWeb (LC Classification + LCSH): https://classweb.org/
- Cataloger's Desktop (LC): suscripción institucional
- VIAF: https://viaf.org/ (para autoridades personales)

## Nota

Esta carpeta no contiene una lista exhaustiva; la lista completa se mantiene
localmente en la Biblioteca UCLV y se cede a los estudiantes durante el curso
para uso exclusivamente educativo.
