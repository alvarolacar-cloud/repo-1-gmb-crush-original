# Paso 12 — Master Prompt Reutilizable

Fase 2 de trazabilidad del sistema GMB Crush.

Fuentes permitidas:

```text
GMB Crush
Input humano
Decisión de diseño
IA sin respaldo
IA heredada (paso X.YY)
```

Orígenes del dato permitidos:

```text
Doctrina GMB Crush
Input humano
Competidores
Datos de búsqueda
Decisión de diseño
Heredado del paso X.YY
IA sin respaldo
```

---

## Bloque 1 — Creación del prompt maestro

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 12.01 · Paso-12 §7 Master Prompt | Se decide crear un prompt maestro reutilizable | GMB Crush | Doctrina GMB Crush | El framework define el Master Prompt como empaquetador del sistema. | Master Prompt GMB Crush |
| 12.02 · Paso-12 §17 Master Prompt completo | Se decide que el prompt genere el sistema completo | GMB Crush | Doctrina GMB Crush | El framework define que el prompt cubre los 14 pasos. | 14 pasos |

## Bloque 2 — Inputs del prompt

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 12.03 · Paso-12 §8 Inputs | Se decide que el prompt pida Main City | GMB Crush | Heredado del paso 1.20 | El framework dicta que Main City es input estructural. Valor heredado del paso 1.20. | Madrid |
| 12.04 · Paso-12 §8 Inputs | Se decide que el prompt pida Direct Local Coverage Areas | GMB Crush | Heredado del paso 1.22–1.23 | El framework dicta el campo Direct LCAs. Valor heredado del paso 1.22–1.23. | Almagro, Chamberí |
| 12.05 · Paso-12 §8 Inputs | Se decide que el prompt pida Candidate Local Coverage Areas | GMB Crush | Heredado del paso 1.24–1.31 | El framework dicta el campo Candidate LCAs. Valor heredado del paso 1.24–1.31. | Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad |
| 12.06 · Paso-12 §8 Inputs | Se decide que el prompt pida Approved Expansion Areas | GMB Crush | Doctrina GMB Crush | El framework define el campo Approved Expansion Areas. | None in Phase 1 |
| 12.07 · Paso-12 §8 Inputs | Se decide que el prompt pida GBP Status | GMB Crush | Heredado del paso 1.04 | El framework dicta el campo GBP Status. Valor heredado del paso 1.04. | Not Created |
| 12.08 · Paso-12 §8 Inputs | Se decide que el prompt pida Planned Primary GBP Category | GMB Crush | Heredado del paso 1.16 | El framework dicta el campo Planned Primary GBP Category. Valor heredado del paso 1.16. | Cerrajero |
| 12.09 · Paso-12 §8 Inputs | Se decide que el prompt pida Planned Additional GBP Categories | GMB Crush | Heredado del paso 1.17–1.18 | El framework dicta el campo Planned Additional GBP Categories. Valores heredados del paso 1.17 y 1.18. | Servicio de cerrajería de urgencia, Servicio de duplicado de llaves |

## Bloque 3 — Outputs del prompt

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 12.10 · Paso-12 §17 Outputs | Se decide que el prompt genere URL Matrix | GMB Crush | Doctrina GMB Crush | El framework define URL Matrix como output canónico. | Sí |
| 12.11 · Paso-12 §17 Outputs | Se decide que el prompt genere Page Type Rules | GMB Crush | Doctrina GMB Crush | El framework define Page Type Rules como output canónico. | Sí |
| 12.12 · Paso-12 §17 Outputs | Se decide que el prompt genere Content Architecture | GMB Crush | Doctrina GMB Crush | El framework define Content Architecture como output canónico. | Sí |
| 12.13 · Paso-12 §17 Outputs | Se decide que el prompt genere Internal Linking Map | GMB Crush | Doctrina GMB Crush | El framework define Internal Linking Map como output canónico. | Sí |
| 12.14 · Paso-12 §17 Outputs | Se decide que el prompt genere Priority Score | GMB Crush | Doctrina GMB Crush | El framework define Priority Score como output canónico. | Sí |
| 12.15 · Paso-12 §17 Outputs | Se decide que el prompt genere Publishing Plan | GMB Crush | Doctrina GMB Crush | El framework define Publishing Plan como output canónico. | Sí |
| 12.16 · Paso-12 §17 Outputs | Se decide que el prompt genere QA Checklist | GMB Crush | Doctrina GMB Crush | El framework define QA Checklist como output canónico. | Sí |
| 12.17 · Paso-12 §17 Outputs | Se decide que el prompt genere GBP Creation & Website Alignment | GMB Crush | Doctrina GMB Crush | El framework define el Paso 14 como output canónico. | Paso 14 |

## Bloque 4 — Restricciones del prompt

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 12.18 · Paso-12 §35 Web-First GBP Rule | Se decide que el prompt no invente GBP URL | GMB Crush | Doctrina GMB Crush | El framework prohíbe inventar GBP URL hasta el Paso 14. | GBP URL N/A hasta creación |
| 12.19 · Paso-12 §22 Reglas operativas | Se decide que el prompt no cree URLs para LCA por defecto | GMB Crush | Doctrina GMB Crush | El framework define que las LCA no generan URLs por defecto. | No URLs LCA |
| 12.20 · Paso-12 §35 Web-First GBP Rule | Se decide que el prompt mantenga web-first | GMB Crush | Doctrina GMB Crush | El framework define web primero, GBP después. | Web primero, GBP después |
