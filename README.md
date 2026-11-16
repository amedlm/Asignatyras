# Plantilla — Práctica P3-SPARQL (Web Semántica UCLV)

Plantilla para el assignment **P3-SPARQL** de GitHub Classroom. Al aceptar
el assignment se crea una copia privada con este contenido.

## Enunciado

Escribe **5 consultas SPARQL** sobre el dataset bibliográfico
`dataset-bibliografico.ttl` (incluido en esta plantilla) cargado en un
endpoint local Apache Jena Fuseki. Las consultas se entregan en el archivo
`solucion.rq`.

| # | Tipo | Enunciado |
|---|---|---|
| 1 | `SELECT` | Listar todos los libros publicados después de 2000, con autor y año |
| 2 | `SELECT` | Contar cuántos libros hay por cada editorial, ordenado descendentemente |
| 3 | `SELECT` | Libros con materia «Filosofía» o «Cuba», usando `OPTIONAL` para mostrar traducciones |
| 4 | `CONSTRUCT` | Devolver tripletas `?libro bib:tieneAutorTraducido ?autorTraducido` para libros con traducción al inglés |
| 5 | `SERVICE` federada | Para cada autor del dataset, enriquecer con su ORCID consultando Wikidata (`SERVICE <https://query.wikidata.org/sparql>`) |

## Estructura inicial

```
.
├── README.md
├── solucion.rq                  ← AQUÍ ESCRIBES TUS 5 CONSULTAS
├── dataset-bibliografico.ttl    ← Dataset de ejemplo (NO editar)
└── .github/
    └── workflows/
        └── validar-sparql.yml   ← autograding (no editar)
```

## Cómo trabajar

1. Carga local del dataset en Fuseki:
   ```bash
   # Iniciar Fuseki (sigue el README del repo principal)
   curl -s -X POST \
     -H "Content-Type: text/turtle" \
     --data-binary @dataset-bibliografico.ttl \
     http://localhost:3030/ds/data
   ```
2. Prueba cada consulta con `curl`:
   ```bash
   QUERY=$(sed -n '/# === Consulta 1 ===/,/# === Consulta 2 ===/p' solucion.rq | sed '$d')
   curl -s -G http://localhost:3030/ds/query \
     --data-urlencode "query=$QUERY" \
     -H "Accept: application/sparql-results+json" | jq '.results.bindings | length'
   ```
3. Commitea con un commit por consulta:
   ```bash
   git commit -m "feat(consulta-1): libros publicados después de 2000"
   ```
4. Push a `main`. El workflow `validar-sparql.yml` ejecuta las 5 consultas
   automáticamente y compara el número de resultados con el gold standard.
5. Cuando el workflow esté verde, abre el Issue de entrega.

## Rúbrica

| Criterio | Peso | Cómo se verifica |
|---|---|---|
| 5 consultas ejecutan sin error | 40 % | HTTP 200 |
| Resultados = gold standard | 30 % | Comparación automática |
| Uso significativo de `OPTIONAL`, `UNION`, `CONSTRUCT` | 10 % | Inspección |
| Consulta federada con `SERVICE` | 10 % | Sintaxis |
| Comentarios y formato | 10 % | Inspección |

¡Mucho éxito!
