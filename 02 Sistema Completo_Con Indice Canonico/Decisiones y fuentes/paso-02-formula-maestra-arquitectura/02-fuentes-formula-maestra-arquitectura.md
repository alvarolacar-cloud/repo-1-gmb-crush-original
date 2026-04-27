# Paso 2 — Fórmula Maestra de Arquitectura

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

## Bloque 1 — Alcance de la fórmula base

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.01 | Se decide que la fórmula base se construye sobre una sola Main City | Madrid | GMB Crush + Input humano | GMB Crush estructura la base por ciudad; Madrid viene de la dirección. | Validada |
| 2.02 | Se decide que las Local Coverage Areas no multiplican páginas por defecto | LCA no generan URLs base | GMB Crush | Barrios/zonas se usan como señales GEO; URLs de zona requieren expansión aprobada. | Validada |
| 2.03 | Se decide que las Approved Expansion Areas no entran en la fórmula inicial | None in Phase 1 | GMB Crush | La expansión es opcional y posterior a la base. | Validada |

## Bloque 2 — Servicios incluidos en el cálculo

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.04 | Se define el número de servicios principales usados en la fórmula | S = 5 | IA sin respaldo | El número depende de la lista de servicios, aún pendiente de validación. | Pendiente de validación |
| 2.05 | Se incluye Cerrajero urgente en el cálculo | Cerrajero urgente | IA sin respaldo | Servicio no validado con input/datos/competidores. | Pendiente de validación |
| 2.06 | Se incluye Apertura de puertas en el cálculo | Apertura de puertas | IA sin respaldo | Servicio no validado con input/datos/competidores. | Pendiente de validación |
| 2.07 | Se incluye Cambio de cerraduras en el cálculo | Cambio de cerraduras | IA sin respaldo | Servicio no validado con input/datos/competidores. | Pendiente de validación |
| 2.08 | Se incluye Cambio de bombines en el cálculo | Cambio de bombines | IA sin respaldo | Servicio no validado con input/datos/competidores. | Pendiente de validación |
| 2.09 | Se incluye Instalación de cerraduras de seguridad en el cálculo | Instalación de cerraduras de seguridad | IA sin respaldo | Servicio no validado con input/datos/competidores. | Pendiente de validación |

## Bloque 3 — Páginas generadas por la fórmula

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.10 | Se decide crear una Homepage | 1 Homepage | GMB Crush | Homepage es Root Entity Anchor obligatorio. | Validada |
| 2.11 | Se decide crear una Service Overview Page por cada servicio principal | 5 Service Overview Pages | GMB Crush + IA sin respaldo | La regla es GMB Crush; el número depende de servicios aún pendientes. | Parcialmente validada |
| 2.12 | Se decide crear un GeoHub para la Main City | 1 GeoHub para Madrid | GMB Crush | GeoHub de ciudad como contenedor local. | Validada |
| 2.13 | Se decide crear una LBS por cada servicio principal en Madrid | 5 LBS | GMB Crush + IA sin respaldo | El patrón es GMB Crush; el número depende de servicios pendientes. | Parcialmente validada |
| 2.14 | Se decide crear una Additional Category Page para la categoría adicional efectiva | 1 Additional Category Page | GMB Crush + IA sin respaldo | GMB exige soporte de categorías; categoría concreta pendiente. | Parcialmente validada |

## Bloque 4 — Categorías adicionales efectivas

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.15 | Se decide que Servicio de cerrajería de urgencia no suma como categoría adicional separada | Cubierta por Cerrajero urgente | GMB Crush | Evita duplicar una intención ya cubierta por core service. | Validada |
| 2.16 | Se decide que Servicio de duplicado de llaves cuenta como categoría adicional efectiva | A = 1 | GMB Crush + IA sin respaldo | La lógica es GMB; la categoría concreta no está validada. | Parcialmente validada |

## Bloque 5 — GeoArticles

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.17 | Se decide usar 3 GeoArticles por servicio principal | G = 3 | GMB Crush | GeoArticle framework pide 3 ideas por Service × City pair. | Validada |
| 2.18 | Se decide calcular GeoArticles como G × S | 3 × 5 | GMB Crush + IA sin respaldo | La fórmula es GMB; S depende de servicios no validados. | Parcialmente validada |
| 2.19 | Se calcula el número total de GeoArticles | 15 GeoArticles | GMB Crush + IA sin respaldo | Deriva de G=3 y S=5; S pendiente. | Parcialmente validada |
| 2.20 | Se decide que los GeoArticles se generan para Madrid, no para cada LCA | 15 GeoArticles para Madrid | GMB Crush | GeoArticles son servicio + ciudad + long-tail; LCA no multiplican URLs. | Validada |

## Bloque 6 — Total de páginas SEO base

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.21 | Se calcula el bloque de Homepage | 1 página | GMB Crush | Parte fija de la arquitectura. | Validada |
| 2.22 | Se calcula el bloque de Service Overview Pages | 5 páginas | GMB Crush + IA sin respaldo | Depende de los servicios elegidos. | Parcialmente validada |
| 2.23 | Se calcula el bloque de GeoHub | 1 página | GMB Crush | Un GeoHub para la Main City. | Validada |
| 2.24 | Se calcula el bloque de LBS | 5 páginas | GMB Crush + IA sin respaldo | Depende de los servicios elegidos. | Parcialmente validada |
| 2.25 | Se calcula el bloque de Additional Category Pages | 1 página | GMB Crush + IA sin respaldo | Depende de categoría adicional efectiva pendiente. | Parcialmente validada |
| 2.26 | Se calcula el bloque de GeoArticles | 15 páginas | GMB Crush + IA sin respaldo | Depende de servicios y temas pendientes de keyword research. | Parcialmente validada |
| 2.27 | Se calcula el total de páginas SEO base | 28 páginas SEO base | GMB Crush + IA sin respaldo | La suma es correcta si se aceptan S=5, A=1 y G=3. | Parcialmente validada |
| 2.28 | Se decide que /contacto/ queda fuera del inventario SEO base | Página auxiliar | GMB Crush | Contacto es página operativa, no uno de los 6 tipos SEO principales. | Validada |

