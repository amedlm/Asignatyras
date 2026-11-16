# Plantilla — Práctica P2-DUBLINCORE (Análisis Documental I UCLV)

Este es el repositorio plantilla para el assignment **P2-DUBLINCORE** de
GitHub Classroom (asignatura Análisis Documental I).

## Enunciado

Crea metadatos **Dublin Core** para **5 recursos digitales** y entrega el
archivo `recursos.xml` con:

1. Una página web institucional (p. ej. UCLV).
2. Un PDF de un artículo científico.
3. Un dataset (CSV, JSON, Turtle...).
4. Una imagen fotográfica (con derechos claros).
5. Un recurso de tu elección (vídeo, audio, software...).

Requisitos mínimos:
- XML válido contra el esquema DCMI.
- 15 elementos Dublin Core Simple presentes por recurso (o justificados).
- ≥ 5 elementos Qualified (refinamientos) por recurso.
- Identificador persistente (DOI, Handle, ISBN, URL canónica).
- Codificación UTF-8.
- Idioma declarado en `dc:language`.

## Estructura inicial

```
.
├── README.md
├── recursos.xml                   ← AQUÍ ESCRIBES TUS METADATOS DC
└── .github/
    └── workflows/
        └── validar-dc.yml         ← autograding (no editar)
```

## Cómo trabajar

1. Elige los 5 recursos digitales y recopila sus datos bibliográficos.
2. Edita `recursos.xml` con la estructura del ejemplo:
   [`marcos-catalograficos/dublin-core/ejemplos-dc.xml`](../marcos-catalograficos/dublin-core/ejemplos-dc.xml)
3. Valida localmente antes de pushar:
   ```bash
   xmllint --noout --schema https://www.dublincore.org/schemas/xmls/qdc/2008/02/11/dc.xsd recursos.xml
   ```
4. Commitea con un commit por recurso:
   ```bash
   git commit -m "feat(recurso-1): metadatos DC para página web UCLV"
   ```
5. Push a `main`. El workflow valida el XML contra el esquema DCMI.
6. Cuando esté verde, abre el Issue de entrega con la plantilla
   `entrega-practica.yml`.

## Rúbrica

| Criterio | Peso | Cómo se verifica |
|---|---|---|
| XML válido contra esquema DCMI | 35 % | xmllint OK |
| 15 elementos presentes por recurso | 25 % | Recuento XPath |
| ≥ 5 refinamientos Qualified por recurso | 15 % | Recuento XPath |
| Identificador persistente (DOI/Handle/ISBN/URL) | 10 % | Inspección |
| Idioma y codificación correctos | 10 % | Inspección |
| Comentarios explicativos | 5 % | Inspección |

## Pista: ejemplo

Ver [`marcos-catalograficos/dublin-core/ejemplos-dc.xml`](../marcos-catalograficos/dublin-core/ejemplos-dc.xml)
para un ejemplo completo con los 15 elementos + Qualified + enlaces RDF.

¡Mucho éxito!
