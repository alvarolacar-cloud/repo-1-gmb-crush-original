**GMB Crush — Paso 08: Priority Score**
Versión literal del chat · Sistema GMB Crush para webs locales

Documento generado a partir de la conversación paso a paso sobre el sistema GMB Crush para construir una web local desde cero.


# Índice

**1. Paso 07 — Priority Score**


# Paso 8 — Priority Score


## Objetivo del Paso 7


Ahora decidimos qué páginas se publican primero.

Hasta ahora hemos generado la arquitectura completa. En el ejemplo de ABC Locksmith teníamos:

111 páginas estratégicas

Pero no tiene sentido publicar las 111 de golpe.

Primero publicamos las páginas que tienen mayor impacto en:

Ingresos
Intención comercial
Categoría GBP
Ciudad principal
Probabilidad de conversión
Soporte al Local 3-Pack


## Lo que tienes que rellenar


Para cada servicio y ciudad, rellenas esto:

Business Name:

Primary GBP Category:

Main City:

Service:

City:

Page Type:
Homepage / Service Overview / GeoHub / Location-Based Service / Additional Category / GeoArticle

Revenue Value:
1 / 2 / 3 / 4 / 5

Search Intent:
1 / 2 / 3 / 4 / 5

GBP Category Relevance:
1 / 2 / 3 / 4 / 5

City Priority:
1 / 2 / 3 / 4 / 5

Competition Gap:
1 / 2 / 3 / 4 / 5

Conversion Urgency:
1 / 2 / 3 / 4 / 5

Existing Page?
Yes / No

Existing Ranking?
None / Low / Medium / High

Notes:


## Ejemplo rellenado


Business Name:
ABC Locksmith

Primary GBP Category:
Locksmith

Main City:
Miami

Service:
Emergency Locksmith

City:
Miami

Page Type:
Location-Based Service

Revenue Value:
5

Search Intent:
5

GBP Category Relevance:
5

City Priority:
5

Competition Gap:
4

Conversion Urgency:
5

Existing Page?
No

Existing Ranking?
None

Notes:
Emergency locksmith is high-value, urgent, directly aligned with locksmith intent, and important for Miami Local Pack visibility.


## Fórmula del Priority Score


Usaría esta fórmula simple:

Priority Score =
Revenue Value
+ Search Intent
+ GBP Category Relevance
+ City Priority
+ Competition Gap
+ Conversion Urgency

Cada factor se puntúa de 1 a 5.

El máximo es:

30 puntos


## Cómo interpretar el score


| Score | Prioridad | Qué significa |
| --- | --- | --- |
| 26–30 | P1 | Publicar inmediatamente |
| 21–25 | P2 | Publicar en la primera fase |
| 16–20 | P3 | Publicar después de las páginas core |
| 10–15 | P4 | Publicar como expansión |
| 0–9 | Hold | No construir todavía |


## Qué significa cada factor


### Revenue Value


Mide cuánto dinero puede generar ese servicio.


| Score | Significado |
| --- | --- |
| 1 | Bajo valor económico |
| 2 | Ticket pequeño |
| 3 | Ticket medio |
| 4 | Buen margen |
| 5 | Alto margen o servicio muy rentable |


Ejemplo:

Emergency Locksmith = 5
Key Duplication = 2
Lock Rekeying = 4
Commercial Locksmith = 5


### Search Intent


Mide si la búsqueda suele venir de alguien preparado para comprar.


| Score | Significado |
| --- | --- |
| 1 | Informativo |
| 2 | Investigación temprana |
| 3 | Comparación |
| 4 | Intención comercial clara |
| 5 | Urgencia / compra inmediata |


Ejemplo:

emergency locksmith in Miami = 5
how much does a locksmith cost = 3
what is lock rekeying = 2


### GBP Category Relevance


Mide cuánto apoya esa página a la categoría principal o adicional del GBP.


| Score | Significado |
| --- | --- |
| 1 | Relación débil con GBP |
| 2 | Relación secundaria |
| 3 | Servicio relacionado |
| 4 | Categoría adicional |
| 5 | Categoría principal o servicio core directo |


### City Priority


Mide la importancia de esa ciudad para el negocio.


| Score | Significado |
| --- | --- |
| 1 | Ciudad secundaria lejana |
| 2 | Ciudad pequeña |
| 3 | Ciudad útil |
| 4 | Ciudad importante |
| 5 | Ciudad principal / GBP location |


Ejemplo:

Miami = 5
Hialeah = 4
Coral Gables = 4
Doral = 3
Hollywood = 3


### Competition Gap


Mide si hay oportunidad de competir.


| Score | Significado |
| --- | --- |
| 1 | Competencia muy fuerte y web propia débil |
| 2 | Difícil |
| 3 | Competencia media |
| 4 | Buena oportunidad |
| 5 | Competidores tienen páginas débiles o genéricas |


### Conversion Urgency


Mide si el usuario necesita resolver el problema rápido.


| Score | Significado |
| --- | --- |
| 1 | Sin urgencia |
| 2 | Baja urgencia |
| 3 | Necesidad moderada |
| 4 | Alta intención |
| 5 | Urgente / llamada inmediata |


Ejemplo:

Emergency Locksmith = 5
Car Lockout = 5
Lock Rekeying = 4
Key Duplication = 2


## Priority Score aplicado al ejemplo


### Servicios principales en Miami


