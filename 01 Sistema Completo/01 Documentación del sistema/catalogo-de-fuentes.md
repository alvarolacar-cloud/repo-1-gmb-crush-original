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

## Catálogo de fuentes — dos dimensiones ortogonales

Cada decisión se rellena con **dos columnas independientes**:

- **Fuente para la decisión** — quién dicta la decisión (la doctrina, el cliente, el operador, la IA).
- **Origen del dato** — de dónde sale el valor concreto que aparece en la decisión.

Ambas dimensiones son ortogonales: la mayoría de decisiones tienen Fuente = GMB Crush porque la doctrina dicta cómo se hace algo, pero el Origen del dato puede ser distinto (competidores, cliente, búsqueda, herencia, etc.).

### Tabla 1 — Fuente para la decisión (5 valores)

Quién dicta la decisión.

| # | Fuente | Frase fija de funcionamiento |
|---|---|---|
| 1 | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. La doctrina dicta cómo se hace; el dato concreto puede venir de varios sitios (ver Origen del dato). |
| 2 | Input humano | El cliente proporciona este dato directamente sin filtro del framework. El sistema lo recoge sin transformación. |
| 3 | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Está cerrada salvo que el cliente solicite cambio o las métricas justifiquen revisión. |
| 4 | IA sin respaldo | Caso extremo: la decisión no sigue ninguna doctrina ni input externo; la IA decide libremente. Solo aplica a placeholders puros del ejemplo (datos de proceso QA, etc.). |
| 5 | IA heredada (paso X.YY) | La fuente que dicta se hereda del paso de origen citado. La cita del paso es obligatoria. |

### Tabla 2 — Origen del dato (6 valores)

De dónde sale el valor concreto.

| # | Origen del dato | Significa |
|---|---|---|
| 1 | Doctrina GMB Crush | El valor está fijado por el framework (regla, default, patrón). No es input externo. |
| 2 | Input humano | El cliente proporciona el valor concreto. |
| 3 | Competidores | El valor sale de análisis SERP / Local Pack. Si todavía no se ha ejecutado, queda como pendiente. |
| 4 | Datos de búsqueda | El valor sale de keyword research (volumen, intención, dificultad). Si todavía no se ha ejecutado, queda como pendiente. |
| 5 | Decisión de diseño | El operador eligió el valor por criterios de UX/conversión (extracción de web de referencia, paleta visual, CTA, layouts). |
| 6 | Heredado del paso X.YY | El valor cascadea de otra decisión. La cita del paso de origen es obligatoria. |
| 7 | IA sin respaldo | Valor inventado para el ejemplo sin investigación. Debe sustituirse por dato real antes de producción. |

### Por qué dos columnas y no una

Las dos columnas responden a preguntas distintas:

- "¿Quién dicta esta decisión?" → la doctrina, el cliente o el operador. Eso va en **Fuente**.
- "¿De dónde sale el valor concreto que aparece?" → competidores, búsqueda, cliente, herencia o IA. Eso va en **Origen del dato**.

Ejemplo: para el servicio core "Cerrajero urgente" (1.34):

- **Fuente:** GMB Crush (la doctrina dicta cómo identificar core services).
- **Origen del dato:** Competidores (el valor concreto debe venir del Local Pack del sector).

Antes mezclábamos las dos en una sola columna y salían combinaciones raras como `GMB Crush + IA sin respaldo`. Con dos columnas, cada celda tiene una fuente y un origen claros y separados.

### Filtrado de tareas

- **Decisiones cerradas:** Origen del dato ∈ {Doctrina GMB Crush, Input humano, Decisión de diseño, Heredado de un paso ya cerrado}.
- **Decisiones pendientes:** Origen del dato ∈ {Competidores (pendiente), Datos de búsqueda (pendiente), IA sin respaldo, Heredado de un paso pendiente}.

La columna **Fuente** no se usa para filtrar tareas — todas las decisiones GMB Crush son canónicas. Lo que pendiente o cerrada es la columna **Origen del dato**.

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
