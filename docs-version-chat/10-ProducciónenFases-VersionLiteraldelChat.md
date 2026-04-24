**GMB Crush — Paso 10: Producción en Fases**
Versión literal del chat · Sistema GMB Crush para webs locales

Documento generado a partir de la conversación paso a paso sobre el sistema GMB Crush para construir una web local desde cero.


# Índice

**1. Paso 09 — Producción en Fases**


# Paso 10 — Producción en fases


## Objetivo del Paso 9


Ahora convertimos todo el sistema en un plan de implementación real.

Hasta ahora tenemos:

Arquitectura
URLs
Tipos de página
Enlazado interno
Prioridad
QA

Pero ahora necesitamos responder:

Qué se construye primero
Qué se publica después
Qué páginas dependen de otras
Qué páginas no deben publicarse todavía
Cómo evitar publicar contenido sin soporte interno
Cómo escalar sin perder control

La lógica de fases es:

Primero entidad
Después servicios
Después ciudad + servicio
Después artículos
Después optimización


## Lo que tienes que rellenar


Business Name:

Website Root Domain:

Primary GBP Category:

Primary Category Slug:

Main City:

Physical Location City:

Top Priority Cities:
1.
2.
3.
4.
5.

Top Priority Services:
1.
2.
3.
4.
5.

Additional GBP Categories that need pages:
1.
2.
3.

Total Pages Calculated:

Homepage Status:
Not Started / Draft / Published

Service Overview Pages Status:
Not Started / Draft / Published

GeoHub Pages Status:
Not Started / Draft / Published

Location-Based Service Pages Status:
Not Started / Draft / Published

Additional Category Pages Status:
Not Started / Draft / Published

GeoArticle Pages Status:
Not Started / Draft / Published

Publishing Capacity:
How many pages can be produced per week?

Content Team:
Solo / Writer / SEO / Developer / Designer

CMS:
WordPress / Webflow / Shopify / Custom / Other

Can schema be added?
Yes / No

Can internal links be edited manually?
Yes / No

Can Google reviews be embedded?
Yes / No

Can images be added by city/service?
Yes / No

Tracking Available:
GMB Crush Geo Grid / Google Search Console / GA4 / Rank Tracker / None


## Ejemplo rellenado


Business Name:
ABC Locksmith

Website Root Domain:
https://www.abclocksmith.com

Primary GBP Category:
Locksmith

Primary Category Slug:
locksmith

Main City:
Miami

Physical Location City:
Miami

Top Priority Cities:
1. Miami
2. Hialeah
3. Coral Gables
4. Doral
5. Hollywood

Top Priority Services:
1. Emergency Locksmith
2. Car Locksmith
3. Commercial Locksmith
4. Residential Locksmith
5. Lock Rekeying

Additional GBP Categories that need pages:
1. Key Duplication Service

Total Pages Calculated:
111

Homepage Status:
Not Started

Service Overview Pages Status:
Not Started

GeoHub Pages Status:
Not Started

Location-Based Service Pages Status:
Not Started

Additional Category Pages Status:
Not Started

GeoArticle Pages Status:
Not Started

Publishing Capacity:
5 pages per week

Content Team:
SEO + Writer + Developer

CMS:
WordPress

Can schema be added?
Yes

Can internal links be edited manually?
Yes

Can Google reviews be embedded?
Yes

Can images be added by city/service?
Yes

Tracking Available:
GMB Crush Geo Grid, Google Search Console, GA4


## Las 4 fases


Fase 1: Entity Foundation
Fase 2: Local Conversion Layer
Fase 3: Semantic Expansion Layer
Fase 4: Optimization Loop


# Fase 1 — Entity Foundation


## Objetivo


Construir la base mínima para que Google entienda:

Quién es la empresa
Qué categoría GBP tiene
Qué servicios ofrece
Dónde está ubicada
Qué ciudad principal atiende
Cómo se conecta la homepage con los servicios


## Lo que tienes que rellenar


Fase 1 Pages:

Homepage:
URL:
Status:
Priority:

Contact Page:
URL:
Status:
Priority:

