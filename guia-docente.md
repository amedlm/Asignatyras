# Guía Docente — Web Semántica (UCLV)

> **Plantilla editable.** Sustituir los campos entre corchetes `【…】` por los
> datos oficiales del curso y exportar a PDF para subir como `guia-docente.pdf`
> al repositorio. Las secciones siguen el modelo oficial de la Universidad
> Central «Marta Abreu» de Las Villas (UCLV) para el Programa de Formación Continua.

---

## 1. Datos generales

| Campo | Valor |
|---|---|
| Asignatura | Web Semántica |
| Código | 【código oficial UCLV】 |
| Programa | Programa de Formación Continua |
| Departamento | Ciencias de la Información |
| Facultad | 【Facultad】 |
| Curso académico | 【20XX–20XX】 |
| Fecha de inicio | 14 de febrero de 2016 (primera impartición) |
| Duración | 【XX】 semanas |
| Horas totales | 64 |
| Créditos | 【n.º de créditos】 |
| Modalidad | Presencial / Semipresencial / A distancia |
| Idioma | Español |

## 2. Equipo docente

| Rol | Nombre | Correo | Despacho |
|---|---|---|---|
| Profesor titular | Amed Leiva-Mederos | amedcuba73@gmail.com | 【edificio/despacho】 |
| Profesor auxiliar | 【nombre】 | 【correo@uclv.cu】 | 【despacho】 |
| Asistente docente | 【nombre】 | 【correo@uclv.cu】 | — |

Horario de tutorías: 【días y horas】.

## 3. Justificación y presentación

La asignatura Web Semántica se imparte en la UCLV desde el 14 de febrero de
2016, dentro del Programa de Formación Continua del Departamento de Ciencias
de la Información. Su objetivo es formar al estudiante en las tecnologías,
estándares y metodologías que permiten publicar, enlazar y consultar datos
estructurados en la Web siguiendo el paradigma de Linked Data y los estándares
del W3C (RDF, RDFS, OWL, SKOS, SPARQL).

【Párrafo adicional del profesor con la motivación específica del curso actual.】

## 4. Objetivos

### 4.1 Objetivo general
Modelar dominios de conocimiento propios de las Ciencias de la Información
mediante ontologías OWL y publicar los datos resultantes como Linked Data
consultable vía SPARQL.

### 4.2 Objetivos específicos
1. Modelar dominios mediante ontologías OWL en Protégé.
2. Serializar datos en RDF/Turtle y consultarlos mediante SPARQL.
3. Publicar datos enlazados siguiendo los cinco principios de Linked Data.
4. Diseñar vocabularios controlados con SKOS.
5. Aplicar tecnologías semánticas a problemas de Ciencias de la Información
   (catálogo bibliotecario, autoridades, tesauros).

## 5. Competencias y resultados de aprendizaje

Ver el archivo [`competencias.md`](./competencias.md) para el mapeo completo
a competencias genéricas y específicas del Programa de Formación Continua UCLV.

## 6. Contenidos por unidad

| Unidad | Tema | Horas | Resultados clave |
|---|---|---|---|
| 1 | Fundamentos de la Web Semántica | 8 | 区分 Web 1.0/2.0/3.0, explicar arquitectura de capas W3C |
| 2 | RDF y Turtle | 10 | Serializar tripletas, usar namespaces, validar sintaxis |
| 3 | Ontologías con OWL | 12 | Declarar clases, propiedades, restricciones; razonar con HermiT |
| 4 | Vocabularios SKOS | 8 | Modelar tesauros, relaciones jerárquicas y asociativas |
| 5 | SPARQL | 12 | Escribir SELECT, CONSTRUCT, ASK; federar endpoints |
| 6 | Datos Enlazados (Linked Data) | 8 | Publicar 5 estrellas, vocabularios reutilizables, dereferenciación |
| 7 | Aplicaciones en Ciencias de la Información | 6 | Casos VIVO-UCLV, Authoris, Wikidata |

## 7. Metodología docente

Aula invertida (flipped classroom) combinada con aprendizaje basado en
proyectos (ABP). El estudiante consulta la teoría y completa un cuestionario
H5P **antes** de cada sesión presencial; durante la sesión se resuelve una
práctica guiada y se recibe retroalimentación inmediata mediante rúbrica.

## 8. Evaluación

| Actividad | Peso | Instrumento | Herramienta |
|---|---|---|---|
| Práctica P1-RDF | 20 % | Repositorio GitHub Classroom | robot + rdflib |
| Práctica P2-OWL | 25 % | Repositorio + PR | robot + HermiT |
| Práctica P3-SPARQL | 25 % | Repositorio + endpoint local | Jena Fuseki |
| Examen teórico | 20 % | Cuestionario H5P | H5P + Moodle |
| Participación en Issues/PR | 10 % | Trazabilidad GitHub | Issues + PRs |

## 9. Cronograma semanal

Ver el archivo [`cronograma.md`](./cronograma.md) para el calendario detallado
semana a semana, incluyendo fechas de entrega.

## 10. Bibliografía

Ver el archivo [`biblioteca.bib`](./biblioteca.bib) para la bibliografía
completa en formato BibTeX. Referencias básicas:

- Hitzler, P., Krötzsch, M., Rudolph, S. (2021). *Foundations of Semantic Web
  Technologies*. 2.ª ed. CRC Press.
- Allemang, D., Hendler, J. (2011). *Semantic Web for the Working Ontologist*.
  2.ª ed. Morgan Kaufmann.
- Hebeler, J. et al. (2011). *Semantic Web Programming*. Wiley.

## 11. Recursos y plataformas

- Repositorio del curso: https://github.com/uclv-cinfo/web-semantica
- GitHub Classroom: invitación vía correo @uclv.cu
- Endpoint Wikidata: https://query.wikidata.org/sparql
- Protégé: https://protege.stanford.edu/

## 12. Políticas

- **Originalidad:** todo el material reutilizado debe citarse siguiendo CC BY-SA 4.0.
- **Entregas tardías:** penalización del 10 % por día, hasta 3 días.
- **Código de conducta:** se aplica el `CODE_OF_CONDUCT.md` del repositorio.
- **Accesibilidad:** los materiales siguen pautas WCAG 2.1 AA.

---

Documento generado a partir de plantilla · UCLV, 【fecha】.
