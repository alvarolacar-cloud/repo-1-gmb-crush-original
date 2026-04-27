# Decisiones y fuentes — GMB Crush V6.4

Fase 2 de trazabilidad del sistema GMB Crush. Un archivo por paso, asignando a cada decisión su fuente real.

---

## Archivos por paso

| Paso | Archivo |
|---|---|
| 01 — Intake Form | [01-fuentes-intake-form.md](paso-01-intake-form/01-fuentes-intake-form.md) |
| 02 — Fórmula maestra | [02-fuentes-formula-maestra-arquitectura.md](paso-02-formula-maestra-arquitectura/02-fuentes-formula-maestra-arquitectura.md) |
| 03 — Matriz base | [03-fuentes-matriz-base.md](paso-03-matriz-base/03-fuentes-matriz-base.md) |
| 04 — URL Rules | [04-fuentes-url-rules.md](paso-04-url-rules/04-fuentes-url-rules.md) |
| 05 — Page Type Rules | [05-fuentes-page-type-rules.md](paso-05-page-type-rules/05-fuentes-page-type-rules.md) |
| 06 — Estructura contenido y LCA | [06-fuentes-estructura-contenido-areas-cobertura-local.md](paso-06-estructura-contenido-areas-cobertura-local/06-fuentes-estructura-contenido-areas-cobertura-local.md) |
| 07 — Internal Linking Rules | [07-fuentes-internal-linking-rules.md](paso-07-internal-linking-rules/07-fuentes-internal-linking-rules.md) |
| 08 — Priority Score | [08-fuentes-priority-score.md](paso-08-priority-score/08-fuentes-priority-score.md) |
| 09 — QA Checklist | [09-fuentes-qa-checklist.md](paso-09-qa-checklist/09-fuentes-qa-checklist.md) |
| 10 — Producción en fases | [10-fuentes-produccion-en-fases.md](paso-10-produccion-en-fases/10-fuentes-produccion-en-fases.md) |
| 11 — Pseudocódigo | [11-fuentes-pseudocodigo-sistema.md](paso-11-pseudocodigo-sistema/11-fuentes-pseudocodigo-sistema.md) |
| 12 — Master Prompt | [12-fuentes-master-prompt.md](paso-12-master-prompt/12-fuentes-master-prompt.md) |
| 13 — Sistema final operativo | [13-fuentes-sistema-final-operativo.md](paso-13-sistema-final-operativo/13-fuentes-sistema-final-operativo.md) |
| 14 — GBP Creation & Website Alignment | [14-fuentes-gbp-creation-website-alignment.md](paso-14-gbp-creation-website-alignment/14-fuentes-gbp-creation-website-alignment.md) |

---

## Estructura de cada tabla

Cada archivo usa 5 columnas:

```
ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo
```

---

## Cómo rellenar las columnas de fuente

Las columnas **Fuente para la decisión** y **Funcionamiento de la fuente** están vinculadas. Para cada valor de fuente hay una frase fija de funcionamiento.

**Pasos:**
1. Elige el valor de fuente de la tabla de abajo.
2. Copia la frase fija correspondiente en "Funcionamiento de la fuente".
3. Si hay un matiz específico, añádelo al final separado por un punto.

### Tabla de referencia

| Fuente para la decisión | Funcionamiento de la fuente |
|---|---|
| Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. |
| GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. |
| Input humano + GMB Crush | El cliente proporciona el dato y el framework determina cómo usarlo. |
| Geografía | Se deriva de la ubicación física del negocio o de la proximidad geográfica a la Main City. |
| Input humano + Geografía | El cliente aporta la dirección y la geografía determina las zonas de cobertura. |
| GMB Crush + Geografía | El framework define el uso de zonas; la geografía determina cuáles aplican. |
| Datos de búsqueda | Se valida con volumen de búsqueda real. Requiere keyword research antes de confirmar. |
| Competidores | Se valida con análisis de competencia. Requiere revisión antes de confirmar. |
| IA sin respaldo | Valor generado para el ejemplo sin dato real. Debe sustituirse en ejecución real. |
| GMB Crush + IA sin respaldo | El patrón es del framework pero el valor concreto está pendiente de validación. |
| Input humano + IA sin respaldo | El dato base es del cliente pero algún campo concreto está pendiente de confirmación. |

---

## Resumen del ejemplo Cerrajeros Madrid 24h (334 decisiones)

| Fuente | Cantidad | % |
|---|---:|---:|
| GMB Crush (pura) | ~218 | 65% |
| GMB Crush + IA sin respaldo | ~13 | 4% |
| Geografía | ~6 | 2% |
| Input humano | ~0 pura | — |
| Datos de búsqueda | 0 | 0% |
| Competidores | 0 | 0% |
| IA sin respaldo | ~97 | 29% |

**Hallazgos principales:**
- 0 decisiones citan Datos de búsqueda o Competidores en todo el sistema.
- Pasos 4, 5, 6, 7, 11 y 13 son framework puro (0% IA sin respaldo).
- Pasos 1, 3 y 14 concentran la mayor parte de IA sin respaldo.
- Los focos principales de IA sin respaldo son: 8 Candidate LCAs, 15 GeoArticle topics, 6 Priority Scores y 6 Q&A + Posts del GBP.