About Page:
URL:
Status:
Priority:

Top Service Overview Pages:
1.
2.
3.

Main GeoHub:
URL:

Schema to implement:
1.
2.
3.

Trust elements to add:
1.
2.
3.

NAP location:
Header / Footer / Contact Page / Homepage

Main CTA:


## Ejemplo rellenado


Fase 1 Pages:

Homepage:
URL: /
Status: Planned
Priority: P1

Contact Page:
URL: /contact/
Status: Planned
Priority: P1

About Page:
URL: /about/
Status: Planned
Priority: P2

Top Service Overview Pages:
1. /locksmith/emergency-locksmith/
2. /locksmith/car-locksmith/
3. /locksmith/commercial-locksmith/

Main GeoHub:
URL: /miami/

Schema to implement:
1. Organization
2. WebSite
3. LocalBusiness
4. BreadcrumbList
5. Service

Trust elements to add:
1. 250+ Google reviews
2. Licensed locksmith technicians
3. 10+ years in business
4. Same-day mobile support

NAP location:
Homepage, footer, contact page

Main CTA:
Call ABC Locksmith today


## Fase 1 — Páginas a publicar


| Orden | Page Type | URL | Priority | Motivo |
| --- | --- | --- | --- | --- |
| 1 | Homepage | / | P1 | Raíz de entidad |
| 2 | Contact | /contact/ | P1 | NAP, contacto, confianza |
| 3 | Service Overview | /locksmith/emergency-locksmith/ | P1 | Servicio urgente y rentable |
| 4 | Service Overview | /locksmith/car-locksmith/ | P1 | Alta intención comercial |
| 5 | Service Overview | /locksmith/commercial-locksmith/ | P1 | Alto ticket |
| 6 | GeoHub | /miami/ | P1 | Ciudad principal |
| 7 | About | /about/ | P2 | Refuerzo de entidad y confianza |


## Qué NO publicar todavía


75 GeoArticles
Todas las ciudades secundarias
Todas las páginas de key duplication
Todas las combinaciones servicio × ciudad
Artículos informativos sin landing de destino


# Fase 2 — Local Conversion Layer


## Objetivo


Construir las páginas que van a captar búsquedas comerciales tipo:

emergency locksmith in Miami
car locksmith in Miami
commercial locksmith in Miami
residential locksmith in Hialeah
lock rekeying in Coral Gables


## Lo que tienes que rellenar


Main City:

Main City Service Pages:
1.
2.
3.
4.
5.

Secondary Cities:
1.
2.
3.
4.

Secondary City Priority Service:
Usually: Emergency / highest-converting service

Additional Category Pages for main city:
1.
2.

GeoHub Pages needed:
1.
2.
3.

Dependencies:
Does each service page have a parent Service Overview?
Yes / No

Does each city have a GeoHub?
Yes / No

Does each page have internal links assigned?
Yes / No


## Ejemplo rellenado


Main City:
Miami

Main City Service Pages:
1. /locksmith/miami/emergency-locksmith/
2. /locksmith/miami/car-locksmith/
3. /locksmith/miami/commercial-locksmith/
4. /locksmith/miami/residential-locksmith/
5. /locksmith/miami/lock-rekeying/

Secondary Cities:
1. Hialeah
2. Coral Gables
3. Doral
4. Hollywood

Secondary City Priority Service:
Emergency Locksmith

Additional Category Pages for main city:
1. /locksmith/miami/key-duplication/

GeoHub Pages needed:
1. /hialeah/
2. /coral-gables/
3. /doral/
4. /hollywood/

Dependencies:
Does each service page have a parent Service Overview?
Yes

Does each city have a GeoHub?
Yes, or created before/with first city-service page

Does each page have internal links assigned?
Yes


## Fase 2 — Páginas a publicar


### Bloque A — Main City + Top Services


