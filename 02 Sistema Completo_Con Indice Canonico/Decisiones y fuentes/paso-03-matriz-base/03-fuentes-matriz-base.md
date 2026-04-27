# Paso 3 — Matriz Base

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

## Bloque 1 — Estructura de la matriz

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.01 · Paso-03 §15 Columnas obligatorias de la URL Matrix | Se decide crear una matriz operativa para controlar las URLs | GMB Crush | GMB Crush requiere controlar páginas, URLs, schema, links y fases en una matriz antes de producir contenido. | URL Matrix |
| 3.02 · Paso-03 §19 ID por tipo de página | Se decide que cada página tenga un ID único | GMB Crush | Los IDs permiten controlar tipos de página, evitar duplicados y referenciar páginas en el sistema de linking. | HP, SO, GH, LBS, AC, GA |
| 3.03 · Paso-03 §15 Columnas obligatorias de la URL Matrix | Se decide incluir columnas de producción | GMB Crush | Cada página debe tener función, metadata, schema, prioridad y fase asignados desde la matriz antes de producción. | URL, H1, Meta Title, Schema, Priority, Phase, Status |

## Bloque 2 — Homepage y páginas auxiliares

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.04 · Paso-03 §7 Regla 1 | Se decide incluir la Homepage en la matriz | GMB Crush | La Homepage es el Root Entity Anchor. Siempre tiene fila en la matriz. | HP-001 |
| 3.05 · Paso-03 §7 Regla 1 | Se decide que la Homepage use la raíz | GMB Crush | El framework define la homepage en root domain. No tiene slug. | / |
| 3.06 · Paso-03 §17 Filas que NO se generan en la base | Se decide incluir página de contacto como auxiliar | GMB Crush | La homepage y otras páginas enlazan a contacto. No es URL SEO base pero debe existir como página operativa. | /contacto/ |

## Bloque 3 — Service Overview Pages

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.07 · Paso-03 §7 Regla 1 | Se decide crear Service Overview para Cerrajero urgente | GMB Crush + IA sin respaldo | El patrón de URL es GMB Crush. El servicio concreto está pendiente de validación con datos reales. | /cerrajero/cerrajero-urgente/ |
| 3.08 · Paso-03 §7 Regla 1 | Se decide crear Service Overview para Apertura de puertas | GMB Crush + IA sin respaldo | El patrón de URL es GMB Crush. El servicio concreto está pendiente de validación. | /cerrajero/apertura-puertas/ |
| 3.09 · Paso-03 §7 Regla 1 | Se decide crear Service Overview para Cambio de cerraduras | GMB Crush + IA sin respaldo | El patrón de URL es GMB Crush. El servicio concreto está pendiente de validación. | /cerrajero/cambio-cerraduras/ |
| 3.10 · Paso-03 §7 Regla 1 | Se decide crear Service Overview para Cambio de bombines | GMB Crush + IA sin respaldo | El patrón de URL es GMB Crush. El servicio concreto está pendiente de validación. | /cerrajero/cambio-bombines/ |
| 3.11 · Paso-03 §7 Regla 1 | Se decide crear Service Overview para Instalación de cerraduras de seguridad | GMB Crush + IA sin respaldo | El patrón de URL es GMB Crush. El servicio concreto está pendiente de validación. | /cerrajero/instalacion-cerraduras-seguridad/ |

## Bloque 4 — GeoHub y Location-Based Service Pages

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.12 · Paso-03 §21 Main City como campo geográfico base | Se decide crear el GeoHub principal de Madrid | GMB Crush + Input humano | El GeoHub se crea por Main City. Madrid viene del input del cliente. | /madrid/ |
| 3.13 · Paso-03 §7 Regla 1 | Se decide crear LBS de Cerrajero urgente en Madrid | GMB Crush + IA sin respaldo | El patrón /category/city/service/ es GMB Crush. El servicio concreto está pendiente de validación. | /cerrajero/madrid/cerrajero-urgente/ |
| 3.14 · Paso-03 §7 Regla 1 | Se decide crear LBS de Apertura de puertas en Madrid | GMB Crush + IA sin respaldo | El patrón es GMB Crush. El servicio concreto está pendiente de validación. | /cerrajero/madrid/apertura-puertas/ |
| 3.15 · Paso-03 §7 Regla 1 | Se decide crear LBS de Cambio de cerraduras en Madrid | GMB Crush + IA sin respaldo | El patrón es GMB Crush. El servicio concreto está pendiente de validación. | /cerrajero/madrid/cambio-cerraduras/ |
| 3.16 · Paso-03 §7 Regla 1 | Se decide crear LBS de Cambio de bombines en Madrid | GMB Crush + IA sin respaldo | El patrón es GMB Crush. El servicio concreto está pendiente de validación. | /cerrajero/madrid/cambio-bombines/ |
| 3.17 · Paso-03 §7 Regla 1 | Se decide crear LBS de Instalación de cerraduras de seguridad en Madrid | GMB Crush + IA sin respaldo | El patrón es GMB Crush. El servicio concreto está pendiente de validación. | /cerrajero/madrid/instalacion-cerraduras-seguridad/ |

## Bloque 5 — Additional Category Page

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.18 · Paso-03 §7 Regla 1 | Se decide crear página de duplicado de llaves en Madrid | GMB Crush + IA sin respaldo | La Additional Category Page sigue el mismo patrón LBS. La categoría concreta está pendiente de validación. | /cerrajero/madrid/duplicado-llaves/ |

## Bloque 6 — GeoArticles

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.19–3.33 · Paso-03 §7 Regla 1 | Se deciden 15 GeoArticles con URLs concretas | GMB Crush + IA sin respaldo | GMB Crush establece 3 ideas por servicio. Los temas y slugs concretos no están validados con keyword research. | 15 URLs /madrid/[topic]/ |

## Bloque 7 — Tratamiento de Local Coverage Areas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.34 · Paso-03 §8 Regla 2 | Se decide que las LCA aparezcan como notas o campos de contenido | GMB Crush + Geografía | GMB Crush permite señales GEO en contenido. Las Direct LCA están validadas por la dirección; las Candidate LCA están pendientes de test GEO. | Almagro, Chamberí, Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad |
| 3.35 · Paso-03 §8 Regla 2 | Se decide que no haya filas URL para Local Coverage Areas | GMB Crush | GMB Crush establece que las LCA no generan URLs salvo que sean Approved Expansion Areas. | No /almagro/, no /chamberi/, no /salamanca/ |
