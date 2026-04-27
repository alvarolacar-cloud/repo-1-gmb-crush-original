# Paso 4 — URL Rules — Fuentes por decisión

Fase 2 de trazabilidad. Sobre `V1-decisiones-paso-04-url-rules.md`.

Negocio del ejemplo: **Cerrajeros Madrid 24h** · 18 decisiones.

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
| 4.01 | 1 — Dominio y formato general | HTTPS | Teoría GMB (best practice / SSL) |
| 4.02 | 1 — Dominio y formato general | www canónico | Teoría GMB (un dominio canónico) sobre IA sin respaldo (elección www vs naked en el ejemplo) |
| 4.03 | 1 — Dominio y formato general | Trailing slash sí | Teoría GMB (regla decisión binaria uniforme) |
| 4.04–4.09 | 2 — Patrones URL principales | 6 patrones URL por page type (Homepage, SO, LBS, AC, GeoHub, GeoArticle) | Teoría GMB (patrones canónicos paso-04 §9–§14) |
| 4.10–4.14 | 3 — URLs concretas de servicio | 5 URLs LBS concretas (cerrajero-urgente, apertura-puertas, cambio-cerraduras, cambio-bombines, instalacion-cerraduras-seguridad) | Teoría GMB (patrón) + IA sin respaldo (servicios heredados de paso 1) |
| 4.15 | 4 — Reglas anti-URL débil | No `near-me` en URLs principales | Teoría GMB |
| 4.16 | 4 — Reglas anti-URL débil | No usar `best/cheap/top-rated` | Teoría GMB |
| 4.17 | 4 — Reglas anti-URL débil | No URLs para Local Coverage Areas en la base | Teoría GMB |
| 4.18 | 4 — Reglas anti-URL débil | Approved Expansion Areas solo si se aprueban | Teoría GMB |

---

## Subtotal del paso

| Fuente | Cantidad |
|---|---:|
| Teoría GMB pura | 13 |
| Teoría GMB (patrón) sobre IA heredada (servicios) | 5 |
| Geografía | 0 |
| Datos de búsqueda | 0 |
| Competidores | 0 |
| IA sin respaldo pura | 0 |
| **Total** | **18** |

**% IA sin respaldo del paso: 0% pura** — todas las decisiones son framework, aunque 5 se apoyan sobre servicios heredados de paso 1 (que sí son IA sin respaldo).

## Hallazgo

Paso 4 es el más limpio del sistema en términos de fuente. Todas las decisiones son patrones canónicos GMB Crush. La calidad de las URLs concretas (4.10–4.14) depende exclusivamente de saneear los servicios core en paso 1.

## Recomendaciones

Ninguna acción específica para el paso 4. Si se sanean los servicios core de paso 1, el paso 4 queda automáticamente trazado.
