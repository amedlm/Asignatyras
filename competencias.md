# Competencias — Web Semántica (UCLV)

Mapeo entre competencias del Programa de Formación Continua, resultados de
aprendizaje y unidades temáticas. Las competencias genéricas y específicas
siguen la nomenclatura oficial UCLV / ANECA.

## 1. Competencias genéricas (transversales)

| Código | Competencia | Nivel | Unidades que la trabajan |
|---|---|---|---|
| CG1 | Capacidad de análisis y síntesis | Avanzado | U1, U3, U6 |
| CG2 | Resolución de problemas en entornos nuevos | Avanzado | U2, U5, U7 |
| CG3 | Comunicación científica escrita | Intermedio | U3, U7 |
| CG4 | Trabajo en equipo y colaborativo | Intermedio | U2 (P2-OWL) |
| CG5 | Uso de Tecnologías de la Información | Avanzado | Todas |
| CG6 | Aprendizaje autónomo | Avanzado | Todas (aula invertida) |
| CG7 | Compromiso ético y atribución | Intermedio | U2, U6 (licencias CC) |

## 2. Competencias específicas (disciplinares)

| Código | Competencia | Nivel | Resultado verificable |
|---|---|---|---|
| CE1 | Modelado conceptual de dominios de información | Avanzado | Ontología OWL cargable en Protégé |
| CE2 | Serialización y publicación de datos estructurados | Avanzado | Dataset Turtle válido de ≥50 tripletas |
| CE3 | Consulta y recuperación semántica | Avanzado | 5 consultas SPARQL correctas |
| CE4 | Diseño de vocabularios controlados | Intermedio | ConceptScheme SKOS con ≥20 conceptos |
| CE5 | Aplicación de LD a Ciencias de la Información | Intermedio | Caso práctico VIVO-UCLV o Authoris |

## 3. Resultados de aprendizaje (RA) por unidad

| Unidad | RA | Criterio de evaluación | Instrumento |
|---|---|---|---|
| U1 | Distingue Web 1.0/2.0/3.0 y explica las capas del W3C | Test H5P ≥80 % | Cuestionario H5P U1 |
| U2 | Serializa tripletas RDF en Turtle sin errores sintácticos | robot validate OK | P1-RDF |
| U3 | Modela ontología OWL consistente con razonador HermiT | reason OK sin inconsistencias | P2-OWL |
| U4 | Diseña ConceptScheme SKOS con relaciones jerárquicas y asociativas | rdflib parse OK, ≥20 conceptos | H5P U4 |
| U5 | Escribe consultas SPARQL correctas (SELECT, CONSTRUCT, OPTIONAL) | 5/5 consultas OK contra Fuseki | P3-SPARQL |
| U6 | Publica un dataset como Linked Data 5 estrellas | Dereferenciación HTTP 303 | Publicación dataset |
| U7 | Aplica Web Semántica a un problema real de CInfo | Memoria + demo | Trabajo final |

## 4. Alineación con criterios ANECA

| Criterio ANECA | Evidencia en el curso |
|---|---|
| Calidad | Materiales versionados, plantillas, rúbricas |
| Innovación | Aula invertida + autograding GitHub Classroom |
| Internacionalización | Endpoints Wikidata/DBpedia, reuso CC BY-SA 4.0 |
| Competitividad | Habilidades demandadas en mercado LD/Semantic Web |
