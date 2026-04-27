# Paso 8 — Priority Score — Fuentes por decisión

Fase 2 de trazabilidad. Sobre `V1-decisiones-paso-08-priority-score.md`.

Negocio del ejemplo: **Cerrajeros Madrid 24h** · 15 decisiones.

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
| 8.01 | 1 — Fórmula de prioridad | Fórmula de seis factores (Revenue + Intent + GBP Relevance + Local Relevance + Gap + Urgency) | Teoría GMB (paso-08 §7) |
| 8.02 | 1 — Fórmula de prioridad | No usar City Priority — se usa Local Relevance | Teoría GMB |
| 8.03 | 2 — Ejemplo canónico | Evaluar como ejemplo la LBS de Cerrajero urgente | Teoría GMB (heredado) |
| **8.04** | 2 — Ejemplo canónico | **Revenue Value = 5** | **IA sin respaldo** — debería venir de input del cliente sobre ticket medio + márgenes |
| **8.05** | 2 — Ejemplo canónico | **Search Intent = 5** | **IA sin respaldo** — debería venir de Datos de búsqueda (volumen + intent type) |
| **8.06** | 2 — Ejemplo canónico | **GBP Category Relevance = 5** | **IA sin respaldo** — debería derivarse del catálogo GBP oficial vs. servicio |
| **8.07** | 2 — Ejemplo canónico | **Local Relevance = 5** | **IA sin respaldo** — debería venir de Datos de búsqueda + Geografía (volumen geo-targeted) |
| **8.08** | 2 — Ejemplo canónico | **Competition Gap = 4** | **IA sin respaldo** — debería venir de Competidores (SERP analysis) |
| **8.09** | 2 — Ejemplo canónico | **Conversion Urgency = 5** | **IA sin respaldo** — defendible por la naturaleza "urgente" del servicio, pero no se justifica formalmente |
| 8.10 | 2 — Ejemplo canónico | Score total = 29 | Teoría GMB (cálculo derivado de 8.04–8.09) |
| 8.11 | 2 — Ejemplo canónico | Prioridad P1 (29 ≥ 26) | Teoría GMB (tabla de tiers) |
| 8.12 | 3 — Inventario completo | Asignar Priority Score a las 28 URLs SEO base | Teoría GMB |
| 8.13 | 3 — Inventario completo | `/contacto/` con prioridad operativa, no SEO | Teoría GMB |
| 8.14 | 3 — Inventario completo | GeoArticles después de sus páginas padre | Teoría GMB (regla de dependencias) |
| 8.15 | 3 — Inventario completo | Tabla completa de 28 URLs en el sistema | Teoría GMB |

---

## Subtotal del paso

| Fuente | Cantidad |
|---|---:|
| Teoría GMB pura | 9 |
| Geografía | 0 |
| Datos de búsqueda | 0 (debería haber 2: Search Intent + Local Relevance) |
| Competidores | 0 (debería haber 1: Competition Gap) |
| **IA sin respaldo** | **6** (8.04–8.09 — los 6 valores 1-5) |
| **Total** | **15** |

**% IA sin respaldo del paso: 40%** — concentrado al 100% en los 6 valores asignados al LBS canónico.

## Hallazgo crítico

El Priority Score es la decisión más sensible del sistema en términos de fuente: **la fórmula es framework, pero los valores 1-5 deberían tener cita externa obligatoria**:

- 8.05 Search Intent → volumen mensual + intent type (informational/transactional/local)
- 8.06 GBP Category Relevance → matching con catálogo oficial GBP
- 8.07 Local Relevance → volumen geo-targeted en Madrid
- 8.08 Competition Gap → SERP analysis (qué competidores rankean ya)
- 8.04 Revenue Value → ticket medio + frecuencia × márgenes (input cliente)
- 8.09 Conversion Urgency → naturaleza del servicio (defendible por lógica, pero formalizar)

## Recomendaciones

1. **Cada valor 8.04–8.09 debe ir acompañado de su fuente** en formato `[5] (fuente: SEMrush volumen 1.900 KW=cerrajero madrid)`.
2. **Aplicar disclosure** al inicio del bloque "Ejemplo canónico" indicando que los valores son borradores hasta validar con datos de búsqueda, competidores e input del cliente.
3. **Para las 27 URLs restantes** (no scoradas en el V1), exigir el mismo formato de fuente por valor.