| Orden | Page Type | URL | Priority |
| --- | --- | --- | --- |
| 1 | Location-Based Service | /locksmith/miami/emergency-locksmith/ | P1 |
| 2 | Location-Based Service | /locksmith/miami/car-locksmith/ | P1 |
| 3 | Location-Based Service | /locksmith/miami/commercial-locksmith/ | P1 |
| 4 | Location-Based Service | /locksmith/miami/residential-locksmith/ | P2 |
| 5 | Location-Based Service | /locksmith/miami/lock-rekeying/ | P2 |


### Bloque B — Additional Category principal


| Orden | Page Type | URL | Priority |
| --- | --- | --- | --- |
| 6 | Additional Category | /locksmith/miami/key-duplication/ | P3 |


### Bloque C — GeoHubs secundarios


| Orden | Page Type | URL | Priority |
| --- | --- | --- | --- |
| 7 | GeoHub | /hialeah/ | P2 |
| 8 | GeoHub | /coral-gables/ | P2 |
| 9 | GeoHub | /doral/ | P3 |
| 10 | GeoHub | /hollywood/ | P3 |


### Bloque D — Secondary City + High-Intent Service


| Orden | Page Type | URL | Priority |
| --- | --- | --- | --- |
| 11 | Location-Based Service | /locksmith/hialeah/emergency-locksmith/ | P2 |
| 12 | Location-Based Service | /locksmith/coral-gables/emergency-locksmith/ | P2 |
| 13 | Location-Based Service | /locksmith/doral/emergency-locksmith/ | P3 |
| 14 | Location-Based Service | /locksmith/hollywood/emergency-locksmith/ | P3 |


# Fase 3 — Semantic Expansion Layer


## Objetivo


Ahora que ya existen las páginas comerciales, creamos contenido de soporte.

Aquí entran los GeoArticles.

Su función es reforzar:

Servicio + Ciudad + Intención long-tail

Ejemplo:

Emergency Locksmith + Miami + Cost Guide


## Lo que tienes que rellenar


Top Service:

Top City:

Matching Location-Based Service Page:

Matching GeoHub Page:

GeoArticle Cluster Name:

GeoArticle Ideas:
1.
2.
3.

Related Article:
1.

Publishing Frequency:
1 article/week
2 articles/month
Other:

Refresh Frequency:
3 months
6 months
Other:

Internal Link Destination:
Primary commercial page URL:
GeoHub URL:
Related article URL:


## Ejemplo rellenado


Top Service:
Emergency Locksmith

Top City:
Miami

Matching Location-Based Service Page:
/locksmith/miami/emergency-locksmith/

Matching GeoHub Page:
/miami/

GeoArticle Cluster Name:
Emergency Locksmith Miami Cluster

GeoArticle Ideas:
1. /miami/emergency-locksmith-cost-guide/
2. /miami/what-to-do-locked-out-of-house/
3. /miami/how-fast-can-locksmith-arrive/

Related Article:
1. /miami/lock-rekeying-vs-lock-replacement/

Publishing Frequency:
1 article/week

Refresh Frequency:
6 months

Internal Link Destination:
Primary commercial page URL:
/locksmith/miami/emergency-locksmith/

GeoHub URL:
/miami/

Related article URL:
/miami/what-to-do-locked-out-of-house/


## Fase 3 — Primer cluster de GeoArticles


| Orden | Page Type | URL | Supports |
| --- | --- | --- | --- |
| 1 | GeoArticle | /miami/emergency-locksmith-cost-guide/ | /locksmith/miami/emergency-locksmith/ |
| 2 | GeoArticle | /miami/what-to-do-locked-out-of-house/ | /locksmith/miami/emergency-locksmith/ |
| 3 | GeoArticle | /miami/how-fast-can-locksmith-arrive/ | /locksmith/miami/emergency-locksmith/ |


## Regla principal


No publicar un GeoArticle si todavía no existe la página comercial que debe apoyar.


# Fase 4 — Optimization Loop


## Objetivo


Después de publicar, entramos en un ciclo de optimización.

Aquí usamos datos reales para mejorar:

Rankings locales
Impresiones
CTR
Conversión
Enlaces internos
Contenido
Schema
FAQs
GeoArticle clusters


## Lo que tienes que rellenar


Tracking Tools:

Geo Grid Tracking:
Yes / No

