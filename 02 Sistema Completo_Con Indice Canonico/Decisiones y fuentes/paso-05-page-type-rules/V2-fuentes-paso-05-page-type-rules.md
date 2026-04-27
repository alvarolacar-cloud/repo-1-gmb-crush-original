# Paso 5 — Page Type Rules — Fuentes por decisión

Fase 2 de trazabilidad. Sobre `V1-decisiones-paso-05-page-type-rules.md`.

Negocio del ejemplo: **Cerrajeros Madrid 24h** · 19 decisiones.

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
| 5.01 | 1 — Homepage | Homepage como Root Entity Anchor | Teoría GMB (paso-05 §7) |
| 5.02 | 1 — Homepage | Homepage ancla marca + servicio principal + ciudad | Teoría GMB |
| 5.03 | 1 — Homepage | Homepage incluye 5 servicios core | Teoría GMB |
| 5.04 | 1 — Homepage | Homepage incluye NAP + CTA | Teoría GMB |
| 5.05 | 2 — Service Overview Pages | SO no geolocalizadas | Teoría GMB (paso-05 §8) |
| 5.06–5.10 | 2 — Service Overview Pages | 5 SO concretas | Teoría GMB (patrón) + IA sin respaldo (servicios heredados) |
| 5.11 | 3 — Location-Based Service Pages | LBS = convertidor local | Teoría GMB (paso-05 §9) |
| 5.12 | 3 — Location-Based Service Pages | Cerrajero urgente en Madrid como LBS canónica | Teoría GMB |
| 5.13 | 3 — Location-Based Service Pages | LBS H1 con servicio + ciudad | Teoría GMB |
| 5.14 | 4 — AC, GeoHub y GeoArticles | Duplicado de llaves como AC | Teoría GMB (heredado paso 1) |
| 5.15 | 4 — AC, GeoHub y GeoArticles | `/madrid/` como GeoHub | Teoría GMB |
| 5.16 | 4 — AC, GeoHub y GeoArticles | GeoArticles como boosters semánticos, no landings | Teoría GMB (paso-05 §12) |
| 5.17 | 4 — AC, GeoHub y GeoArticles | GeoArticles enlazan a LBS y GeoHub | Teoría GMB |
| 5.18 | 5 — Schema | Schema asignado por tipo de página | Teoría GMB (mapa schema canónico) |
| 5.19 | 5 — Schema | No usar `sameAs` de GBP hasta que exista el GBP | Teoría GMB (regla web-first) |

---

## Subtotal del paso

| Fuente | Cantidad |
|---|---:|
| Teoría GMB pura | 14 |
| Teoría GMB (patrón) sobre IA heredada (servicios SO) | 5 |
| Geografía | 0 |
| Datos de búsqueda | 0 |
| Competidores | 0 |
| IA sin respaldo pura | 0 |
| **Total** | **19** |

**% IA sin respaldo del paso: 0% pura** — todas las decisiones son reglas de page type del framework.

## Hallazgo

El paso 5 está completamente trazado por teoría GMB. Las únicas dependencias indirectas (servicios SO en 5.06–5.10) heredan la calidad del paso 1.

## Recomendaciones

Ninguna acción específica para el paso 5.
