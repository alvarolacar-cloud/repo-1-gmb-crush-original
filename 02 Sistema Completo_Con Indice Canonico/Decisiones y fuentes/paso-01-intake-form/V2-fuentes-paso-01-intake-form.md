# Paso 1 — Intake Form — Fuentes por decisión

Fase 2 de trazabilidad. Sobre `V1-decisiones-paso-01-intake-form.md`, se asigna fuente real a cada decisión.

Negocio del ejemplo: **Cerrajeros Madrid 24h** · 47 decisiones.

---

## Convenciones de fuente

- **Teoría GMB** — la dicta una regla del framework (8 frameworks fuente listados en `paso-01 §40`).
- **Geografía** — hechos físicos verificables (NAP, dirección, barrios reales).
- **Datos de búsqueda** — keyword volume, intención, GSC.
- **Competidores** — SERP analysis, gap, perfiles GBP rivales.
- **IA sin respaldo** — sin fuente citada; el valor se inventa o se hereda de otra IA sin respaldo.

---

## Tabla de fuentes

| IDs | Bloque V1 | Decisión | Fuente |
|---|---|---|---|
| 1.01–1.03 | 1 — Identidad del negocio | Nombre, URL, dominio canónico | Teoría GMB (campo) + IA sin respaldo (valor del ejemplo) |
| 1.04–1.07 | 2 — Estado inicial GBP | Not Created, after launch, Not Started, no URL | Teoría GMB (regla web-first) |
| 1.08–1.14 | 3 — NAP y contacto | Nombre, dirección, ciudad, provincia, CP, país, teléfono | Geografía (cliente real) → en ejemplo IA sin respaldo |
| 1.15 | 3 — NAP y contacto | Email | IA sin respaldo |
| 1.16 | 4 — Categorías GBP planificadas | Categoría primaria "Cerrajero" | IA sin respaldo (sin catálogo GBP ni validación) |
| 1.17–1.18 | 4 — Categorías GBP planificadas | 2 categorías adicionales | IA sin respaldo |
| 1.19–1.21 | 5 — Dirección física, Main City y zonas | Dirección física como ancla, Main City, ubicación física | Geografía (cliente real) → en ejemplo IA sin respaldo |
| 1.22–1.23 | 5 — Dirección física, Main City y zonas | 2 Direct LCAs (Almagro, Chamberí) | Geografía (salen del NAP — paso 1 §35.1) |
| **1.24–1.31** | 5 — Dirección física, Main City y zonas | **8 Candidate LCAs** (Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad) | **IA sin respaldo** — el sistema declara que deberían venir de proximidad/búsqueda/competencia + test GEO 3/6 (paso 1 §34), pero el test no consta ejecutado |
| 1.32–1.33 | 6 — Expansión geográfica | LCAs no generan URLs, no Approved Expansion | Teoría GMB |
| **1.34–1.38** | 7 — Servicios principales | **5 servicios core** | **IA sin respaldo** (sin keyword research ni gap analysis) |
| 1.39–1.40 | 8 — Consolidación de categorías adicionales | Cubierta / página propia | Teoría GMB (regla operativa 3) |
| 1.41 | 9 — Contenido, conversión y confianza | G=3 GeoArticles | Teoría GMB (default) |
| 1.42 | 9 — Contenido, conversión y confianza | CTA "Llamar ahora" | IA sin respaldo |
| 1.43–1.47 | 9 — Contenido, conversión y confianza | 5 trust signals | IA sin respaldo (en cliente real serían input verificable) |

---

## Subtotal del paso

| Fuente | Cantidad |
|---|---:|
| Teoría GMB pura | 12 |
| Geografía pura | 2 |
| Datos de búsqueda | 0 |
| Competidores | 0 |
| **IA sin respaldo** | **33** |
| **Total** | **47** |

**% IA sin respaldo del paso: 70%** — el más alto del sistema. Concentrado en NAP del ejemplo, categorías GBP, Candidate LCAs, servicios core, CTA y trust signals.

## Recomendaciones de cierre para este paso

1. Documentar el test GEO 3/6 ejecutado sobre los 8 Candidate LCAs.
2. Citar keyword volume + intent para los 5 servicios core.
3. Marcar trust signals como "pendientes de validación con cliente real" o moverlos a anexo.
4. Las decisiones 1.08–1.21 dejarán de ser IA sin respaldo cuando el ejemplo se sustituya por un cliente con NAP real.
