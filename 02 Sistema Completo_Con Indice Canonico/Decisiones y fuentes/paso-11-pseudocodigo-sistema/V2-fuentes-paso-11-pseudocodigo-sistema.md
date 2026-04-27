# Paso 11 — Pseudocódigo del Sistema — Fuentes por decisión

Fase 2 de trazabilidad. Sobre `V1-decisiones-paso-11-pseudocodigo-sistema.md`.

Negocio del ejemplo: **Cerrajeros Madrid 24h** · 16 decisiones.

---

## Convenciones de fuente

- **Teoría GMB** — la dicta una regla del framework.
- **Geografía** — hechos físicos verificables.
- **Datos de búsqueda** — keyword volume, intención, GSC.
- **Competidores** — SERP analysis, gap.
- **IA sin respaldo** — sin fuente citada o heredada.

---

## Tabla de fuentes

| IDs | Bloque V1 | Decisión | Fuente |
|---|---|---|---|
| 11.01 | 1 — Inputs, slugs y categorías | Cargar inputs base | Teoría GMB (deriva de paso 1) |
| 11.02 | 1 — Inputs, slugs y categorías | Normalizar slugs | Teoría GMB (paso-04 reglas slug) |
| 11.03 | 1 — Inputs, slugs y categorías | Validar categorías adicionales (cubierta / página) | Teoría GMB (paso 1 regla operativa 3) |
| 11.04 | 2 — Generación base | Generar Homepage | Teoría GMB |
| 11.05 | 2 — Generación base | Generar 5 SO | Teoría GMB |
| 11.06 | 2 — Generación base | Generar GeoHub de Madrid | Teoría GMB |
| 11.07 | 2 — Generación base | Generar 5 LBS | Teoría GMB |
| 11.08 | 2 — Generación base | Generar AC de duplicado-llaves | Teoría GMB |
| 11.09 | 2 — Generación base | Generar 15 GeoArticles | Teoría GMB |
| 11.10 | 3 — LCAs y expansión | Inyectar LCAs en contenido y schema | Teoría GMB (paso 6) |
| 11.11 | 3 — LCAs y expansión | No generar expansión sin aprobación | Teoría GMB |
| 11.12 | 4 — Enlaces, prioridad, QA y outputs | Asignar enlaces internos por page type | Teoría GMB (paso 7) |
| 11.13 | 4 — Enlaces, prioridad, QA y outputs | Calcular prioridad por página | Teoría GMB (paso 8) |
| 11.14 | 4 — Enlaces, prioridad, QA y outputs | Comprobar dependencias (LBS requiere SO + GeoHub) | Teoría GMB (regla de dependencias) |
| 11.15 | 4 — Enlaces, prioridad, QA y outputs | Ejecutar QA antes de publicar | Teoría GMB (paso 9) |
| 11.16 | 4 — Enlaces, prioridad, QA y outputs | Producir 6 matrices finales | Teoría GMB |

---

## Subtotal del paso

| Fuente | Cantidad |
|---|---:|
| Teoría GMB pura | 16 |
| Geografía | 0 |
| Datos de búsqueda | 0 |
| Competidores | 0 |
| IA sin respaldo | 0 |
| **Total** | **16** |

**% IA sin respaldo del paso: 0%** — todo el pseudocódigo deriva mecánicamente de las reglas de los pasos 1–10.

## Hallazgo

El paso 11 es la traducción algorítmica del sistema. Por definición no toma decisiones nuevas — solo orquesta las decisiones de pasos anteriores. La calidad de su output depende exclusivamente de la calidad de los inputs de paso 1 (que sí tienen IA sin respaldo).

## Recomendaciones

Ninguna acción específica para el paso 11.
