# Paso 12 — Master Prompt Reutilizable

Fase 2 de trazabilidad: se añade fuente y funcionamiento a las decisiones del ejemplo **Cerrajeros Madrid 24h**.

Fuentes usadas:

```text
GMB Crush
Input humano
Geografía
Datos de búsqueda
Competidores
IA sin respaldo
```

---

## Bloque 1 — Creación del prompt maestro

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 12.01 · Paso-12 §7 Regla 1 Master Prompt genera sistema completo | Se decide crear un prompt maestro reutilizable | GMB Crush | El sistema debe ser reutilizable y automatizable. El Master Prompt encapsula todo el SOP en un único prompt ejecutable. | Master Prompt GMB Crush |
| 12.02 · Paso-12 §7 Regla 1 Master Prompt genera sistema completo | Se decide que el prompt genere el sistema completo | GMB Crush | El prompt debe reproducir los 14 pasos del SOP. No es un prompt parcial sino el sistema completo. | 14 pasos |

## Bloque 2 — Inputs del prompt

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 12.03 · Paso-12 §8 Regla 2 Main City first | El prompt pide Main City | Input humano + GMB Crush | Madrid es el input del cliente. GMB Crush usa la Main City como base de toda la arquitectura. | Madrid |
| 12.04 · Paso-12 §9 Regla 3 LCA como señales de contenido | El prompt pide Direct Local Coverage Areas | Input humano + Geografía | Las Direct LCA salen del NAP/dirección del cliente. Se usan como señales GEO en el contenido. | Almagro, Chamberí |
| 12.05 · Paso-12 §9 Regla 3 LCA como señales de contenido | El prompt pide Candidate Local Coverage Areas | Geografía | Las Candidate LCA son zonas próximas con potencial. Requieren validación antes de usarse en producción. | Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad |
| 12.06 · Paso-12 §10 Regla 4 Approved Expansion Areas separadas | El prompt pide Approved Expansion Areas | GMB Crush | Las Expansion Areas son un módulo separado. No hay expansión en la fase base. | None in Phase 1 |
| 12.07 · Paso-12 §17 Master Prompt completo | El prompt pide GBP Status | Input humano | El estado del GBP es un input del cliente. Determina qué pasos del GBP están activos. | Not Created |
| 12.08 · Paso-12 §17 Master Prompt completo | El prompt pide Planned Primary GBP Category | Input humano + GMB Crush | La categoría principal planificada deriva del nombre y servicio principal del negocio. | Cerrajero |
| 12.09 · Paso-12 §11 Regla 5 Duplicate category detection | El prompt pide Planned Additional GBP Categories | IA sin respaldo | Las categorías adicionales concretas están pendientes de validación con datos reales. | Servicio de cerrajería de urgencia, Servicio de duplicado de llaves |

## Bloque 3 — Outputs del prompt

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 12.10–12.17 · Paso-12 §7 Regla 1 Master Prompt genera sistema completo | El prompt genera matrices, reglas, content architecture, links, score, plan, QA y GBP alignment | GMB Crush | El sistema requiere outputs operativos estructurados para cada capa. El Master Prompt los genera todos en una sola ejecución. | Sí |

## Bloque 4 — Restricciones del prompt

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 12.18 · Paso-12 §22 Rol y restricciones iniciales | No inventar GBP URL | GMB Crush | No se añade sameAs ni GBP URL hasta que el GBP exista y esté verificado. | GBP URL N/A hasta creación |
| 12.19 · Paso-12 §9 Regla 3 LCA como señales de contenido | No crear URLs para LCA por defecto | GMB Crush | Las LCA son señales GEO en el contenido, no URLs. Solo se crean URLs si hay Approved Expansion Areas. | No URLs LCA |
| 12.20 · Paso-12 §22 Rol y restricciones iniciales | Mantener web-first | Input humano + GMB Crush | El flujo web-first está acordado con el cliente y alineado con el framework. La web se construye antes que el GBP. | Web primero, GBP después |
