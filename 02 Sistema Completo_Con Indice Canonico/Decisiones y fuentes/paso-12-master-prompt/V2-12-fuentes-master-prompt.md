# Paso 12 — Master Prompt Reutilizable

Fase 2 de trazabilidad: se añade fuente y funcionamiento a las decisiones del ejemplo **Cerrajeros Madrid 24h**.

Fuentes usadas (jerarquía de prioridad):

```text
IA sin respaldo
IA heredada
Datos de búsqueda
Competidores
GMB Crush
Input humano
```

---

## Bloque 1 — Creación del prompt maestro

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 12.01 · Paso-12 §7 Master Prompt | Se decide crear un prompt maestro reutilizable | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. El Master Prompt empaqueta el sistema completo. | Master Prompt GMB Crush |
| 12.02 · Paso-12 §17 Master Prompt completo | Se decide que el prompt genere el sistema completo | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. El prompt cubre los 14 pasos. | 14 pasos |

## Bloque 2 — Inputs del prompt

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 12.03 · Paso-12 §8 Inputs | Se decide que el prompt pida Main City | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. Madrid heredado del paso 1.20. | Madrid |
| 12.04 · Paso-12 §8 Inputs | Se decide que el prompt pida Direct Local Coverage Areas | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Direct Local Coverage Areas se extraen del ancla física del NAP según paso 1 §35.1. Heredado del paso 1.22–1.23. | Almagro, Chamberí |
| 12.05 · Paso-12 §8 Inputs | Se decide que el prompt pida Candidate Local Coverage Areas | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Candidate Local Coverage Areas se proponen siguiendo el test de coherencia GEO 3/6 (paso 1 §34); requieren validación con datos de búsqueda o competidores antes de uso fuerte. Heredado del paso 1.24–1.31. | Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad |
| 12.06 · Paso-12 §8 Inputs | Se decide que el prompt pida Approved Expansion Areas | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Campo obligatorio del intake. | None in Phase 1 |
| 12.07 · Paso-12 §8 Inputs | Se decide que el prompt pida GBP Status | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. Heredado del paso 1.04. | Not Created |
| 12.08 · Paso-12 §8 Inputs | Se decide que el prompt pida Planned Primary GBP Category | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Categoría principal heredada del paso 1.16. | Cerrajero |
| 12.09 · Paso-12 §8 Inputs | Se decide que el prompt pida Planned Additional GBP Categories | IA heredada (paso 1.17–1.18) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. | Servicio de cerrajería de urgencia, Servicio de duplicado de llaves |

## Bloque 3 — Outputs del prompt

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 12.10 · Paso-12 §17 Outputs | Se decide que el prompt genere URL Matrix | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. URL Matrix es output canónico. | Sí |
| 12.11 · Paso-12 §17 Outputs | Se decide que el prompt genere Page Type Rules | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. | Sí |
| 12.12 · Paso-12 §17 Outputs | Se decide que el prompt genere Content Architecture | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. | Sí |
| 12.13 · Paso-12 §17 Outputs | Se decide que el prompt genere Internal Linking Map | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. | Sí |
| 12.14 · Paso-12 §17 Outputs | Se decide que el prompt genere Priority Score | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. | Sí |
| 12.15 · Paso-12 §17 Outputs | Se decide que el prompt genere Publishing Plan | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. | Sí |
| 12.16 · Paso-12 §17 Outputs | Se decide que el prompt genere QA Checklist | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. | Sí |
| 12.17 · Paso-12 §17 Outputs | Se decide que el prompt genere GBP Creation & Website Alignment | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Cubre el Paso 14. | Paso 14 |

## Bloque 4 — Restricciones del prompt

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 12.18 · Paso-12 §35 Web-First GBP Rule | Se decide que el prompt no invente GBP URL | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Prohíbe inventar GBP URL hasta el Paso 14. | GBP URL N/A hasta creación |
| 12.19 · Paso-12 §22 Reglas operativas | Se decide que el prompt no cree URLs para LCA por defecto | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las LCA no generan URLs por defecto. | No URLs LCA |
| 12.20 · Paso-12 §35 Web-First GBP Rule | Se decide que el prompt mantenga web-first | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Web primero, GBP después. | Web primero, GBP después |
