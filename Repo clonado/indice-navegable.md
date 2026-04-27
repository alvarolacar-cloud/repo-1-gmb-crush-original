# Índice navegable del sistema GMB Crush — Cerrajeros Madrid 24h

---

## Estructura del sistema

El sistema tiene **14 pasos** organizados en **4 bloques funcionales**. Cada paso es un archivo Markdown independiente. El documento maestro (`gmb-crush-sistema-completo-v6-4.md`) integra los 14 pasos en un único flujo.

---

## Bloque 1 — Fundamentos

Aquí definimos la entidad, servicios, ciudades, categorías GBP y volumen total de páginas.

| Paso | Archivo | Descripción |
|---|---|---|
| 1 | `01-intake-form.md` | Formulario de entrada: NAP, servicios core, categorías GBP, Main City, Direct/Candidate LCA, Approved Expansion Areas. Incluye módulo de interpretación GMB Crush de la dirección física. |
| 2 | `02-formula-maestra-arquitectura.md` | Fórmula maestra de arquitectura: cálculo del total de páginas (28 SEO base), estructura jerárquica, page types y relaciones entre ellos. |
| 3 | `03-matriz-base.md` | Matriz base: tabla completa de todas las URLs del sitio con su page type, slug, servicio asociado, ciudad y fase de producción. |

---

## Bloque 2 — Arquitectura

Aquí decidimos cómo se estructura la web, qué URLs tendrá y cómo se conectan entre ellas.

| Paso | Archivo | Descripción |
|---|---|---|
| 4 | `04-url-rules.md` | Reglas de URL: patrón canónico `/category/city/service/`, convenciones de slug, reglas de unicidad, URLs prohibidas. |
| 5 | `05-page-type-rules.md` | Reglas de page type: definición de Homepage, Service Overview, GeoHub, Service Page, GeoArticle y /contacto/. Estructura, schema, CTA y contenido de cada tipo. |
| 6 | `06-estructura-contenido-areas-cobertura-local.md` | Estructura de contenido para áreas de cobertura local: cómo las Direct/Candidate LCA se integran en el contenido de cada page type sin generar URLs propias. |

---

## Bloque 3 — Priorización

Aquí decidimos qué se publica primero, qué se revisa antes de lanzar y en qué orden se ejecuta.

| Paso | Archivo | Descripción |
|---|---|---|
| 7 | `07-internal-linking-rules.md` | Reglas de internal linking: jerarquía de enlaces, anchor text, distribución de link equity, enlaces contextuales y navegacionales. |
| 8 | `08-priority-score.md` | Priority Score: matriz de prioridad para las 28 URLs basada en impacto SEO, intención de búsqueda y dependencias técnicas. |
| 9 | `09-qa-checklist.md` | QA Checklist: lista de verificación para cada URL antes de publicación (schema, CTA, internal links, contenido, meta tags). |

---

## Bloque 4 — Automatización

Aquí convertimos todo en una plantilla repetible para cualquier negocio local.

| Paso | Archivo | Descripción |
|---|---|---|
| 10 | `10-produccion-en-fases.md` | Producción en fases: calendario de producción de 7 fases para las 28 URLs, con orden de ejecución y dependencias. |
| 11 | `11-pseudocodigo-sistema.md` | Pseudocódigo del sistema: 16 bloques que describen el flujo algorítmico completo desde INPUT hasta OUTPUT. |
| 12 | `12-master-prompt.md` | Master Prompt reutilizable: prompt completo para que una IA ejecute el sistema de principio a fin con cualquier negocio local. |

---

## Pasos adicionales

| Paso | Archivo | Descripción |
|---|---|---|
| 13 | `13-sistema-final-operativo.md` | Sistema final operativo: resumen ejecutivo del sistema completo, reglas consolidadas y configuración final. |
| 14 | `14-gbp-creation-website-alignment.md` | GBP Creation & Website Alignment: configuración del Google Business Profile después de publicar la web base. Categorías, servicios GBP, fotos, posts, alineación con la web. |

---

## Documentos transversales

| Archivo | Descripción |
|---|---|
| `gmb-crush-sistema-completo-v6-4.md` | Documento maestro: integra los 14 pasos en un único flujo continuo. |
| `correcciones-aplicadas.md` | Log de todas las correcciones aplicadas al sistema. |
| `validation-full-system.md` | Validación completa de los 14 pasos. |
| `indice-navegable.md` | Este archivo. |
| `README.md` | Descripción general del repositorio. |

---

## Fuentes del sistema

1. **Framework GMB Crush** — estructura, page types, URL patterns, schema, fases, interlinking, QA
2. **Competidores** — servicios, keywords, zonas, estructura web de competidores
3. **Datos de búsqueda** — volúmenes, intenciones, long-tails reales
4. **Geografía** — barrios/distritos reales, proximidad al NAP, coherencia geográfica
5. **Input humano** — NAP, nombre del negocio, dirección, teléfono, decisiones del dueño

> Las decisiones no ancladas a ninguna de estas 5 fuentes se marcan como "la IA decide por sí misma" en los archivos de auditoría de trazabilidad.
