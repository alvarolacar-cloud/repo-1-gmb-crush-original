# Paso 13 — Sistema Final Operativo

Fase 2 de trazabilidad: se añade fuente, justificación y estado a las decisiones del ejemplo **Cerrajeros Madrid 24h**.

Fuentes usadas:

```text
GMB Crush
Input humano
Geografía
Datos de búsqueda
Competidores
IA sin respaldo
```

Estados usados:

```text
Validada
Parcialmente validada
Pendiente de validación
IA sin respaldo
```

---

## Bloque 1 — Consolidación del sistema

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 13.01 | Se consolida el sistema en SOP final | Sistema GMB Crush de 14 pasos | GMB Crush | El sistema debe quedar operativo y secuencial. | Validada |
| 13.02 | El sistema empieza con Intake | Paso 1 | GMB Crush | Primero inputs, luego arquitectura. | Validada |
| 13.03 | El sistema cierra con GBP después de la web | Paso 14 | Input humano + GMB Crush | Web-first acordado. | Validada |

## Bloque 2 — Secuencia operativa

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 13.04-13.14 | Se decide la secuencia de pasos 2 a 12 | Arquitectura → matriz → URL rules → page types → contenido → links → score → QA → producción → pseudocódigo → prompt | GMB Crush | Secuencia lógica para evitar duplicados, huérfanas y outputs incompletos. | Validada |

## Bloque 3 — Outputs finales

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 13.15 | El sistema produce matrices | URL Matrix, Schema Map, Linking Map, QA, Publishing Plan | GMB Crush | Outputs operativos del sistema. | Validada |
| 13.16 | El sistema se optimiza con tracking | GMB Crush Geo Grid, GSC, GA4 | GMB Crush + IA sin respaldo | Tracking recomendado; herramientas específicas deben confirmarse. | Parcialmente validada |
| 13.17 | Local Coverage Areas refuerzan contenido, no URLs | LCA como señales GEO | GMB Crush | Zonas se usan como señales, no URLs por defecto. | Validada |
| 13.18 | Approved Expansion Areas son opcionales | None in Phase 1 | GMB Crush | No expansión sin aprobación. | Validada |

