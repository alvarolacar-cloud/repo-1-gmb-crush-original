# Paso 3 — Matriz Base

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

## Bloque 1 — Estructura de la matriz

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.01 | Se decide crear una matriz operativa para controlar las URLs | URL Matrix | GMB Crush | La metodología requiere controlar páginas, URLs, schema, links y fases. | Validada |
| 3.02 | Se decide que cada página tenga un ID único | HP, SO, GH, LBS, AC, GA | GMB Crush | IDs permiten controlar tipos de página y evitar duplicados. | Validada |
| 3.03 | Se decide incluir columnas de producción | URL, H1, Meta Title, Schema, Priority, Phase, Status | GMB Crush | Cada página debe tener función, metadata, schema, prioridad y fase. | Validada |

## Bloque 2 — Homepage y páginas auxiliares

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.04 | Se decide incluir la Homepage en la matriz | HP-001 | GMB Crush | Homepage es Root Entity Anchor. | Validada |
| 3.05 | Se decide que la Homepage use la raíz | / | GMB Crush | El framework define la homepage en root domain. | Validada |
| 3.06 | Se decide incluir página de contacto como auxiliar | /contacto/ | GMB Crush | La homepage y otras páginas deben enlazar a contacto; no es URL SEO base. | Validada |

## Bloque 3 — Service Overview Pages

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.07 | Se decide crear Service Overview para Cerrajero urgente | /cerrajero/cerrajero-urgente/ | GMB Crush + IA sin respaldo | Patrón GMB; servicio pendiente de validación. | Parcialmente validada |
| 3.08 | Se decide crear Service Overview para Apertura de puertas | /cerrajero/apertura-puertas/ | GMB Crush + IA sin respaldo | Patrón GMB; servicio pendiente de validación. | Parcialmente validada |
| 3.09 | Se decide crear Service Overview para Cambio de cerraduras | /cerrajero/cambio-cerraduras/ | GMB Crush + IA sin respaldo | Patrón GMB; servicio pendiente de validación. | Parcialmente validada |
| 3.10 | Se decide crear Service Overview para Cambio de bombines | /cerrajero/cambio-bombines/ | GMB Crush + IA sin respaldo | Patrón GMB; servicio pendiente de validación. | Parcialmente validada |
| 3.11 | Se decide crear Service Overview para Instalación de cerraduras de seguridad | /cerrajero/instalacion-cerraduras-seguridad/ | GMB Crush + IA sin respaldo | Patrón GMB; servicio pendiente de validación. | Parcialmente validada |

## Bloque 4 — GeoHub y Location-Based Service Pages

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.12 | Se decide crear el GeoHub principal de Madrid | /madrid/ | GMB Crush + Input humano | GeoHub por Main City; Madrid viene del input. | Validada |
| 3.13 | Se decide crear LBS de Cerrajero urgente en Madrid | /cerrajero/madrid/cerrajero-urgente/ | GMB Crush + IA sin respaldo | Patrón /category/city/service/ validado; servicio pendiente. | Parcialmente validada |
| 3.14 | Se decide crear LBS de Apertura de puertas en Madrid | /cerrajero/madrid/apertura-puertas/ | GMB Crush + IA sin respaldo | Patrón validado; servicio pendiente. | Parcialmente validada |
| 3.15 | Se decide crear LBS de Cambio de cerraduras en Madrid | /cerrajero/madrid/cambio-cerraduras/ | GMB Crush + IA sin respaldo | Patrón validado; servicio pendiente. | Parcialmente validada |
| 3.16 | Se decide crear LBS de Cambio de bombines en Madrid | /cerrajero/madrid/cambio-bombines/ | GMB Crush + IA sin respaldo | Patrón validado; servicio pendiente. | Parcialmente validada |
| 3.17 | Se decide crear LBS de Instalación de cerraduras de seguridad en Madrid | /cerrajero/madrid/instalacion-cerraduras-seguridad/ | GMB Crush + IA sin respaldo | Patrón validado; servicio pendiente. | Parcialmente validada |

## Bloque 5 — Additional Category Page

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.18 | Se decide crear página de duplicado de llaves en Madrid | /cerrajero/madrid/duplicado-llaves/ | GMB Crush + IA sin respaldo | Additional Category Page está respaldada; categoría concreta pendiente. | Parcialmente validada |

## Bloque 6 — GeoArticles

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.19-3.33 | Se deciden 15 GeoArticles con URLs concretas | 15 URLs /madrid/[topic]/ | GMB Crush + IA sin respaldo | GMB exige 3 ideas por servicio; temas y slugs no están validados con keyword research. | Pendiente de validación |

## Bloque 7 — Tratamiento de Local Coverage Areas

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.34 | Se decide que las LCA aparezcan como notas o campos de contenido | Almagro, Chamberí, Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad | GMB Crush + Geografía | GMB permite señales GEO; directas validadas, candidatas pendientes. | Parcialmente validada |
| 3.35 | Se decide que no haya filas URL para Local Coverage Areas | No /almagro/, no /chamberi/, no /salamanca/ | GMB Crush | LCA no generan URLs salvo Approved Expansion Areas. | Validada |

