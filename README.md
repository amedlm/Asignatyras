# U7 — Aplicaciones en Ciencias de la Información

| | |
|---|---|
| Horas | 6 |
| Sesiones | 2 |
| Prerrequisitos | U1–U6 aprobadas |
| Práctica | Trabajo final de aplicación (evaluable) |

## Objetivos

1. Mapear casos de uso de Web Semántica a problemas de Ciencias de la Información.
2. Analizar la ontología VIVO-UCLV para gestión de currículums investigativos.
3. Comprender Authoris para control de autoridades semántico.
4. Usar Wikidata como fuente para catálogos bibliográficos.
5. Justificar el valor de Linked Data en bibliotecas, archivos y repositorios.

## Lecturas obligatorias

- Leiva-Mederos, A. et al. (2021). *Ontología VIVO-UCLV*. Library Hi Tech.
- Leiva-Mederos, A. et al. (2023). *Authoris: control de autoridades en la Web Semántica*. El Profesional de la Información.
- Vrandečić, D., Krötzsch, M. (2014). *Wikidata*. CACM.

## Lecturas complementarias

- VIVO Project: https://vivoweb.org/
- ISNI: https://isni.org/
- ORCID: https://orcid.org/

## Actividades

### Sesión 1 — VIVO-UCLV y Authoris
- Presentación de la ontología VIVO-UCLV: cómo modela la producción
  científica institucional.
- Demostración de Authoris: control de autoridades enlazado con Wikidata y
  VIAF.
- Discusión: ¿cómo reutilizar estos activos en el TFG del estudiante?

### Sesión 2 — Wikidata como hub bibliográfico
- Consultas SPARQL sobre Wikidata: obras de autor cubano, premios Cervantes,
  traducciones.
- Alineación de autoridades locales con Wikidata vía `owl:sameAs`.
- Estrategia de enriquecimiento: de MARC 21 (texto) a LD (URI).

### Trabajo final
- Elegir un caso real (Biblioteca UCLV, Repositorio Institucional, archivo
  personal) y proponer una aplicación semántica.
- Entrega: memoria `.md` (≥ 1500 palabras) + dataset `.ttl` o consulta `.rq`
  demostrativa.
- Defensa oral opcional (10 min).

## Evaluación

| Criterio | Peso |
|---|---|
| Justificación del caso de uso | 25 % |
| Reutilización de vocabularios estándar | 20 % |
| Dataset o consulta demostrativa funcional | 25 % |
| Calidad de la memoria (citas, estructura) | 20 % |
| Conexión con VIVO-UCLV / Authoris / Wikidata | 10 % |

## Recursos adicionales

- Currículum del responsable (ORCID): https://orcid.org/0009-0001-5050-5563
- Lista de enlaces institucionales: [`../recursos/enlaces.md`](../recursos/enlaces.md).
- Ontologías ejemplo: [`../ontologias-ejemplo/`] (VIVO-UCLV, Authoris).

## Glosario clave

- **VIVO**: ontología para representar investigadores, publicaciones, premios.
- **Authoris**: herramienta del responsable para control de autoridades semántico.
- **CRIS**: Current Research Information System.
- **ISNI/ORCID/VIAF**: identificadores persistentes para personas y obras.
