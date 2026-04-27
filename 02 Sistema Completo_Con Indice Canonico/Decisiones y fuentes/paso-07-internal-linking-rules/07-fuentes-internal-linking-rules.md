# Paso 7 — Internal Linking Rules

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

## Bloque 1 — Enlaces desde Homepage

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 7.01 · Paso-07 §20 Homepage distribuye autoridad | Homepage enlaza a Service Overview Pages | GMB Crush | La Homepage distribuye autoridad hacia las Service Overview Pages. Es el primer nivel del silo. | 5 Service Overview Pages |
| 7.02 · Paso-07 §20 Homepage distribuye autoridad | Homepage enlaza al GeoHub de Madrid | GMB Crush | La Homepage debe enlazar al Main GeoHub como contenedor de ciudad. | /madrid/ |
| 7.03 · Paso-07 §20 Homepage distribuye autoridad | Homepage enlaza a Additional Category Page | GMB Crush | Las Additional Category Pages deben estar enlazadas desde la Homepage para recibir autoridad. | /cerrajero/madrid/duplicado-llaves/ |
| 7.04 · Paso-07 §20 Homepage distribuye autoridad | Homepage enlaza a contacto | GMB Crush | Contacto es destino operacional obligatorio. Siempre debe estar enlazado desde la Homepage. | /contacto/ |

## Bloque 2 — Enlaces desde Service Overview y LBS

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 7.05 · Paso-07 §21 Service Overview enlaza a su versión local | Service Overview enlaza a versión local en Madrid | GMB Crush | La Service Overview empuja autoridad hacia su versión city/service. Es el enlace descendente del silo. | /cerrajero/[service]/ → /cerrajero/madrid/[service]/ |
| 7.06 · Paso-07 §21 Service Overview enlaza a su versión local | Service Overview enlaza a servicios relacionados | GMB Crush | El cross-linking entre Service Overviews refuerza el silo semántico de servicios. | Cross-links entre servicios |
| 7.07 · Paso-07 §23 LBS enlaza hacia arriba | LBS enlaza a página padre | GMB Crush | La LBS debe enlazar a su parent Service Overview para cerrar el silo. | LBS → Service Overview |
| 7.08 · Paso-07 §23 LBS enlaza hacia arriba | LBS enlaza al GeoHub | GMB Crush | La LBS debe enlazar al GeoHub de la ciudad para reforzar el cluster local. | LBS → /madrid/ |
| 7.09 · Paso-07 §24 LBS enlaza lateralmente | LBS enlaza a servicios relacionados en Madrid | GMB Crush | El enlace lateral entre LBS del mismo city silo refuerza la relevancia local. | LBS → otras LBS |
| 7.10 · Paso-07 §26 GeoArticle enlaza a la landing | LBS enlaza a GeoArticles relacionados | GMB Crush | Los GeoArticles refuerzan la LBS con señales semánticas adicionales. El enlace es bidireccional. | LBS → GeoArticles |

## Bloque 3 — GeoHub y GeoArticles

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 7.11 · Paso-07 §22 GeoHub enlaza a todo el cluster | GeoHub enlaza a todas las LBS de Madrid | GMB Crush | El GeoHub organiza y enlaza todos los servicios de la ciudad. Es el hub del cluster local. | 5 LBS |
| 7.12 · Paso-07 §22 GeoHub enlaza a todo el cluster | GeoHub enlaza a Additional Category Page | GMB Crush | El GeoHub agrupa también las categorías locales adicionales. | /cerrajero/madrid/duplicado-llaves/ |
| 7.13 · Paso-07 §22 GeoHub enlaza a todo el cluster | GeoHub enlaza a GeoArticles | GMB Crush | El GeoHub agrupa todos los artículos ciudad/servicio del cluster. | 15 GeoArticles |
| 7.14 · Paso-07 §26 GeoArticle enlaza a la landing | GeoArticles enlazan a LBS correspondiente | GMB Crush | El interlink GeoArticle → LBS es obligatorio. El GeoArticle pasa relevancia semántica a la landing. | GeoArticle → LBS |
| 7.15 · Paso-07 §26 GeoArticle enlaza a la landing | GeoArticles enlazan al GeoHub | GMB Crush | El interlink GeoArticle → GeoHub es obligatorio. Cierra el cluster de ciudad. | GeoArticle → /madrid/ |

## Bloque 4 — Restricciones de enlaces

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 7.16 · Paso-07 §27 No enlaces a coverage areas sin URL | No enlazar LCA sin URL aprobada | GMB Crush | No se enlaza a URLs inexistentes o no aprobadas. Las LCA solo reciben enlaces si tienen URL propia aprobada. | No enlazar /almagro/ |
| 7.17 · Paso-07 §28 Anchor text variado | Usar anchors contextuales | GMB Crush | Los anchors contextuales evitan el exact-match forzado y son más naturales para el lector y los motores. | Anchors naturales |
| 7.18 · Paso-07 §29 Breadcrumbs como enlace estructural | Usar breadcrumbs | GMB Crush | Los breadcrumbs implementan BreadcrumbList y refuerzan la navegación jerárquica del silo. | Home > Madrid > Servicio |
