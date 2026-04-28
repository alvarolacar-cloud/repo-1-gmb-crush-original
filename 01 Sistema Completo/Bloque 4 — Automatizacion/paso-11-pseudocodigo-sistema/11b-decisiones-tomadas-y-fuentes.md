# Paso 11 — Pseudocódigo del Sistema

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

## Bloque 1 — Inputs, slugs y categorías

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 11.01 · Paso-11 §7 Load inputs | Se decide cargar inputs base | GMB Crush | Doctrina GMB Crush | El framework define el bloque 1 del pseudocódigo: cargar inputs del Paso 1. | Business name, URL, NAP, Main City, servicios, LCA, GBP status |
| 11.02 · Paso-11 §8 Normalize slugs | Se decide normalizar slugs | GMB Crush | Doctrina GMB Crush | El framework define las reglas de slugs (lowercase, sin acentos, guiones medios). | Cerrajero urgente → cerrajero-urgente |
| 11.03 · Paso-11 §9 Validate categories | Se decide validar categorías adicionales | GMB Crush | Doctrina GMB Crush | El framework define la regla de clasificación cubierta/necesita página. | Cubierta / necesita página |

## Bloque 2 — Generación base

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 11.04 · Paso-11 §10 Homepage | Se decide generar Homepage | GMB Crush | Doctrina GMB Crush | El framework dicta generar 1 Homepage. | HP-001 |
| 11.05 · Paso-11 §11 Service Overview | Se decide generar Service Overview Pages | GMB Crush | Doctrina GMB Crush | El framework dicta "1 SO por servicio". | 5 páginas |
| 11.06 · Paso-11 §12 GeoHub | Se decide generar GeoHub de Madrid | GMB Crush | Doctrina GMB Crush | El framework dicta 1 GeoHub por Main City. | /madrid/ |
| 11.07 · Paso-11 §13 LBS | Se decide generar LBS de Madrid | GMB Crush | Doctrina GMB Crush | El framework dicta "1 LBS por servicio en Main City". | 5 páginas |
| 11.08 · Paso-11 §14 Additional Category | Se decide generar Additional Category Page efectiva | GMB Crush | Doctrina GMB Crush | El framework dicta crear AC para categoría adicional efectiva. | /cerrajero/madrid/duplicado-llaves/ |
| 11.09 · Paso-11 §15 GeoArticles | Se decide generar GeoArticles | GMB Crush | Doctrina GMB Crush | El framework define G × S = N artículos. | 15 artículos |

## Bloque 3 — Local Coverage Areas y expansión

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 11.10 · Paso-11 §16 Use Local Coverage Areas | Se decide inyectar Local Coverage Areas en contenido y schema | GMB Crush | Doctrina GMB Crush | El framework define que las LCA se inyectan como señales GEO. | LCA como señales GEO |
| 11.11 · Paso-11 §17 Generate expansion only if approved | Se decide no generar expansión si no está aprobada | GMB Crush | Doctrina GMB Crush | El framework define que la expansión solo con Approved Expansion Areas. | Approved Expansion Areas: None |

## Bloque 4 — Enlaces, prioridad, QA y outputs

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 11.12 · Paso-11 §18 Assign internal links | Se decide asignar enlaces internos por tipo de página | GMB Crush | Doctrina GMB Crush | El framework define el Internal Linking Map del Paso 7. | Internal Linking Map |
| 11.13 · Paso-11 §19 Score priority | Se decide calcular prioridad por página | GMB Crush | Doctrina GMB Crush | El framework define el Priority Score del Paso 8. | Priority Score |
| 11.14 · Paso-11 §20 Check dependencies | Se decide comprobar dependencias | GMB Crush | Doctrina GMB Crush | El framework dicta LBS requiere SO + GeoHub publicados antes. | LBS requiere Service Overview + GeoHub |
| 11.15 · Paso-11 §21 Run QA | Se decide ejecutar QA antes de publicar | GMB Crush | Doctrina GMB Crush | El framework define QA gate obligatorio antes de Published. | QA Matrix |
| 11.16 · Paso-11 §22 Output matrices | Se decide producir matrices finales | GMB Crush | Doctrina GMB Crush | El framework define output canónico: 6 matrices. | URL Matrix, Internal Linking Matrix, Schema Map, Priority Score, Publishing Plan, QA Matrix |
