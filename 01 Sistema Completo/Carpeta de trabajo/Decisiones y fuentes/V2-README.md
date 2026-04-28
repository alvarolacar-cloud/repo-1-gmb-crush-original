# Decisiones y fuentes — GMB Crush V6.4

Fase 2 de trazabilidad del sistema GMB Crush. Un archivo por paso, asignando a cada decisión su fuente real.

Este documento usa la taxonomía V3 ampliada con dos fuentes adicionales:

- `IA heredada (paso X.YY)` — para cascadas: cuando la decisión actual es patrón GMB pero el valor viene de una IA generada en otro paso.
- `Decisión de diseño` — para elecciones del operador o agencia que no provienen del cliente, framework, datos de búsqueda ni competidores.

---

## Archivos por paso

| Paso | Archivo |
|---|---|
| 01 — Intake Form | [01-fuentes-intake-form.md](01-fuentes-intake-form.md) |
| 02 — Fórmula maestra | [02-fuentes-formula-maestra-arquitectura.md](02-fuentes-formula-maestra-arquitectura.md) |
| 03 — Matriz base | [03-fuentes-matriz-base.md](03-fuentes-matriz-base.md) |
| 04 — URL Rules | [04-fuentes-url-rules.md](04-fuentes-url-rules.md) |
| 05 — Page Type Rules | [05-fuentes-page-type-rules.md](05-fuentes-page-type-rules.md) |
| 06 — Estructura contenido y LCA | [06-fuentes-estructura-contenido-areas-cobertura-local.md](06-fuentes-estructura-contenido-areas-cobertura-local.md) |
| 07 — Internal Linking Rules | [07-fuentes-internal-linking-rules.md](07-fuentes-internal-linking-rules.md) |
| 08 — Priority Score | [08-fuentes-priority-score.md](08-fuentes-priority-score.md) |
| 09 — QA Checklist | [09-fuentes-qa-checklist.md](09-fuentes-qa-checklist.md) |
| 10 — Producción en fases | [10-fuentes-produccion-en-fases.md](10-fuentes-produccion-en-fases.md) |
| 11 — Pseudocódigo | [11-fuentes-pseudocodigo-sistema.md](11-fuentes-pseudocodigo-sistema.md) |
| 12 — Master Prompt | [12-fuentes-master-prompt.md](12-fuentes-master-prompt.md) |
| 13 — Sistema final operativo | [13-fuentes-sistema-final-operativo.md](13-fuentes-sistema-final-operativo.md) |
| 14 — GBP Creation & Website Alignment | [14-fuentes-gbp-creation-website-alignment.md](14-fuentes-gbp-creation-website-alignment.md) |

---

## Estructura de cada tabla

Cada archivo usa 5 columnas:

```
ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo
```

---

## Catálogo de fuentes — 10 entradas

| # | Fuente | Frase fija de funcionamiento |
|---|---|---|
| 1 | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. |
| 2 | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. |
| 3 | Input humano + GMB Crush | El cliente aporta el dato y GMB Crush define cómo usarlo dentro de la arquitectura, contenido, schema o GBP. |
| 4 | Datos de búsqueda | Se valida con keyword research (volumen, intención, dificultad). Requiere validación antes de confirmar. |
| 5 | Competidores | Se valida con análisis de competencia (SERP analysis, gap competitivo). Requiere validación antes de confirmar. |
| 6 | IA sin respaldo | Valor generado para el ejemplo sin dato real, sin keyword research, sin análisis competitivo y sin confirmación humana. Debe validarse o sustituirse antes de producción. |
| 7 | GMB Crush + IA sin respaldo | GMB Crush valida la estructura o regla. El valor concreto usado en el ejemplo está pendiente de validación con input humano, datos de búsqueda o competidores. La IA se generó en este mismo paso. |
| 8 | Input humano + IA sin respaldo | El dato base viene del input humano. Algún campo concreto es placeholder y requiere validación. |
| 9 | IA heredada (paso X.YY) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. La IA NO se generó aquí, viene de otro paso. |
| 10 | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Está cerrada salvo que el cliente solicite cambio o las métricas justifiquen revisión. |

---

## Cómo distinguir IA heredada de las combinaciones con IA

Las tres categorías que contienen "IA" se aplican distinto según dónde se genera el valor IA:

| Si la IA se genera... | Fuente correcta |
|---|---|
| en este mismo paso, sola | `IA sin respaldo` |
| en este mismo paso, junto a regla GMB | `GMB Crush + IA sin respaldo` |
| en este mismo paso, junto a dato del cliente | `Input humano + IA sin respaldo` |
| en otro paso (cascada) | `IA heredada (paso X.YY)` |

Cuando la decisión es "IA heredada", la cita del paso origen es obligatoria entre paréntesis.

---

## Filtrado de tareas

- **Pendientes de validación:** cualquier celda cuya fuente contenga `IA sin respaldo`, `IA heredada`, `Datos de búsqueda` o `Competidores`.
- **Cerradas:** `GMB Crush`, `Input humano`, `Input humano + GMB Crush`, `Decisión de diseño`.

---

## Resumen del ejemplo Cerrajeros Madrid 24h (334 decisiones)

| Fuente | Cantidad | % | Estado |
|---|---:|---:|---|
| GMB Crush | 182 | ~54% | Cerrada |
| Input humano + GMB Crush | 20 | ~6% | Cerrada |
| Input humano | 16 | ~5% | Cerrada |
| Decisión de diseño | 1 | <1% | Cerrada |
| IA heredada (paso X.YY) | 56 | ~17% | Pendiente — se cura al cerrar el paso origen |
| GMB Crush + IA sin respaldo | 25 | ~7% | Pendiente — IA generada en este paso |
| Input humano + IA sin respaldo | 1 | <1% | Pendiente — detalle concreto sin validar |
| IA sin respaldo | 29 | ~9% | Pendiente |
| Competidores | 4 | ~1% | Pendiente |
| Datos de búsqueda | 0 | 0% | — |

**Estado general:** 219 decisiones cerradas (~66%) · 115 decisiones pendientes (~34%).

**Hallazgos principales:**

- 0 decisiones citan Datos de búsqueda; 4 citan Competidores (los trust signals del paso 1 que requieren benchmark sectorial).
- Pasos 4, 5, 6, 7, 11 y 13 son framework puro (0% IA).
- Pasos 1, 3 y 14 concentran la mayor parte de IA sin respaldo no heredada.
- Paso 2 está dominado por `IA heredada (paso 1.34–1.38)` (18 de 28 decisiones) porque depende de los servicios IA del paso 1.
- Paso 3 tiene 15 GeoArticles marcados `GMB Crush + IA sin respaldo` (regla framework pero topics concretos IA generados aquí, requieren keyword research).
- Las 8 Candidate LCAs (1.24–1.31) se marcan `GMB Crush + IA sin respaldo`.
- Las 2 Direct LCAs (1.22, 1.23) se marcan `Input humano + GMB Crush`.
- El dominio web (1.02, 1.03) y sus 4 herederos (4.02, 14.22, 14.23, 14.40) se marcan `Input humano` o `Input humano + GMB Crush`.
- El modelo de negocio (14.05) y los horarios (14.24) se marcan `Input humano`.
- Los 4 trust signals (1.43, 1.45, 1.46, 1.47) se marcan `Competidores`.
- El CTA (1.42) se marca `Decisión de diseño`.
- 56 decisiones IA heredada se curan automáticamente al validar el paso de origen (mayoría: paso 1.34–1.38 servicios + 1.17–1.18 categorías + 1.24–1.31 candidate LCAs).
