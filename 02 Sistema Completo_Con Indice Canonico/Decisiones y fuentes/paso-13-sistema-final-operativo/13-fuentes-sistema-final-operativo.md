# Paso 13 — Sistema Final Operativo

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

## Bloque 1 — Consolidación del sistema

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 13.01 · Paso-13 §19 Índice final del sistema | Se consolida el sistema en SOP final | GMB Crush | El sistema debe quedar operativo y secuencial. El Paso 13 es la consolidación de todos los pasos anteriores en un SOP ejecutable. | Sistema GMB Crush de 14 pasos |
| 13.02 · Paso-13 §7 Sistema 1 Intake | El sistema empieza con Intake | GMB Crush | Primero se cargan los inputs del cliente. Sin inputs validados no se genera arquitectura. | Paso 1 |
| 13.03 · Paso-13 §25 Operating workflow completo | El sistema cierra con GBP después de la web | Input humano + GMB Crush | El flujo web-first está acordado con el cliente y alineado con el framework. El GBP se crea en el Paso 14, después de la web. | Paso 14 |

## Bloque 2 — Secuencia operativa

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 13.04–13.14 · Paso-13 §8–§18 Sistemas 2 a 12 | Se decide la secuencia de pasos 2 a 12 | GMB Crush | La secuencia lógica del framework evita duplicados, páginas huérfanas y outputs incompletos. Cada paso depende del anterior. | Arquitectura → matriz → URL rules → page types → contenido → links → score → QA → producción → pseudocódigo → prompt |

## Bloque 3 — Outputs finales

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 13.15 · Paso-13 §25 Operating workflow completo | El sistema produce matrices | GMB Crush | Los outputs operativos del sistema son matrices estructuradas. No son documentos de texto libre sino tablas ejecutables. | URL Matrix, Schema Map, Linking Map, QA, Publishing Plan |
| 13.16 · Paso-13 §25 Operating workflow completo | El sistema se optimiza con tracking | GMB Crush + IA sin respaldo | GMB Crush recomienda las herramientas de tracking. La disponibilidad real de cada herramienta debe confirmarse en ejecución. | GMB Crush Geo Grid, GSC, GA4 |
| 13.17 · Paso-13 §24 Local Coverage Areas en contenido | Local Coverage Areas refuerzan contenido, no URLs | GMB Crush | Las zonas se usan como señales GEO en el contenido. No generan URLs por defecto. Solo se crean URLs si hay Approved Expansion Areas. | LCA como señales GEO |
| 13.18 · Paso-13 §25 Operating workflow completo | Approved Expansion Areas son opcionales | GMB Crush | No se activa la expansión geográfica sin aprobación explícita. La expansión es un módulo posterior a la fase base. | None in Phase 1 |
