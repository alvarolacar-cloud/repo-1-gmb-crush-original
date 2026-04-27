# Paso 6 — Estructura de Contenido + Local Coverage Areas

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

## Bloque 1 — Main City y Local Coverage Areas

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 6.01 | Se decide que Madrid crea la estructura principal | Madrid | Input humano + GMB Crush | Madrid viene de dirección; GMB estructura por ciudad. | Validada |
| 6.02 | Se decide que Direct LCA refuercen el contenido | Almagro, Chamberí | Input humano + Geografía | Ambas salen del NAP/dirección. | Validada |
| 6.03 | Se decide que Candidate LCA puedan usarse si pasan test GEO | Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad | Geografía | Son candidatas; requieren validación de proximidad/datos/competencia. | Pendiente de validación |
| 6.04 | Se decide que las LCA no sustituyan a Madrid | La página sigue siendo Madrid | GMB Crush | Las páginas son city/service; zonas son señales GEO. | Validada |

## Bloque 2 — Uso por tipo de página

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 6.05 | Se decide que la Homepage pueda mencionar LCA de forma ligera | Almagro, Chamberí, etc. | GMB Crush | Homepage establece dónde opera; menciones deben ser secundarias. | Validada |
| 6.06 | Se decide que Service Overview no use LCA | Sin zonas locales | GMB Crush | Service Overview es no geolocalizada. | Validada |
| 6.07 | Se decide que LBS use LCA en intro, H2s y FAQs | Páginas servicio + Madrid | GMB Crush | Location pages permiten geo-specific paragraph, neighborhoods/local issues. | Validada |
| 6.08 | Se decide que GeoHub use sección de cobertura local | /madrid/ | GMB Crush | GeoHub puede incluir neighborhood coverage. | Validada |
| 6.09 | Se decide que Additional Category use cobertura local como contexto | /cerrajero/madrid/duplicado-llaves/ | GMB Crush | Additional Category Page debe ser local y GEO-optimizada. | Validada |
| 6.10 | Se decide que GeoArticles usen zonas como ejemplos locales | Madrid + zonas GEO | GMB Crush | GeoArticles incluyen local references/landmarks/neighborhoods. | Validada |

## Bloque 3 — Restricciones

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 6.11 | Se decide que una mención de zona no equivale a crear URL | Mencionar Almagro ≠ crear /almagro/ | GMB Crush | La arquitectura base no crea URLs por zona. | Validada |
| 6.12 | Se decide no afirmar oficina física en cada LCA | No oficina en Salamanca/Retiro salvo verdad | GMB Crush | GeoArticles y páginas locales no deben fingir ubicación física. | Validada |
| 6.13 | Se decide que areaServed pueda incluir cobertura real validada | Madrid + zonas validadas | GMB Crush + Geografía | Schema debe reflejar cobertura real/validada, no aspiracional. | Parcialmente validada |

