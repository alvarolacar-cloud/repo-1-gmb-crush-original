# Paso 2 — Fórmula Maestra de Arquitectura

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

## Bloque 1 — Alcance de la fórmula base

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 2.01 · Paso-02 §8 Fórmula maestra | Se decide que la fórmula base se construye sobre una sola Main City | GMB Crush | Heredado del paso 1.20 | El framework exige una sola Main City. El valor sale del paso 1.20. | Madrid |
| 2.02 · Paso-02 §8 Fórmula maestra | Se decide que las Local Coverage Areas no multiplican páginas por defecto | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Las LCA son señales GEO, no URLs. | Almagro, Chamberí, Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa y Prosperidad no generan URLs base |
| 2.03 · Paso-02 §17 Approved Expansion Areas | Se decide que las Approved Expansion Areas no entran en la fórmula inicial | GMB Crush | Doctrina GMB Crush | El framework define esta regla. La expansión requiere aprobación. | None in Phase 1 |

## Bloque 2 — Servicios incluidos en el cálculo

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 2.04 · Paso-02 §9 core_services | Se define el número de servicios principales usados en la fórmula | GMB Crush | Heredado del paso 1.34–1.38 | El framework define S como el número de core services. El conteo S=5 deriva de los servicios del paso 1. | S = 5 |
| 2.05 · Paso-02 §9 core_services | Se incluye Cerrajero urgente en el cálculo | GMB Crush | Heredado del paso 1.34 | El framework dicta usar los servicios core en la fórmula. Valor heredado. | Cerrajero urgente |
| 2.06 · Paso-02 §9 core_services | Se incluye Apertura de puertas en el cálculo | GMB Crush | Heredado del paso 1.35 | El framework dicta usar los servicios core en la fórmula. Valor heredado. | Apertura de puertas |
| 2.07 · Paso-02 §9 core_services | Se incluye Cambio de cerraduras en el cálculo | GMB Crush | Heredado del paso 1.36 | El framework dicta usar los servicios core en la fórmula. Valor heredado. | Cambio de cerraduras |
| 2.08 · Paso-02 §9 core_services | Se incluye Cambio de bombines en el cálculo | GMB Crush | Heredado del paso 1.37 | El framework dicta usar los servicios core en la fórmula. Valor heredado. | Cambio de bombines |
| 2.09 · Paso-02 §9 core_services | Se incluye Instalación de cerraduras de seguridad en el cálculo | GMB Crush | Heredado del paso 1.38 | El framework dicta usar los servicios core en la fórmula. Valor heredado. | Instalación de cerraduras de seguridad |

## Bloque 3 — Páginas generadas por la fórmula

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 2.10 · Paso-02 §8 Fórmula maestra | Se decide crear una Homepage | GMB Crush | Doctrina GMB Crush | El framework define que la fórmula incluye 1 Homepage como Root Entity Anchor. | 1 Homepage |
| 2.11 · Paso-02 §8 Fórmula maestra | Se decide crear una Service Overview Page por cada servicio principal | GMB Crush | Heredado del paso 1.34–1.38 | El framework dicta "1 SO por servicio". El conteo 5 deriva de los servicios del paso 1. | 5 Service Overview Pages |
| 2.12 · Paso-02 §8 Fórmula maestra | Se decide crear un GeoHub para la Main City | GMB Crush | Doctrina GMB Crush | El framework dicta 1 GeoHub por Main City. | 1 GeoHub para Madrid |
| 2.13 · Paso-02 §8 Fórmula maestra | Se decide crear una Location-Based Service Page por cada servicio principal en Madrid | GMB Crush | Heredado del paso 1.34–1.38 | El framework dicta "1 LBS por servicio en Main City". El conteo 5 deriva de los servicios del paso 1. | 5 LBS |
| 2.14 · Paso-02 §10 Additional Categories | Se decide crear una Additional Category Page para la categoría adicional efectiva | GMB Crush | Heredado del paso 1.18 | El framework dicta crear AC para categoría adicional efectiva. Valor heredado. | 1 Additional Category Page |

## Bloque 4 — Categorías adicionales efectivas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 2.15 · Paso-02 §10 Additional Categories | Se decide que Servicio de cerrajería de urgencia no suma como categoría adicional separada | GMB Crush | Heredado del paso 1.39 | El framework define la regla de consolidación. Valor heredado. | Queda cubierta por Cerrajero urgente |
| 2.16 · Paso-02 §10 Additional Categories | Se decide que Servicio de duplicado de llaves sí cuenta como categoría adicional efectiva | GMB Crush | Heredado del paso 1.40 | El framework define la regla de clasificación. Valor heredado. | A = 1 |

## Bloque 5 — GeoArticles

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 2.17 · Paso-02 §11 GeoArticles | Se decide usar 3 GeoArticles por servicio principal | GMB Crush | Doctrina GMB Crush | El framework establece el default operativo G=3. | G = 3 |
| 2.18 · Paso-02 §11 GeoArticles | Se decide calcular GeoArticles como G × S | GMB Crush | Heredado del paso 1.34–1.38 | El framework define la fórmula G × S. El conteo deriva de los servicios. | 3 × 5 |
| 2.19 · Paso-02 §11 GeoArticles | Se calcula el número total de GeoArticles | GMB Crush | Heredado del paso 1.34–1.38 | El framework define la fórmula G × S. | 15 GeoArticles |
| 2.20 · Paso-02 §11 GeoArticles | Se decide que los GeoArticles se generan para Madrid, no para cada Local Coverage Area | GMB Crush | Doctrina GMB Crush | El framework dicta generar GeoArticles para la Main City. | 15 GeoArticles para Madrid |

## Bloque 6 — Total de páginas SEO base

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 2.21 · Paso-02 §16 Inventario base | Se calcula el bloque de Homepage | GMB Crush | Doctrina GMB Crush | El framework define 1 Homepage. | 1 página |
| 2.22 · Paso-02 §16 Inventario base | Se calcula el bloque de Service Overview Pages | GMB Crush | Heredado del paso 1.34–1.38 | El framework dicta 1 SO por servicio. | 5 páginas |
| 2.23 · Paso-02 §16 Inventario base | Se calcula el bloque de GeoHub | GMB Crush | Doctrina GMB Crush | El framework define 1 GeoHub por Main City. | 1 página |
| 2.24 · Paso-02 §16 Inventario base | Se calcula el bloque de Location-Based Service Pages | GMB Crush | Heredado del paso 1.34–1.38 | El framework dicta 1 LBS por servicio en Main City. | 5 páginas |
| 2.25 · Paso-02 §16 Inventario base | Se calcula el bloque de Additional Category Pages | GMB Crush | Heredado del paso 1.18 | El framework dicta 1 AC por categoría adicional efectiva. | 1 página |
| 2.26 · Paso-02 §16 Inventario base | Se calcula el bloque de GeoArticles | GMB Crush | Heredado del paso 1.34–1.38 | El framework define G × S. | 15 páginas |
| 2.27 · Paso-02 §16 Inventario base | Se calcula el total de páginas SEO base | GMB Crush | Heredado del paso 1.34–1.38 | El framework define la fórmula 1+S+1+S+A+G×S. El total 28 depende de S=5 y A=1, ambos heredados del paso 1. | 28 páginas SEO base |
| 2.28 · Paso-02 §16 Inventario base | Se decide que `/contacto/` queda fuera del inventario SEO base | GMB Crush | Doctrina GMB Crush | El framework define que la página de contacto es auxiliar. | Página auxiliar |
