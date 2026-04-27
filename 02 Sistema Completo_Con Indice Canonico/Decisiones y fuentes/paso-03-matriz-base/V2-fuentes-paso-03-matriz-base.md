# Paso 3 — Matriz Base — Fuentes por decisión

Fase 2 de trazabilidad. Sobre `V1-decisiones-paso-03-matriz-base.md`.

Negocio del ejemplo: **Cerrajeros Madrid 24h** · 35 decisiones.

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
| 3.01–3.03 | 1 — Estructura de la matriz | URL Matrix, IDs únicos, columnas de producción | Teoría GMB |
| 3.04–3.05 | 2 — Homepage y páginas auxiliares | Homepage HP-001, `/` | Teoría GMB |
| 3.06 | 2 — Homepage y páginas auxiliares | `/contacto/` auxiliar | Teoría GMB |
| 3.07–3.11 | 3 — Service Overview Pages | 5 SO URLs | Teoría GMB (patrón) sobre IA sin respaldo (servicios heredados) |
| 3.12 | 4 — GeoHub y LBS | `/madrid/` GeoHub | Teoría GMB |
| 3.13–3.17 | 4 — GeoHub y LBS | 5 LBS URLs | Teoría GMB (patrón) sobre IA sin respaldo (servicios heredados) |
| 3.18 | 5 — Additional Category Page | `/cerrajero/madrid/duplicado-llaves/` | Teoría GMB |
| **3.19–3.33** | **6 — GeoArticles** | **15 URLs GeoArticle concretas** | **IA sin respaldo** (correcciones-pendientes NP4: "no vienen de keyword research real") |
| 3.34–3.35 | 7 — Tratamiento de Local Coverage Areas | LCAs como notas, no filas URL | Teoría GMB |

---

## Subtotal del paso

| Fuente | Cantidad |
|---|---:|
| Teoría GMB pura | 19 |
| Teoría GMB + IA heredada (servicios paso 1) | 0 (contabilizados en pasos canónicos como Teoría GMB con nota) |
| Geografía | 0 |
| Datos de búsqueda | 0 |
| Competidores | 0 |
| **IA sin respaldo pura** | **15** (los 15 GeoArticles) |
| Heredada parcial | 1 (clasificación de duplicado) |
| **Total** | **35** |

**% IA sin respaldo del paso: 43%** — concentrado al 100% en los 15 títulos/URLs de GeoArticles (3.19–3.33).

## Hallazgo crítico

Los 15 GeoArticles de los IDs 3.19–3.33 **son la mayor concentración de IA sin respaldo del sistema entero**. Cada slug es una intención de keyword research no documentada:

- `cuanto-cuesta-un-cerrajero-urgente`, `cuanto-tarda-un-cerrajero`, `que-hacer-si-no-puedes-entrar-casa`...

Sin volumen de búsqueda, dificultad ni gap competitivo citados, son borradores de redacción IA.

## Recomendaciones

1. **Aplicar disclosure NP4** ("estos 15 títulos son borrador derivado de la fórmula G×S=15 + lógica del servicio. No vienen de keyword research real") al inicio del bloque 6 del paso.
2. **Antes de producir**, validar cada slug con: volumen mensual, intent, dificultad, oportunidad competitiva.
3. La fórmula garantiza la **cantidad** (15); los **temas concretos** requieren validación independiente.
