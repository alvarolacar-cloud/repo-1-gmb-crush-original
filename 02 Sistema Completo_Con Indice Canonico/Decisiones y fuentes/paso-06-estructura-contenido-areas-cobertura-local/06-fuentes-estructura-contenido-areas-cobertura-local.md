# Paso 6 — Estructura de Contenido + Local Coverage Areas

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

## Bloque 1 — Main City y Local Coverage Areas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 6.01 · Paso-06 §7 Principio 1 Main City crea arquitectura | Se decide que Madrid crea la estructura principal | Input humano + GMB Crush | Madrid viene de la dirección del cliente. GMB Crush estructura toda la arquitectura de contenido por ciudad principal. | Madrid |
| 6.02 · Paso-06 §8 Principio 2 LCA enriquecen contenido | Se decide que Direct LCA refuercen el contenido | Input humano + Geografía | Las Direct LCA (Almagro, Chamberí) salen directamente del NAP/dirección del cliente. Se usan como señales GEO en el contenido. | Almagro, Chamberí |
| 6.03 · Paso-06 §8 Principio 2 LCA enriquecen contenido | Se decide que Candidate LCA puedan usarse si pasan test GEO | Geografía | Las Candidate LCA son zonas próximas con potencial de cobertura. Requieren validación de proximidad, datos y competencia antes de usarse. | Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad |
| 6.04 · Paso-06 §7 Principio 1 Main City crea arquitectura | Se decide que las LCA no sustituyan a Madrid | GMB Crush | Las páginas son city/service. Las zonas son señales GEO en el contenido, no el sujeto principal de la página. | La página sigue siendo Madrid |

## Bloque 2 — Uso por tipo de página

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 6.05 · Paso-06 §21 Homepage con cobertura ligera | Se decide que la Homepage pueda mencionar LCA de forma ligera | GMB Crush | La Homepage establece dónde opera el negocio. Las menciones de zonas deben ser secundarias y no dominar el contenido. | Almagro, Chamberí, etc. |
| 6.06 · Paso-06 §22 Service Overview sin cobertura local | Se decide que Service Overview no use LCA | GMB Crush | La Service Overview es no geolocalizada. No debe incluir referencias a zonas o barrios. | Sin zonas locales |
| 6.07 · Paso-06 §23 Intro local en LBS | Se decide que LBS use LCA en intro, H2s y FAQs | GMB Crush | Las Location-Based Service Pages permiten geo-specific paragraph, neighborhoods y local issues. Es el tipo de página que más aprovecha las LCA. | Páginas servicio + Madrid |
| 6.08 · Paso-06 §26 GeoHub con sección de cobertura principal | Se decide que GeoHub use sección de cobertura local | GMB Crush | El GeoHub puede incluir una sección de neighborhood coverage que liste las zonas de cobertura de la ciudad. | /madrid/ |
| 6.09 · Paso-06 §25 Additional Category con caso local | Se decide que Additional Category use cobertura local como contexto | GMB Crush | La Additional Category Page debe ser local y GEO-optimizada. Las LCA se usan como contexto de servicio. | /cerrajero/madrid/duplicado-llaves/ |
| 6.10 · Paso-06 §27 GeoArticles con ejemplos locales | Se decide que GeoArticles usen zonas como ejemplos locales | GMB Crush | Los GeoArticles incluyen local references, landmarks y neighborhoods como ejemplos concretos en el contenido. | Madrid + zonas GEO |

## Bloque 3 — Restricciones

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 6.11 · Paso-06 §10 Principio 4 Mencionar zona no es crear página | Se decide que una mención de zona no equivale a crear URL | GMB Crush | La arquitectura base no crea URLs por zona. Mencionar Almagro en el contenido no genera /almagro/. | Mencionar Almagro ≠ crear /almagro/ |
| 6.12 · Paso-06 §11 Principio 5 No falsa ubicación | Se decide no afirmar oficina física en cada LCA | GMB Crush | Las páginas locales no deben fingir ubicación física donde no existe. Solo se afirma presencia donde hay evidencia real. | No oficina en Salamanca/Retiro salvo verdad |
| 6.13 · Paso-06 §8 Principio 2 LCA enriquecen contenido | Se decide que areaServed pueda incluir cobertura real validada | GMB Crush + Geografía | El schema areaServed debe reflejar cobertura real y validada, no aspiracional. Las zonas candidatas no se incluyen hasta validación. | Madrid + zonas validadas |