Google Search Console:
Yes / No

GA4:
Yes / No

GBP Insights:
Yes / No

Main Keywords to Track:
1.
2.
3.
4.
5.

Cities to Track:
1.
2.
3.
4.
5.

Review Frequency:
Weekly / Biweekly / Monthly

Optimization Actions:
1.
2.
3.
4.
5.

Content Refresh Frequency:
3 months / 6 months / 12 months

Pages to Watch:
1.
2.
3.


## Ejemplo rellenado


Tracking Tools:
GMB Crush Geo Grid, Google Search Console, GA4, GBP Insights

Geo Grid Tracking:
Yes

Google Search Console:
Yes

GA4:
Yes

GBP Insights:
Yes

Main Keywords to Track:
1. emergency locksmith Miami
2. car locksmith Miami
3. locksmith Miami
4. emergency locksmith Hialeah
5. lock rekeying Miami

Cities to Track:
1. Miami
2. Hialeah
3. Coral Gables
4. Doral
5. Hollywood

Review Frequency:
Monthly

Optimization Actions:
1. Add FAQs to underperforming pages
2. Improve internal links to pages stuck on page 2
3. Add reviews and trust blocks
4. Add GeoArticles for weak service-city combinations
5. Refresh metadata and schema

Content Refresh Frequency:
6 months

Pages to Watch:
1. /locksmith/miami/emergency-locksmith/
2. /locksmith/miami/car-locksmith/
3. /miami/


## Calendario recomendado para ABC Locksmith


Supongamos que el equipo puede publicar 5 páginas por semana.


### Semana 1 — Entity Foundation


| Día | Página |
| --- | --- |
| 1 | / |
| 2 | /contact/ |
| 3 | /locksmith/emergency-locksmith/ |
| 4 | /locksmith/car-locksmith/ |
| 5 | /locksmith/commercial-locksmith/ |


### Semana 2 — Main City Foundation


| Día | Página |
| --- | --- |
| 1 | /miami/ |
| 2 | /locksmith/miami/emergency-locksmith/ |
| 3 | /locksmith/miami/car-locksmith/ |
| 4 | /locksmith/miami/commercial-locksmith/ |
| 5 | /locksmith/residential-locksmith/ |


### Semana 3 — Main City Completion


| Día | Página |
| --- | --- |
| 1 | /locksmith/lock-rekeying/ |
| 2 | /locksmith/miami/residential-locksmith/ |
| 3 | /locksmith/miami/lock-rekeying/ |
| 4 | /locksmith/miami/key-duplication/ |
| 5 | /hialeah/ |


### Semana 4 — Secondary City Layer


| Día | Página |
| --- | --- |
| 1 | /coral-gables/ |
| 2 | /locksmith/hialeah/emergency-locksmith/ |
| 3 | /locksmith/coral-gables/emergency-locksmith/ |
| 4 | /doral/ |
| 5 | /hollywood/ |


### Semana 5 — First GeoArticle Cluster


| Día | Página |
| --- | --- |
| 1 | /miami/emergency-locksmith-cost-guide/ |
| 2 | /miami/what-to-do-locked-out-of-house/ |
| 3 | /miami/how-fast-can-locksmith-arrive/ |
| 4 | Internal linking review |
| 5 | Schema + QA pass |


## Publishing dependencies


| Página | Debe existir antes |
| --- | --- |
| Location-Based Service Page | Homepage + Service Overview + GeoHub |
| Additional Category Page | Homepage + GeoHub + related services |
| GeoArticle | Matching Location-Based Service Page + GeoHub |
| Secondary City GeoArticle | Secondary city landing page + GeoHub |
| GeoHub | Homepage |
| Service Overview | Homepage |


## Output final del Paso 9


Fase 1: Entity Foundation
Fase 2: Local Conversion Layer
Fase 3: Semantic Expansion Layer
Fase 4: Optimization Loop

Calendario de publicación
Dependencias entre páginas
Orden de producción
Orden de publicación
Reglas para GeoArticles
Reglas de QA por lote
Sistema de refresh
Sistema de tracking