| Page Type | URL | Revenue | Intent | GBP | City | Gap | Urgency | Score | Priority |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Location-Based Service | /locksmith/miami/emergency-locksmith/ | 5 | 5 | 5 | 5 | 4 | 5 | 29 | P1 |
| Location-Based Service | /locksmith/miami/car-locksmith/ | 4 | 5 | 4 | 5 | 4 | 5 | 28 | P1 |
| Location-Based Service | /locksmith/miami/commercial-locksmith/ | 5 | 4 | 4 | 5 | 3 | 4 | 26 | P1 |
| Location-Based Service | /locksmith/miami/residential-locksmith/ | 4 | 4 | 4 | 5 | 3 | 4 | 25 | P2 |
| Location-Based Service | /locksmith/miami/lock-rekeying/ | 4 | 4 | 4 | 5 | 3 | 4 | 25 | P2 |
| Additional Category | /locksmith/miami/key-duplication/ | 2 | 3 | 4 | 5 | 3 | 2 | 19 | P3 |


## Resultado


Las primeras páginas comerciales a construir serían:

/locksmith/miami/emergency-locksmith/
/locksmith/miami/car-locksmith/
/locksmith/miami/commercial-locksmith/

Después:

/locksmith/miami/residential-locksmith/
/locksmith/miami/lock-rekeying/

Y luego:

/locksmith/miami/key-duplication/


## Priority Score por tipo de página


### Homepage


La homepage siempre es:

P1

Porque es la raíz de entidad.


### Service Overview Pages


Se priorizan según:

Revenue Value
GBP relevance
Número de páginas locales que soportan

Ejemplo:


| URL | Score | Priority |
| --- | --- | --- |
| /locksmith/emergency-locksmith/ | 29 | P1 |
| /locksmith/car-locksmith/ | 28 | P1 |
| /locksmith/commercial-locksmith/ | 26 | P1 |
| /locksmith/residential-locksmith/ | 25 | P2 |
| /locksmith/lock-rekeying/ | 25 | P2 |


### GeoHub Pages


| URL | City Priority | Strategic Value | Priority |
| --- | --- | --- | --- |
| /miami/ | 5 | 5 | P1 |
| /hialeah/ | 4 | 4 | P2 |
| /coral-gables/ | 4 | 4 | P2 |
| /doral/ | 3 | 3 | P3 |
| /hollywood/ | 3 | 3 | P3 |


## Matriz P1 para ABC Locksmith


| Priority | Page Type | URL | Por qué |
| --- | --- | --- | --- |
| P1 | Homepage | / | Root Entity Anchor |
| P1 | Service Overview | /locksmith/emergency-locksmith/ | Servicio urgente y rentable |
| P1 | Service Overview | /locksmith/car-locksmith/ | Alta intención local |
| P1 | Service Overview | /locksmith/commercial-locksmith/ | Alto valor económico |
| P1 | GeoHub | /miami/ | Ciudad principal |
| P1 | Location-Based Service | /locksmith/miami/emergency-locksmith/ | Máxima urgencia |
| P1 | Location-Based Service | /locksmith/miami/car-locksmith/ | Alta conversión |
| P1 | Location-Based Service | /locksmith/miami/commercial-locksmith/ | Alto ticket |


## Matriz P2 para ABC Locksmith


| Priority | Page Type | URL | Por qué |
| --- | --- | --- | --- |
| P2 | Service Overview | /locksmith/residential-locksmith/ | Servicio core |
| P2 | Service Overview | /locksmith/lock-rekeying/ | Buen valor y relevancia |
| P2 | GeoHub | /hialeah/ | Ciudad secundaria importante |
| P2 | GeoHub | /coral-gables/ | Ciudad secundaria importante |
| P2 | Location-Based Service | /locksmith/miami/residential-locksmith/ | Servicio core en ciudad principal |
| P2 | Location-Based Service | /locksmith/miami/lock-rekeying/ | Alta intención |
| P2 | Location-Based Service | /locksmith/hialeah/emergency-locksmith/ | Urgencia en ciudad secundaria |
| P2 | Location-Based Service | /locksmith/coral-gables/emergency-locksmith/ | Urgencia en ciudad secundaria |


## Matriz P3 para ABC Locksmith


| Priority | Page Type | URL | Por qué |
| --- | --- | --- | --- |
| P3 | GeoHub | /doral/ | Ciudad de expansión |
| P3 | GeoHub | /hollywood/ | Ciudad de expansión |
| P3 | Additional Category | /locksmith/miami/key-duplication/ | Soporte GBP adicional |
| P3 | GeoArticle | /miami/emergency-locksmith-cost-guide/ | Booster para página P1 |
| P3 | GeoArticle | /miami/what-to-do-locked-out-of-house/ | Long-tail + urgencia |
| P3 | GeoArticle | /miami/how-fast-can-locksmith-arrive/ | Soporte AI Overview |


## Reglas anti-error del Paso 7


No publicar primero artículos antes que landings.

Incorrecto:

/miami/emergency-locksmith-cost-guide/

antes de:

/locksmith/miami/emergency-locksmith/

Correcto:

Primero la página comercial.
Después el artículo que la apoya.


## Cómo añadirlo a la matriz del Paso 3


En la URL Matrix, añadimos estas columnas:

Revenue Value
Search Intent
GBP Category Relevance
City Priority
Competition Gap
Conversion Urgency
Total Score
Priority Tier
Publish Phase


## Output final del Paso 7


Sistema de scoring
Prioridad P1 / P2 / P3 / P4
Orden de publicación
Páginas que se construyen primero
Páginas que esperan
Páginas comerciales antes que artículos
Ciudad principal antes que ciudades secundarias
Servicios rentables antes que servicios de bajo ticket
GeoArticles ligados a páginas ya publicadas