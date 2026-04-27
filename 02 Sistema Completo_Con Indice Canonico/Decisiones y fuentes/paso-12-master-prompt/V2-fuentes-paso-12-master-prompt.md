# Paso 12 — Master Prompt Reutilizable — Fuentes por decisión

Fase 2 de trazabilidad. Sobre `V1-decisiones-paso-12-master-prompt.md`.

Negocio del ejemplo: **Cerrajeros Madrid 24h** · 20 decisiones.

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
| 12.01 | 1 — Creación del prompt maestro | Crear Master Prompt reutilizable | Teoría GMB |
| 12.02 | 1 — Creación del prompt maestro | El prompt cubre 14 pasos | Teoría GMB |
| 12.03 | 2 — Inputs del prompt | Pedir Main City | Teoría GMB sobre Geografía heredada (Madrid sale del NAP en paso 1.20) |
| 12.04 | 2 — Inputs del prompt | Pedir Direct LCAs | Teoría GMB sobre Geografía heredada (Almagro, Chamberí salen del NAP en paso 1.22–1.23) |
| 12.05 | 2 — Inputs del prompt | Pedir Candidate LCAs | Teoría GMB sobre IA sin respaldo (8 candidates heredados) |
| 12.06 | 2 — Inputs del prompt | Pedir Approved Expansion Areas | Teoría GMB |
| 12.07 | 2 — Inputs del prompt | Pedir GBP Status | Teoría GMB |
| 12.08 | 2 — Inputs del prompt | Pedir Planned Primary GBP Category | Teoría GMB sobre IA sin respaldo (valor heredado) |
| 12.09 | 2 — Inputs del prompt | Pedir Planned Additional GBP Categories | Teoría GMB sobre IA sin respaldo (valor heredado) |
| 12.10 | 3 — Outputs del prompt | Generar URL Matrix | Teoría GMB |
| 12.11 | 3 — Outputs del prompt | Generar Page Type Rules | Teoría GMB |
| 12.12 | 3 — Outputs del prompt | Generar Content Architecture | Teoría GMB |
| 12.13 | 3 — Outputs del prompt | Generar Internal Linking Map | Teoría GMB |
| 12.14 | 3 — Outputs del prompt | Generar Priority Score | Teoría GMB |
| 12.15 | 3 — Outputs del prompt | Generar Publishing Plan | Teoría GMB |
| 12.16 | 3 — Outputs del prompt | Generar QA Checklist | Teoría GMB |
| 12.17 | 3 — Outputs del prompt | Generar GBP Creation & Website Alignment (paso 14) | Teoría GMB |
| 12.18 | 4 — Restricciones del prompt | No inventar GBP URL hasta creación | Teoría GMB |
| 12.19 | 4 — Restricciones del prompt | No crear URLs para LCAs por defecto | Teoría GMB |
| 12.20 | 4 — Restricciones del prompt | Mantener web-first | Teoría GMB |

---

## Subtotal del paso

| Fuente | Cantidad |
|---|---:|
| Teoría GMB pura | 15 (12.01–12.02, 12.06–12.07, 12.10–12.17, 12.18–12.20) |
| Teoría GMB sobre Geografía heredada | 2 (12.03, 12.04) |
| Teoría GMB sobre IA heredada | 3 (12.05, 12.08, 12.09) |
| Datos de búsqueda | 0 |
| Competidores | 0 |
| IA sin respaldo pura | 0 |
| **Total** | **20** |

**% IA sin respaldo del paso: 0% pura** — todas las decisiones son estructurales. La calidad de los inputs heredados depende del paso 1.

## Hallazgo

El paso 12 no introduce decisiones nuevas — empaqueta los outputs del sistema completo en un prompt reutilizable. Limpiar paso 1 limpia automáticamente paso 12.

## Recomendaciones

1. El V1 del paso 12 (a diferencia de mi audit anterior basado en archivos locales) **no introduce trust signals nuevos** — el repo V6.4 corrigió esa inconsistencia.
2. Ninguna acción específica más allá de saneear paso 1.
