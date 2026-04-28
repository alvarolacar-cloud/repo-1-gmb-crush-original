# Decisiones y fuentes — GMB Crush V6.4

Fase 2 de trazabilidad del sistema GMB Crush. Un archivo por paso, asignando a cada decisión su fuente real.

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

## Cómo rellenar las columnas de fuente

Las columnas **Fuente para la decisión** y **Funcionamiento de la fuente** están vinculadas. Cada fuente tiene una frase fija de funcionamiento.

**Pasos:**
1. Identifica todas las fuentes posibles de la decisión.
2. Aplica la regla de prioridad de abajo para elegir una sola fuente (la que más arriba esté en la jerarquía manda).
3. Copia la frase fija correspondiente en `Funcionamiento de la fuente`.
4. Si hay un matiz específico (citar paso de origen, aclarar el caso), añádelo al final separado por un punto.

---

## Regla de prioridad — una decisión, una fuente

Cuando una decisión depende de varias fuentes, en la columna `Fuente para la decisión` se pone solo la que más arriba aparece en esta jerarquía:

```
1. IA sin respaldo
2. IA heredada (paso X.YY)
3. Datos de búsqueda
4. Competidores
5. GMB Crush
6. Input humano
```

**Por qué:** la fuente que manda es la que determina si la decisión está cerrada o requiere acción. Si una decisión combina GMB Crush con IA heredada, manda IA heredada porque es el eslabón débil — el patrón está bien, pero el valor sobre el que opera no. La columna refleja siempre lo que limita la validez.

Si necesitas mencionar las otras fuentes, lo haces como matiz al final del Funcionamiento, separado por un punto.

---

## Tabla de referencia — 6 fuentes únicas

| # | Fuente | Frase fija de funcionamiento |
|---|---|---|
| 1 | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. |
| 2 | IA heredada (paso X.YY) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. |
| 3 | Datos de búsqueda | El valor requiere validación con keyword research (volumen, intención, dificultad) antes de confirmar. |
| 4 | Competidores | El valor requiere validación con análisis de competencia (SERP analysis, gap competitivo) antes de confirmar. |
| 5 | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. |
| 6 | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. |

---

## Filtrado de tareas

Con esta jerarquía, identificar la lista de tareas pendientes es trivial:

- **Requieren acción (prioridad 1–4):** IA sin respaldo · IA heredada · Datos de búsqueda · Competidores
- **Cerradas (prioridad 5–6):** GMB Crush · Input humano

---

## Resumen del ejemplo Cerrajeros Madrid 24h (334 decisiones)

Recuento bajo la nueva jerarquía (manda la fuente más arriba):

| Fuente | Cantidad | % | Estado |
|---|---:|---:|---|
| IA sin respaldo | 56 | ~17% | Requiere validación |
| IA heredada | 58 | ~17% | Se cura al cerrar paso de origen |
| Datos de búsqueda | 0 | 0% | — |
| Competidores | 0 | 0% | — |
| GMB Crush | 200 | ~60% | Cerrada |
| Input humano | 20 | ~6% | Cerrada |

**Hallazgos principales:**

- 0 decisiones citan Datos de búsqueda o Competidores en todo el sistema.
- Pasos 4, 5, 6, 7, 11 y 13 son framework puro (0% IA sin respaldo).
- Pasos 1, 3 y 14 concentran la mayor parte de IA sin respaldo.
- Los focos principales de IA sin respaldo son: 15 GeoArticle topics, 6 Priority Scores, 6 Q&A + Posts del GBP, 5 capacidades de cliente del paso 10 y los trust signals/CTA del paso 1.
- Las 14 decisiones de Local Coverage Areas (Direct y Candidate) se marcan **GMB Crush** porque la doctrina respalda su selección (§35.1 para Direct, §34 test GEO 3/6 para Candidate).
- Las 2 decisiones de provincia y código postal (1.11, 1.12) se marcan **Input humano** porque vienen del NAP completo proporcionado por el cliente.
- Paso 2 está dominado por IA heredada porque depende de los servicios elegidos en paso 1 (1.34–1.38).
