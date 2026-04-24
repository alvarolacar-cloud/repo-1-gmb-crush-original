**GMB Crush — Paso 02: Fórmula Maestra de Arquitectura**
Versión literal del chat · Sistema GMB Crush para webs locales

Documento generado a partir de la conversación paso a paso sobre el sistema GMB Crush para construir una web local desde cero.


# Índice

**1. Paso 02 — Fórmula Maestra de Arquitectura**


# Paso 2 — Fórmula maestra de arquitectura


## Objetivo del Paso 2


En el Paso 1 recogimos los datos del negocio.

Ahora usamos esos datos para calcular:

Cuántas páginas necesita la web
Qué tipos de páginas hay que crear
Qué páginas son obligatorias
Qué páginas son opcionales o futuras
Qué páginas pueden duplicarse si no tenemos cuidado

Este paso es importante porque GMB Crush no construye una web local como una simple web con “Inicio / Servicios / Contacto”. La estructura se divide en Homepage, Service Overview Pages, Location-Based Service Pages, Additional Category Pages, GeoHub Pages y GeoArticle Pages.


## Lo que tienes que rellenar


Business Name:

Primary GBP Category:

Primary Category Slug:

Main City:

Target Cities:
1.
2.
3.
4.
5.

Core Services:
1.
2.
3.
4.
5.

Additional GBP Categories:
1.
2.
3.

Additional Categories already covered by Core Services:
1.
2.

Additional Categories that need separate pages:
1.
2.

GeoArticles per Service x City:
Default: 3

Does every service apply to every city?
Yes / No

If no, specify exclusions:
- Service:
- City excluded:
- Reason:


## Ejemplo rellenado


Business Name:
ABC Locksmith

Primary GBP Category:
Locksmith

Primary Category Slug:
locksmith

Main City:
Miami

Target Cities:
1. Miami
2. Hialeah
3. Coral Gables
4. Doral
5. Hollywood

Core Services:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying

Additional GBP Categories:
1. Emergency Locksmith Service
2. Key Duplication Service

Additional Categories already covered by Core Services:
1. Emergency Locksmith Service

Additional Categories that need separate pages:
1. Key Duplication Service

GeoArticles per Service x City:
3

Does every service apply to every city?
Yes

Aquí hay un detalle importante.

Emergency Locksmith Service ya está cubierto por el servicio principal Emergency Locksmith. Por eso no crearíamos dos páginas distintas como:

/locksmith/miami/emergency-locksmith/

y además:

/locksmith/miami/emergency-locksmith-service/

Eso puede crear duplicación o canibalización. La página correcta sería una sola:

/locksmith/miami/emergency-locksmith/

Y esa página soportaría tanto el servicio como la categoría adicional del GBP.


## Fórmula maestra


La fórmula base es esta:

1 Homepage
+ S Service Overview Pages
+ C GeoHub Pages
+ S × C Location-Based Service Pages
+ A × C Additional Category Pages
+ G × S × C GeoArticle Pages

Donde:

S = número de servicios principales
C = número de ciudades objetivo
A = número de categorías adicionales que necesitan página separada
G = número de GeoArticles por servicio y ciudad


## Fórmula rellenada con el ejemplo


Para ABC Locksmith:

S = 5 servicios principales
C = 5 ciudades
A = 1 categoría adicional separada
G = 3 GeoArticles por servicio x ciudad

Entonces:

1 Homepage
+ 5 Service Overview Pages
+ 5 GeoHub Pages
+ 5 × 5 Location-Based Service Pages
+ 1 × 5 Additional Category Pages
+ 3 × 5 × 5 GeoArticle Pages

Resultado:

1 Homepage
+ 5 Service Overview Pages
+ 5 GeoHub Pages
+ 25 Location-Based Service Pages
+ 5 Additional Category Pages
+ 75 GeoArticle Pages

Total:

111 páginas estratégicas


## Tabla del inventario de páginas


| Tipo de página | Fórmula | Resultado |
| --- | --- | --- |
| Homepage | 1 | 1 |
| Service Overview Pages | S | 5 |
| GeoHub Pages | C | 5 |
| Location-Based Service Pages | S × C | 25 |
| Additional Category Pages | A × C | 5 |
| GeoArticle Pages | G × S × C | 75 |
| Total | — | 111 |


## Matriz rápida de activación servicio × ciudad


Antes de crear URLs, conviene validar si todos los servicios se ofrecen en todas las ciudades.


| City | Emergency Locksmith | Car Locksmith | Residential Locksmith | Commercial Locksmith | Lock Rekeying |
| --- | --- | --- | --- | --- | --- |
| Miami | YES | YES | YES | YES | YES |
| Hialeah | YES | YES | YES | YES | YES |
| Coral Gables | YES | YES | YES | YES | YES |
| Doral | YES | YES | YES | YES | YES |
| Hollywood | YES | YES | YES | YES | YES |


## Matriz de categorías adicionales


| Additional GBP Category | Already covered by a core service? | Needs separate page? | Notes |
| --- | --- | --- | --- |
| Emergency Locksmith Service | YES | NO | Covered by /locksmith/city/emergency-locksmith/ |
| Key Duplication Service | NO | YES | Needs separate city pages |


## Resultado final del Paso 2


Business: ABC Locksmith
Primary Category: Locksmith
Services: 5
Cities: 5
Effective Additional Categories: 1
GeoArticles per Service x City: 3

Total Pages: 111

El Paso 3 será convertir esto en una matriz base, tipo Google Sheet / Airtable / Notion, donde cada página tendrá su fila con:

Page Type
Service
City
URL
H1
Meta Title
Schema
Priority
Status