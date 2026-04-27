# Paso 9 — QA Checklist — Fuentes por decisión

Fase 2 de trazabilidad. Sobre `V1-decisiones-paso-09-qa-checklist.md`.

Negocio del ejemplo: **Cerrajeros Madrid 24h** · 23 decisiones.

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
| 9.01 | 1 — Ejemplo desarrollado | LBS auditada `/cerrajero/madrid/cerrajero-urgente/` | Teoría GMB (heredado) |
| 9.02 | 1 — Ejemplo desarrollado | ID de QA = LBS-001 | Teoría GMB |
| 9.03 | 1 — Ejemplo desarrollado | Tipo de página = Location-Based Service | Teoría GMB |
| 9.04 | 1 — Ejemplo desarrollado | Servicio objetivo = Cerrajero urgente | Teoría GMB (heredado) |
| 9.05 | 1 — Ejemplo desarrollado | Main City = Madrid | Teoría GMB (heredado) |
| 9.06 | 1 — Ejemplo desarrollado | Estado QA = Ready for QA | IA sin respaldo (proceso inventado para el ejemplo) |
| 9.07 | 1 — Ejemplo desarrollado | Reviewer = SEO Manager | IA sin respaldo |
| 9.08 | 1 — Ejemplo desarrollado | Fecha QA = 2026-04-24 | IA sin respaldo |
| 9.09 | 2 — Checks obligatorios | Validar parent page = `/cerrajero/cerrajero-urgente/` | Teoría GMB |
| 9.10 | 2 — Checks obligatorios | Validar GeoHub = `/madrid/` | Teoría GMB |
| 9.11 | 2 — Checks obligatorios | Validar servicios relacionados | Teoría GMB |
| 9.12 | 2 — Checks obligatorios | Validar GeoArticle relacionado | Teoría GMB |
| 9.13 | 2 — Checks obligatorios | Validar LocalBusiness schema | Teoría GMB |
| 9.14 | 2 — Checks obligatorios | Validar BreadcrumbList | Teoría GMB |
| 9.15 | 2 — Checks obligatorios | Validar FAQPage | Teoría GMB |
| 9.16 | 2 — Checks obligatorios | Validar Speakable | Teoría GMB |
| 9.17 | 2 — Checks obligatorios | Validar NAP del Paso 1 | Teoría GMB |
| 9.18 | 2 — Checks obligatorios | Validar CTA presente | Teoría GMB |
| 9.19 | 2 — Checks obligatorios | Validar no falsa ubicación | Teoría GMB (regla "no fake location") |
| 9.20 | 2 — Checks obligatorios | Validar no canibalización | Teoría GMB (regla anti-canibalización) |
| 9.21 | 3 — Inventario QA | 28 URLs en QA Status | Teoría GMB |
| 9.22 | 3 — Inventario QA | `/contacto/` también pasa QA operativo | Teoría GMB |
| 9.23 | 3 — Inventario QA | Resto de URLs Pending hasta ejecución | Teoría GMB |

---

## Subtotal del paso

| Fuente | Cantidad |
|---|---:|
| Teoría GMB pura | 20 |
| Geografía | 0 |
| Datos de búsqueda | 0 |
| Competidores | 0 |
| **IA sin respaldo** | **3** (9.06–9.08) |
| **Total** | **23** |

**% IA sin respaldo del paso: 13%** — concentrado en los 3 datos del proceso (estado, reviewer, fecha) que son placeholders del ejemplo.

## Hallazgo

El paso 9 es framework casi puro. Las únicas decisiones IA sin respaldo (9.06–9.08) son metadatos del proceso QA inventados para ilustrar — no son fallos estructurales del sistema, son rellenos del ejemplo.

## Recomendaciones

1. Marcar 9.06–9.08 como "datos de proceso del ejemplo, no del sistema" en una nota.
2. Cuando se ejecute QA real, esos campos pasarán a tener fuente verificable (timestamp + nombre del reviewer real).
