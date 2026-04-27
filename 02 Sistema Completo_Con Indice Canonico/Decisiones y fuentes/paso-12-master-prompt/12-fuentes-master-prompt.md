# Paso 12 — Master Prompt Reutilizable

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

## Bloque 1 — Creación del prompt maestro

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 12.01 | Se decide crear un prompt maestro reutilizable | Master Prompt GMB Crush | GMB Crush | El sistema debe ser reutilizable y automatizable. | Validada |
| 12.02 | Se decide que el prompt genere el sistema completo | 14 pasos | GMB Crush | El prompt debe reproducir todo el SOP. | Validada |

## Bloque 2 — Inputs del prompt

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 12.03 | El prompt pide Main City | Madrid | Input humano + GMB Crush | Madrid es input; GMB usa ciudad como base. | Validada |
| 12.04 | El prompt pide Direct Local Coverage Areas | Almagro, Chamberí | Input humano + Geografía | Salen del NAP/dirección. | Validada |
| 12.05 | El prompt pide Candidate Local Coverage Areas | Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad | Geografía | Candidatas; requieren validación. | Pendiente de validación |
| 12.06 | El prompt pide Approved Expansion Areas | None in Phase 1 | GMB Crush | No hay expansión inicial. | Validada |
| 12.07 | El prompt pide GBP Status | Not Created | Input humano | Situación inicial acordada. | Validada |
| 12.08 | El prompt pide Planned Primary GBP Category | Cerrajero | Input humano + GMB Crush | Deriva del nombre/categoría principal planificada. | Parcialmente validada |
| 12.09 | El prompt pide Planned Additional GBP Categories | Servicio de cerrajería de urgencia, Servicio de duplicado de llaves | IA sin respaldo | Categorías concretas pendientes de validación. | Pendiente de validación |

## Bloque 3 — Outputs del prompt

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 12.10-12.17 | El prompt genera matrices, reglas, content architecture, links, score, plan, QA y GBP alignment | Sí | GMB Crush | El sistema requiere outputs operativos para cada capa. | Validada |

## Bloque 4 — Restricciones del prompt

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 12.18 | No inventar GBP URL | GBP URL N/A hasta creación | GMB Crush | No sameAs/GBP URL inexistente. | Validada |
| 12.19 | No crear URLs para LCA por defecto | No URLs LCA | GMB Crush | LCA son señales GEO salvo expansión. | Validada |
| 12.20 | Mantener web-first | Web primero, GBP después | Input humano + GMB Crush | Flujo acordado y alineado con sistema. | Validada |

