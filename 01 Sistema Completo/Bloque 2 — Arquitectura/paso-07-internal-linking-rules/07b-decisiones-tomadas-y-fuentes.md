# Paso 7 — Internal Linking Rules

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

## Bloque 1 — Enlaces desde Homepage

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 7.01 · Paso-07 §8 Homepage | Se decide que la Homepage enlace a Service Overview Pages | GMB Crush | Doctrina GMB Crush | El framework define Homepage → Services. | 5 Service Overview Pages |
| 7.02 · Paso-07 §8 Homepage | Se decide que la Homepage enlace al GeoHub de Madrid | GMB Crush | Doctrina GMB Crush | El framework define Homepage → GeoHub principal. | /madrid/ |
| 7.03 · Paso-07 §8 Homepage | Se decide que la Homepage enlace a la página de categoría adicional | GMB Crush | Doctrina GMB Crush | El framework define Homepage → Additional Category. | /cerrajero/madrid/duplicado-llaves/ |
| 7.04 · Paso-07 §8 Homepage | Se decide que la Homepage enlace a contacto | GMB Crush | Doctrina GMB Crush | El framework define Homepage → Contact. | /contacto/ |

## Bloque 2 — Enlaces desde Service Overview y LBS

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 7.05 · Paso-07 §9 Service Overview | Se decide que cada Service Overview enlace a su versión local en Madrid | GMB Crush | Doctrina GMB Crush | El framework define SO → LBS local correspondiente. | /cerrajero/[service]/ → /cerrajero/madrid/[service]/ |
| 7.06 · Paso-07 §9 Service Overview | Se decide que Service Overview enlace a servicios relacionados | GMB Crush | Doctrina GMB Crush | El framework define cross-links entre SO. | Cross-links entre servicios |
| 7.07 · Paso-07 §11 LBS | Se decide que LBS enlace a su página padre | GMB Crush | Doctrina GMB Crush | El framework define LBS → Service Overview padre. | LBS → Service Overview |
| 7.08 · Paso-07 §11 LBS | Se decide que LBS enlace al GeoHub | GMB Crush | Doctrina GMB Crush | El framework define LBS → GeoHub Main City. | LBS → /madrid/ |
| 7.09 · Paso-07 §11 LBS | Se decide que LBS enlace a servicios relacionados en Madrid | GMB Crush | Doctrina GMB Crush | El framework define cross-links entre LBS de la misma ciudad. | LBS → otras LBS |
| 7.10 · Paso-07 §11 LBS | Se decide que LBS enlace a GeoArticles relacionados | GMB Crush | Doctrina GMB Crush | El framework define LBS → GeoArticle del mismo servicio. | LBS → GeoArticles |

## Bloque 3 — Enlaces desde GeoHub y GeoArticles

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 7.11 · Paso-07 §10 GeoHub | Se decide que GeoHub enlace a todas las LBS de Madrid | GMB Crush | Doctrina GMB Crush | El framework define que el GeoHub agrupa todo el cluster Main City. | 5 LBS |
| 7.12 · Paso-07 §10 GeoHub | Se decide que GeoHub enlace a Additional Category Page | GMB Crush | Doctrina GMB Crush | El framework define GeoHub → AC del cluster. | /cerrajero/madrid/duplicado-llaves/ |
| 7.13 · Paso-07 §10 GeoHub | Se decide que GeoHub enlace a GeoArticles | GMB Crush | Doctrina GMB Crush | El framework define GeoHub → todos los GeoArticles del cluster. | 15 GeoArticles |
| 7.14 · Paso-07 §13 GeoArticle | Se decide que GeoArticles enlacen a su LBS correspondiente | GMB Crush | Doctrina GMB Crush | El framework define GeoArticle → matching LBS (regla obligatoria). | GeoArticle → LBS |
| 7.15 · Paso-07 §13 GeoArticle | Se decide que GeoArticles enlacen al GeoHub | GMB Crush | Doctrina GMB Crush | El framework define GeoArticle → GeoHub. | GeoArticle → /madrid/ |

## Bloque 4 — Restricciones de enlaces

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 7.16 · Paso-07 §15 Restricciones | Se decide no enlazar Local Coverage Areas sin URL aprobada | GMB Crush | Doctrina GMB Crush | El framework prohíbe enlazar a URLs que no existen ni se han aprobado. | No enlazar /almagro/ |
| 7.17 · Paso-07 §15 Anchors | Se decide usar anchors contextuales | GMB Crush | Doctrina GMB Crush | El framework define anchors variados y contextuales, no manipulativos. | Anchors naturales |
| 7.18 · Paso-07 §19 Breadcrumbs | Se decide usar breadcrumbs | GMB Crush | Doctrina GMB Crush | El framework define breadcrumbs canónicos por page type. | Home > Madrid > Servicio |
