**GMB Crush — Sistema Completo**
Versión literal del chat · 12 pasos + preámbulo

Documento generado a partir de la conversación paso a paso sobre el sistema GMB Crush para construir una web local desde cero.


# Índice

**1. Preámbulo — Cómo construiría una web de 0 siguiendo GMB Crush**
**2. Paso 01 — Intake Form**
**3. Paso 02 — Fórmula Maestra de Arquitectura**
**4. Paso 03 — Matriz Base**
**5. Paso 04 — URL Rules**
**6. Paso 05 — Page Type Rules**
**7. Paso 06 — Internal Linking Rules**
**8. Paso 07 — Priority Score**
**9. Paso 08 — QA Checklist**
**10. Paso 09 — Producción en Fases**
**11. Paso 10 — Pseudocódigo del Sistema**
**12. Paso 11 — Master Prompt Reutilizable**
**13. Paso 12 — Sistema Final Operativo**


# Preámbulo — Cómo construiría una web de 0 siguiendo GMB Crush


Así la construiría desde cero siguiendo GMB Crush: no empezaría por el diseño, sino por una arquitectura de entidad local que conecte GBP → homepage → servicios → ciudades → artículos → enlaces internos.


## 1. Primero definiría la entidad raíz


Antes de crear páginas, fijaría estos datos:

Marca: [Brand Name]
NAP completo: nombre, dirección, teléfono
Categoría principal GBP: [Primary GBP Category]
Categorías adicionales GBP: [Additional GBP Categories]
Servicios principales: [Service List]
Ciudad principal: [Main City]
Ciudades objetivo: [Service Area Cities]

Esto importa porque la metodología GMB Crush evalúa si la categoría principal de GBP está realmente soportada por la web mediante contenido, páginas de servicio, estructura semántica, schema e intención local.


## 2. Construiría la web con esta jerarquía


/
├── /primary-category/service/
├── /primary-category/service-2/
├── /primary-category/main-city/service/
├── /primary-category/main-city/service-2/
├── /primary-category/city-2/service/
├── /primary-category/city-2/service-2/
├── /main-city/
├── /city-2/
├── /main-city/article-topic/
└── /city-2/article-topic/

La lógica base de GMB Crush divide la web en seis tipos de página: Homepage, Service Overview Pages, Location-Based Service Pages, Additional Category Pages, GeoHub Pages y GeoArticle Pages. Cada una cumple una función distinta dentro del silo local.


## 3. Homepage: la página raíz de la entidad


La homepage no la usaría como una página genérica bonita. La usaría como el Root Entity Anchor.

Su trabajo sería decirle a Google y a los LLMs:

Esta marca ofrece este servicio principal, en esta ciudad principal, con estas categorías, servicios y áreas.

Estructura:

URL: /
H1: [Brand Name] – Trusted [Primary Service] in [Main City]
Meta Title: Top-Rated [Primary Service] in [Main City] | [Brand Name]

Incluiría:

- Intro con marca + servicio principal + ciudad principal.
- Bloque de 3–6 servicios principales con enlaces.
- Pruebas de confianza: reseñas, badges, años de experiencia, certificaciones.
- NAP completo visible y rastreable.
- CTA claro: llamar, reservar, pedir presupuesto.
- Enlaces a páginas de servicio.
- Enlaces al GeoHub de la ciudad principal.
- Enlaces a páginas de categorías adicionales.
- Schema: Organization, WebSite y LocalBusiness si hay presencia física en esa ciudad.


## 4. Páginas de servicio sin ciudad


Después crearía las páginas de servicio principales. Estas no están pensadas para rankear “servicio + ciudad”, sino para construir autoridad temática.

Ejemplo:

/locksmith/emergency-locksmith/
/locksmith/car-locksmith/
/locksmith/residential-locksmith/

Formato:

H1: Professional [Service] Services by [Brand Name]
Meta Title: [Service] by [Brand Name] | [Primary Category] Experts

Cada página tendría mínimo 1.000 palabras y cubriría:

- Qué es el servicio.
- A quién ayuda.
- Problemas que resuelve.
- Proceso paso a paso.
- Beneficios.
- FAQs.
- CTA.
- Enlaces hacia sus versiones locales.


## 5. Páginas “servicio + ciudad”: las páginas que más empujan el Local Pack


Estas serían las páginas más importantes para posicionar consultas como:

emergency locksmith in Miami
car locksmith in Orlando
residential locksmith in Tampa

URL:

/primary-category/city/service/

Ejemplo:

/locksmith/miami/emergency-locksmith/
/locksmith/orlando/emergency-locksmith/
/locksmith/tampa/emergency-locksmith/

Cada página tendría una sola intención:

Un servicio + una ciudad.

No mezclaría varias ciudades ni varios servicios en la misma landing.


## 6. Páginas para categorías adicionales GBP


Si el GBP tiene categorías adicionales, no las dejaría sin soporte.

Ejemplo:

Categoría principal: Plumber
Categorías adicionales: Drainage Service, Water Heater Repair Service

Crearía páginas específicas como:

/plumber/miami/drain-cleaning/
/plumber/miami/water-heater-repair/

Cada categoría adicional necesita su propia página local porque GMB Crush lo trata como soporte de profundidad de entidad.


## 7. GeoHub Pages: una página contenedora por ciudad


Luego construiría un GeoHub por cada ciudad importante.

Ejemplo:

/miami/
/orlando/
/tampa/

O, si quiero una estructura más categorizada:

/locksmith/miami/
/locksmith/orlando/
/locksmith/tampa/

El GeoHub no es una landing de un servicio. Es un contenedor de ciudad.


## 8. GeoArticles: artículos semánticos para empujar servicios y ciudades


Después construiría artículos por servicio + ciudad.

No son landing pages. Son boosters.

Ejemplo para /locksmith/miami/emergency-locksmith/:

/miami/what-to-do-locked-out-of-house/
/miami/how-fast-can-emergency-locksmith-arrive/
/miami/emergency-locksmith-cost-guide/

Cada GeoArticle debe reforzar una combinación:

1 servicio + 1 ciudad + 1 intención long-tail


## 9. La estructura de enlazado interno


| Página | Debe enlazar a |
| --- | --- |
| Homepage | Servicios principales, GeoHub principal, categorías adicionales |
| Service Overview Page | Versiones ciudad + servicio |
| Location-Based Service Page | Servicio padre, GeoHub, artículos relacionados |
| Additional Category Page | GeoHub y servicios relacionados |
| GeoHub | Todos los servicios, categorías y artículos de esa ciudad |
| GeoArticle | Página de servicio local, GeoHub y otro artículo relacionado |


## 10. Ejemplo práctico de arquitectura


Supongamos:

Business: ABC Locksmith
Primary GBP Category: Locksmith
Main City: Miami
Services:
- Emergency Locksmith
- Car Locksmith
- Residential Locksmith
- Commercial Locksmith

Cities:
- Miami
- Hialeah
- Coral Gables

Construiría:

/
/locksmith/emergency-locksmith/
/locksmith/car-locksmith/
/locksmith/residential-locksmith/
/locksmith/commercial-locksmith/

/miami/
/hialeah/
/coral-gables/

/locksmith/miami/emergency-locksmith/
/locksmith/miami/car-locksmith/
/locksmith/miami/residential-locksmith/
/locksmith/miami/commercial-locksmith/

/miami/what-to-do-locked-out-of-house/
/miami/emergency-locksmith-cost/
/miami/car-key-replacement-guide/


## 11. Orden de construcción


Fase 1: Core Entity Build.

Homepage
Contact page
About page
Service Overview Pages
Schema base
NAP visible
GBP link
Review blocks

Fase 2: Geo Conversion Build.

GeoHub principal
City + Service Pages para la ciudad principal
City + Service Pages para ciudades secundarias
Additional Category Pages

Fase 3: Semantic Expansion.

GeoArticles
FAQ clusters
Comparison articles
Problem-solution guides
Internal link expansion
Refresh cada 3–6 meses


## 12. Mi regla principal


No construiría una web local así:

/
 /services/
 /areas-we-serve/
 /contact/

Eso es demasiado débil para GMB Crush.

La construiría así:

Homepage = entidad raíz
Service pages = autoridad temática
City + service pages = conversión local
Additional category pages = soporte GBP
GeoHub pages = contenedores de ciudad
GeoArticles = profundidad semántica y AI Overview


## Fórmula de dominación local


1 homepage
+ 1 página por servicio principal
+ 1 GeoHub por ciudad
+ 1 página por servicio × ciudad
+ 1 página por categoría GBP adicional × ciudad
+ 3 GeoArticles por servicio × ciudad

Ejemplo con 5 servicios, 5 ciudades y 2 categorías adicionales:

1 homepage
5 service pages
5 GeoHubs
25 city-service pages
10 additional category pages
75 GeoArticles
= 116 páginas estratégicas

No todas se publican el primer día. Pero ese sería el mapa de dominación local.


# Paso 1 — Intake Form


## Objetivo del Paso 1


Este paso es obligatorio porque todo lo demás depende de estos datos. En GMB Crush, primero se valida la entidad del negocio, la categoría principal GBP, los servicios, las ciudades y la estructura semántica antes de crear páginas.


## Lo que tienes que rellenar


Business Name:

Website URL:

NAP completo:
- Nombre:
- Dirección:
- Teléfono:

Primary GBP Category:

Additional GBP Categories:

Main City:

Service Area Cities:

List of Services:

GBP URL:

País / Estado / Provincia:

¿Tiene ubicación física abierta al público?
Sí / No

¿En qué ciudad está físicamente ubicado?

¿Atiende otras ciudades sin oficina física allí?
Sí / No


## Ejemplo rellenado


Business Name:
ABC Locksmith

Website URL:
https://abclocksmith.com

NAP completo:
- Nombre: ABC Locksmith
- Dirección: 123 Main St, Miami, FL
- Teléfono: +1 305 000 0000

Primary GBP Category:
Locksmith

Additional GBP Categories:
- Emergency Locksmith Service
- Key Duplication Service

Main City:
Miami

Service Area Cities:
- Miami
- Hialeah
- Coral Gables
- Doral
- Hollywood

List of Services:
- Emergency Locksmith
- Car Locksmith
- Residential Locksmith
- Commercial Locksmith
- Lock Rekeying

GBP URL:
https://google.com/business/abc-locksmith

País / Estado / Provincia:
Florida, USA

¿Tiene ubicación física abierta al público?
Sí

¿En qué ciudad está físicamente ubicado?
Miami

¿Atiende otras ciudades sin oficina física allí?
Sí


## Output del Paso 1


Al terminar este paso tienes:

Entidad del negocio definida
Categoría principal GBP definida
Categorías adicionales definidas
Servicios principales definidos
Ciudad principal definida
Ciudades objetivo definidas
NAP validado
Ubicación física identificada
Áreas de servicio identificadas


## Decisión importante


No se crean URLs todavía. Primero se valida la entidad.

Este paso es la base para los 11 pasos siguientes:

Inputs → Arquitectura → URLs → Tipos de página → Contenido → Enlazado → Schema → Prioridad → Publicación → QA → Tracking → Optimización


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


# Paso 3 — Matriz base


## Objetivo del Paso 3


Ahora convertimos el cálculo del Paso 2 en una matriz operativa.

Es decir, pasamos de esto:

111 páginas estratégicas

a esto:

Cada página tiene una fila propia
Cada URL tiene un tipo de página
Cada página tiene ciudad, servicio, H1, meta title, schema y prioridad

La matriz será la base para todo lo que viene después:

URLs
Contenido
Enlazado interno
Schema
Calendario de publicación
QA
Tracking


## Lo que tienes que rellenar


Spreadsheet Name:

Website Root Domain:

Primary GBP Category:

Primary Category Slug:

Main City:

GeoHub URL Style:
Option A: /city/
Option B: /category/city/

Services:
1.
2.
3.
4.
5.

Service Slugs:
1.
2.
3.
4.
5.

Target Cities:
1.
2.
3.
4.
5.

City Slugs:
1.
2.
3.
4.
5.

Additional Categories that need separate pages:
1.
2.
3.

Additional Category Slugs:
1.
2.
3.

GeoArticles per Service x City:

Default Page Status:
Planned / Draft / Published

Default Priority:
P1 / P2 / P3 / P4


## Ejemplo rellenado


Spreadsheet Name:
ABC Locksmith – GMB Crush Website Architecture

Website Root Domain:
https://www.abclocksmith.com

Primary GBP Category:
Locksmith

Primary Category Slug:
locksmith

Main City:
Miami

GeoHub URL Style:
Option A: /city/

Services:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying

Service Slugs:
1. emergency-locksmith
2. car-locksmith
3. residential-locksmith
4. commercial-locksmith
5. lock-rekeying

Target Cities:
1. Miami
2. Hialeah
3. Coral Gables
4. Doral
5. Hollywood

City Slugs:
1. miami
2. hialeah
3. coral-gables
4. doral
5. hollywood

Additional Categories that need separate pages:
1. Key Duplication Service

Additional Category Slugs:
1. key-duplication

GeoArticles per Service x City:
3

Default Page Status:
Planned

Default Priority:
P3


## Estructura de la matriz


La matriz principal debería tener estas columnas:

ID
Page Type
Parent Type
Service
Service Slug
City
City Slug
Additional Category
URL
H1
Meta Title
Meta Description
Schema Type
Internal Links Required
Priority
Status
Notes


## Explicación de cada columna


| Columna | Para qué sirve |
| --- | --- |
| ID | Identificador único de la página |
| Page Type | Tipo de página según GMB Crush |
| Parent Type | Si depende de homepage, servicio, ciudad o artículo |
| Service | Servicio principal |
| Service Slug | Versión limpia para URL |
| City | Ciudad objetivo |
| City Slug | Versión limpia para URL |
| Additional Category | Categoría adicional GBP, si aplica |
| URL | URL final |
| H1 | H1 recomendado |
| Meta Title | Title SEO |
| Meta Description | Descripción SEO |
| Schema Type | Schema recomendado |
| Internal Links Required | A qué páginas debe enlazar |
| Priority | Prioridad de publicación |
| Status | Estado de producción |
| Notes | Notas estratégicas |


## Plantilla vacía


| ID | Page Type | Service | City | Additional Category | URL | H1 | Meta Title | Schema Type | Priority | Status |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  | Homepage |  |  |  |  |  |  |  |  |  |
|  | Service Overview |  |  |  |  |  |  |  |  |  |
|  | GeoHub |  |  |  |  |  |  |  |  |  |
|  | Location-Based Service |  |  |  |  |  |  |  |  |  |
|  | Additional Category |  |  |  |  |  |  |  |  |  |
|  | GeoArticle |  |  |  |  |  |  |  |  |  |


## Bloque 1 — Homepage


| ID | Page Type | Service | City | URL | H1 | Meta Title | Schema Type | Priority | Status |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| HP-001 | Homepage | Locksmith Services | Miami | / | ABC Locksmith – Trusted Locksmith Services in Miami | Top-Rated Locksmith in Miami \ | ABC Locksmith | Organization, WebSite, LocalBusiness | P1 | Planned |


## Bloque 2 — Service Overview Pages


Estas páginas no llevan ciudad.


| ID | Page Type | Service | City | URL | H1 | Meta Title | Schema Type | Priority | Status |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SO-001 | Service Overview | Emergency Locksmith | — | /locksmith/emergency-locksmith/ | Professional Emergency Locksmith Services by ABC Locksmith | Emergency Locksmith by ABC Locksmith \ | Locksmith Experts | Service, WebPage, BreadcrumbList, Speakable | P1 | Planned |
| SO-002 | Service Overview | Car Locksmith | — | /locksmith/car-locksmith/ | Professional Car Locksmith Services by ABC Locksmith | Car Locksmith by ABC Locksmith \ | Locksmith Experts | Service, WebPage, BreadcrumbList, Speakable | P1 | Planned |
| SO-003 | Service Overview | Residential Locksmith | — | /locksmith/residential-locksmith/ | Professional Residential Locksmith Services by ABC Locksmith | Residential Locksmith by ABC Locksmith \ | Locksmith Experts | Service, WebPage, BreadcrumbList, Speakable | P2 | Planned |
| SO-004 | Service Overview | Commercial Locksmith | — | /locksmith/commercial-locksmith/ | Professional Commercial Locksmith Services by ABC Locksmith | Commercial Locksmith by ABC Locksmith \ | Locksmith Experts | Service, WebPage, BreadcrumbList, Speakable | P2 | Planned |
| SO-005 | Service Overview | Lock Rekeying | — | /locksmith/lock-rekeying/ | Professional Lock Rekeying Services by ABC Locksmith | Lock Rekeying by ABC Locksmith \ | Locksmith Experts | Service, WebPage, BreadcrumbList, Speakable | P2 | Planned |


## Bloque 3 — GeoHub Pages


Una página por ciudad.


| ID | Page Type | Service | City | URL | H1 | Meta Title | Schema Type | Priority | Status |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GH-001 | GeoHub | All Services | Miami | /miami/ | ABC Locksmith – Locksmith Services in Miami | Locksmith Services in Miami \ | ABC Locksmith | CollectionPage, BreadcrumbList | P1 | Planned |
| GH-002 | GeoHub | All Services | Hialeah | /hialeah/ | ABC Locksmith – Locksmith Services in Hialeah | Locksmith Services in Hialeah \ | ABC Locksmith | CollectionPage, BreadcrumbList | P2 | Planned |
| GH-003 | GeoHub | All Services | Coral Gables | /coral-gables/ | ABC Locksmith – Locksmith Services in Coral Gables | Locksmith Services in Coral Gables \ | ABC Locksmith | CollectionPage, BreadcrumbList | P2 | Planned |
| GH-004 | GeoHub | All Services | Doral | /doral/ | ABC Locksmith – Locksmith Services in Doral | Locksmith Services in Doral \ | ABC Locksmith | CollectionPage, BreadcrumbList | P3 | Planned |
| GH-005 | GeoHub | All Services | Hollywood | /hollywood/ | ABC Locksmith – Locksmith Services in Hollywood | Locksmith Services in Hollywood \ | ABC Locksmith | CollectionPage, BreadcrumbList | P3 | Planned |


## Bloque 4 — Location-Based Service Pages


Aquí se crea una página por cada combinación: Servicio × Ciudad.

Ejemplo con Miami:


| ID | Page Type | Service | City | URL | H1 | Meta Title | Schema Type | Priority | Status |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| LBS-001 | Location-Based Service | Emergency Locksmith | Miami | /locksmith/miami/emergency-locksmith/ | ABC Locksmith – Emergency Locksmith in Miami | Top Emergency Locksmith in Miami \ | ABC Locksmith | LocalBusiness, BreadcrumbList | P1 | Planned |
| LBS-002 | Location-Based Service | Car Locksmith | Miami | /locksmith/miami/car-locksmith/ | ABC Locksmith – Car Locksmith in Miami | Top Car Locksmith in Miami \ | ABC Locksmith | LocalBusiness, BreadcrumbList | P1 | Planned |
| LBS-003 | Location-Based Service | Residential Locksmith | Miami | /locksmith/miami/residential-locksmith/ | ABC Locksmith – Residential Locksmith in Miami | Residential Locksmith in Miami \ | ABC Locksmith | LocalBusiness, BreadcrumbList | P2 | Planned |
| LBS-004 | Location-Based Service | Commercial Locksmith | Miami | /locksmith/miami/commercial-locksmith/ | ABC Locksmith – Commercial Locksmith in Miami | Commercial Locksmith in Miami \ | ABC Locksmith | LocalBusiness, BreadcrumbList | P2 | Planned |
| LBS-005 | Location-Based Service | Lock Rekeying | Miami | /locksmith/miami/lock-rekeying/ | ABC Locksmith – Lock Rekeying in Miami | Lock Rekeying in Miami \ | ABC Locksmith | LocalBusiness, BreadcrumbList | P2 | Planned |


## Bloque 5 — Additional Category Pages


En el ejemplo, la única categoría adicional que necesita página separada es Key Duplication Service.


| ID | Page Type | Service | City | Additional Category | URL | H1 | Meta Title | Schema Type | Priority | Status |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| AC-001 | Additional Category | Key Duplication | Miami | Key Duplication Service | /locksmith/miami/key-duplication/ | Key Duplication in Miami by ABC Locksmith | Key Duplication in Miami \ | ABC Locksmith | Service, BreadcrumbList | P2 | Planned |
| AC-002 | Additional Category | Key Duplication | Hialeah | Key Duplication Service | /locksmith/hialeah/key-duplication/ | Key Duplication in Hialeah by ABC Locksmith | Key Duplication in Hialeah \ | ABC Locksmith | Service, BreadcrumbList | P3 | Planned |
| AC-003 | Additional Category | Key Duplication | Coral Gables | Key Duplication Service | /locksmith/coral-gables/key-duplication/ | Key Duplication in Coral Gables by ABC Locksmith | Key Duplication in Coral Gables \ | ABC Locksmith | Service, BreadcrumbList | P3 | Planned |


## Bloque 6 — GeoArticle Pages


Aquí no hace falta crear las 75 filas manualmente en este momento. En la matriz base añadimos el patrón y algunos ejemplos.


| ID | Page Type | Service | City | URL | H1 | Meta Title | Schema Type | Priority | Status |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GA-001 | GeoArticle | Emergency Locksmith | Miami | /miami/what-to-do-locked-out-of-house/ | What to Do If You’re Locked Out of Your House in Miami | Locked Out of House in Miami? What to Do | Article, FAQPage, Breadcrumb, Speakable | P3 | Planned |  |
| GA-002 | GeoArticle | Emergency Locksmith | Miami | /miami/emergency-locksmith-cost-guide/ | How Much Does an Emergency Locksmith Cost in Miami? | Emergency Locksmith Cost in Miami \ | Guide | Article, FAQPage, Breadcrumb, Speakable | P3 | Planned |
| GA-003 | GeoArticle | Emergency Locksmith | Miami | /miami/how-fast-can-locksmith-arrive/ | How Fast Can a Locksmith Arrive in Miami? | Locksmith Response Times in Miami \ | ABC Locksmith | Article, FAQPage, Breadcrumb, Speakable | P3 | Planned |


## La matriz base completa tendría 111 filas


| Page Type | Cantidad |
| --- | --- |
| Homepage | 1 |
| Service Overview Pages | 5 |
| GeoHub Pages | 5 |
| Location-Based Service Pages | 25 |
| Additional Category Pages | 5 |
| GeoArticle Pages | 75 |
| Total | 111 |


## Cómo automatizar la creación de filas


En una hoja de cálculo, haría estas pestañas:

1. Inputs
2. Services
3. Cities
4. Additional Categories
5. URL Matrix
6. Internal Links
7. Schema Map
8. Publishing Plan
9. QA Checklist


## Decisión importante del Paso 3


Para este ejemplo vamos a usar este estilo de URL:

GeoHub:
/city/

Location-Based Service:
/category/city/service/

GeoArticle:
/city/article-topic/

Ejemplo:

/miami/
/locksmith/miami/emergency-locksmith/
/miami/emergency-locksmith-cost-guide/


## Paso 3 completado


Output de este paso:

URL Matrix creada
Tipos de página definidos
Columnas de producción definidas
Primeras URLs generadas
Schema asignado por tipo de página
Estado inicial asignado
Prioridad inicial asignada


# Paso 4 — URL Rules


## Objetivo del Paso 4


Ahora vamos a fijar las reglas de URLs para que la web no crezca de forma caótica.

Este paso evita problemas como:

URLs duplicadas
Canibalización
Slugs inconsistentes
Ciudades mezcladas
Servicios mezclados
Páginas de categoría duplicadas
GeoArticles que parecen landing pages
URLs demasiado largas
Estructuras imposibles de escalar

En GMB Crush, cada tipo de página tiene un patrón distinto: la homepage usa `/`, las Service Overview Pages usan `/category/service/`, las Location-Based Service Pages usan `/category/city/service/`, los GeoHubs usan `/city/` o `/category/city/`, y los GeoArticles usan `/city/service-topic/` o `/category/city/service-topic/`.


## Lo que tienes que rellenar


Website Root Domain:

Canonical Domain:
Option A: https://www.domain.com
Option B: https://domain.com

Trailing Slash:
Yes / No

Primary GBP Category:

Primary Category Slug:

Main City:

GeoHub URL Style:
Option A: /city/
Option B: /category/city/

Service Overview URL Style:
/[primary-category-slug]/[service-slug]/

Location-Based Service URL Style:
/[primary-category-slug]/[city-slug]/[service-slug]/

Additional Category URL Style:
/[primary-category-slug]/[city-slug]/[additional-category-slug]/

GeoArticle URL Style:
Option A: /[city-slug]/[article-topic-slug]/
Option B: /[primary-category-slug]/[city-slug]/[article-topic-slug]/

Use State in URL?
Yes / No

Use “near me” in URL?
Yes / No

Use stop words in URL?
Yes / No

Use service modifiers in URL?
Yes / No

Example modifiers:
- emergency
- 24-hour
- mobile
- affordable
- same-day

Words to avoid in URLs:

Approved city slugs:

Approved service slugs:

Approved additional category slugs:


## Ejemplo rellenado


Website Root Domain:
https://www.abclocksmith.com

Canonical Domain:
https://www.abclocksmith.com

Trailing Slash:
Yes

Primary GBP Category:
Locksmith

Primary Category Slug:
locksmith

Main City:
Miami

GeoHub URL Style:
Option A: /city/

Service Overview URL Style:
/[primary-category-slug]/[service-slug]/

Location-Based Service URL Style:
/[primary-category-slug]/[city-slug]/[service-slug]/

Additional Category URL Style:
/[primary-category-slug]/[city-slug]/[additional-category-slug]/

GeoArticle URL Style:
Option A: /[city-slug]/[article-topic-slug]/

Use State in URL?
No

Use “near me” in URL?
No

Use stop words in URL?
No, unless needed for readability

Use service modifiers in URL?
Yes, only if they represent a real service or search intent

Words to avoid in URLs:
- best
- cheap
- near-me
- top-rated
- number-one
- fast-service
- professional-service

Approved city slugs:
- miami
- hialeah
- coral-gables
- doral
- hollywood

Approved service slugs:
- emergency-locksmith
- car-locksmith
- residential-locksmith
- commercial-locksmith
- lock-rekeying

Approved additional category slugs:
- key-duplication


## Regla 1 — Dominio canónico


Elige una sola versión del dominio:

https://www.domain.com

o:

https://domain.com

No uses ambas.

Ejemplo correcto:

https://www.abclocksmith.com

Entonces todas las URLs deben generarse así:

https://www.abclocksmith.com/locksmith/miami/emergency-locksmith/

No así:

https://abclocksmith.com/locksmith/miami/emergency-locksmith/
https://www.abclocksmith.com/locksmith/miami/emergency-locksmith
http://www.abclocksmith.com/locksmith/miami/emergency-locksmith/

Regla final:

Una web = un dominio canónico = una estructura de URL.


## Regla 2 — Usar trailing slash


Mi recomendación para este sistema:

Trailing slash: Yes

Ejemplo correcto:

/locksmith/miami/emergency-locksmith/

Evitar mezcla:

/locksmith/miami/emergency-locksmith
/locksmith/miami/emergency-locksmith/

Regla final:

Todas las URLs terminan en /


## Regla 3 — Homepage


Patrón:

/

Ejemplo:

https://www.abclocksmith.com/

La homepage no debe tener una URL tipo:

/home/
/inicio/
/locksmith-miami/
/miami-locksmith/


## Regla 4 — Service Overview Pages


Patrón obligatorio:

/[primary-category-slug]/[service-slug]/

Ejemplo:

/locksmith/emergency-locksmith/

Ejemplos para ABC Locksmith:

/locksmith/emergency-locksmith/
/locksmith/car-locksmith/
/locksmith/residential-locksmith/
/locksmith/commercial-locksmith/
/locksmith/lock-rekeying/

Estas páginas no llevan ciudad. Su función es ser el pilar temático del servicio, no rankear directamente para “servicio + ciudad”.

Malos ejemplos:

/emergency-locksmith-miami/
/miami-emergency-locksmith/
/services/emergency-locksmith/
/locksmith-service/emergency-locksmith/
/locksmith/miami/emergency-locksmith-overview/

Regla final:

Service Overview = categoría + servicio, sin ciudad.


## Regla 5 — Location-Based Service Pages


Patrón obligatorio:

/[primary-category-slug]/[city-slug]/[service-slug]/

Ejemplo:

/locksmith/miami/emergency-locksmith/

Ejemplos para ABC Locksmith:

/locksmith/miami/emergency-locksmith/
/locksmith/miami/car-locksmith/
/locksmith/miami/residential-locksmith/

/locksmith/hialeah/emergency-locksmith/
/locksmith/hialeah/car-locksmith/
/locksmith/hialeah/residential-locksmith/

Malos ejemplos:

/miami/emergency-locksmith/
/emergency-locksmith/miami/
/locksmith/emergency-locksmith-miami/
/locksmith/miami/
/locksmith/miami-services/
/locksmith/miami/emergency-car-residential-locksmith/

Regla final:

Location-Based Service Page = una ciudad + un servicio.

No mezclar:

Miami + Hialeah
Emergency Locksmith + Car Locksmith
Residential + Commercial


## Regla 6 — Additional Category Pages


Patrón obligatorio:

/[primary-category-slug]/[city-slug]/[additional-category-slug]/

Ejemplo:

/locksmith/miami/key-duplication/

Ejemplos para ABC Locksmith:

/locksmith/miami/key-duplication/
/locksmith/hialeah/key-duplication/
/locksmith/coral-gables/key-duplication/
/locksmith/doral/key-duplication/
/locksmith/hollywood/key-duplication/

Regla final:

Categoría adicional GBP = página local específica si no está ya cubierta por un servicio principal.


## Regla 7 — GeoHub Pages


Tenemos dos opciones válidas:

/[city-slug]/

Ejemplo:

/miami/

O:

/[primary-category-slug]/[city-slug]/

Ejemplo:

/locksmith/miami/

Mi recomendación para una web local sencilla o media:

/[city-slug]/

Regla final:

GeoHub = contenedor de ciudad, no página de un servicio.


## Regla 8 — GeoArticle Pages


Patrón recomendado:

/[city-slug]/[article-topic-slug]/

Ejemplo:

/miami/emergency-locksmith-cost-guide/

Ejemplos para ABC Locksmith:

/miami/what-to-do-locked-out-of-house/
/miami/emergency-locksmith-cost-guide/
/miami/how-fast-can-locksmith-arrive/

También válido:

/[primary-category-slug]/[city-slug]/[article-topic-slug]/

Ejemplo:

/locksmith/miami/emergency-locksmith-cost-guide/

Pero para ABC Locksmith usamos:

/[city-slug]/[article-topic-slug]/

Regla final:

GeoArticle = ciudad + intención long-tail.
No debe competir con la landing servicio + ciudad.


## Regla 9 — No usar “near me” en URLs


Mal ejemplo:

/locksmith/miami/emergency-locksmith-near-me/
/miami/locksmith-near-me/
/near-me/emergency-locksmith/

Mejor opción:

/locksmith/miami/emergency-locksmith/
/miami/how-to-choose-an-emergency-locksmith/

Puedes usar “near me” en H2, FAQs, texto, anchor text o GeoArticle title si tiene sentido. Pero no lo usaría como slug principal.


## Regla 10 — No usar “best”, “cheap” o “top-rated” en URLs


Malos ejemplos:

/best-locksmith-miami/
/cheap-car-locksmith-miami/
/top-rated-emergency-locksmith-miami/

Mejores ejemplos:

/locksmith/miami/emergency-locksmith/
/locksmith/miami/car-locksmith/
/miami/emergency-locksmith-cost-guide/

Regla final:

La URL debe ser estable, limpia y objetiva.


## Regla 11 — Slugs limpios


Usar:

minúsculas
guiones medios
sin acentos
sin símbolos
sin comas
sin apostrofes
sin emojis
sin mayúsculas
sin fechas salvo que sea necesario

Ejemplos:


| Texto original | Slug correcto |
| --- | --- |
| Emergency Locksmith | emergency-locksmith |
| Car Locksmith | car-locksmith |
| Coral Gables | coral-gables |
| Key Duplication Service | key-duplication |
| Lock Rekeying | lock-rekeying |
| 24 Hour Locksmith | 24-hour-locksmith |


## Regla 12 — Cuándo usar modificadores


Permitidos si son parte del servicio:

emergency-locksmith
24-hour-locksmith
mobile-locksmith
car-key-replacement
lock-rekeying

Evitar si son solo adjetivos SEO:

best-locksmith
cheap-locksmith
top-locksmith
number-one-locksmith
trusted-locksmith
fast-locksmith


## Regla 13 — No duplicar categorías adicionales ya cubiertas


No hacemos dos URLs:

/locksmith/miami/emergency-locksmith/
/locksmith/miami/emergency-locksmith-service/

Hacemos una sola:

/locksmith/miami/emergency-locksmith/


## Regla 14 — No fingir ubicación física


Si el negocio está físicamente en Miami pero atiende Hialeah, Coral Gables, Doral y Hollywood, las URLs pueden existir:

/locksmith/hialeah/emergency-locksmith/
/locksmith/coral-gables/emergency-locksmith/
/locksmith/doral/emergency-locksmith/

Pero el contenido no debe decir:

“Our Hialeah office”
“Our Coral Gables location”
“Visit our Doral storefront”

A menos que realmente haya oficina allí.


## Estructura final aprobada para ABC Locksmith


Homepage:
/

Service Overview:
/locksmith/emergency-locksmith/
/locksmith/car-locksmith/
/locksmith/residential-locksmith/
/locksmith/commercial-locksmith/
/locksmith/lock-rekeying/

GeoHub:
/miami/
/hialeah/
/coral-gables/
/doral/
/hollywood/

Location-Based Service:
/locksmith/miami/emergency-locksmith/
/locksmith/miami/car-locksmith/
/locksmith/miami/residential-locksmith/
/locksmith/miami/commercial-locksmith/
/locksmith/miami/lock-rekeying/

Additional Category:
/locksmith/miami/key-duplication/
/locksmith/hialeah/key-duplication/
/locksmith/coral-gables/key-duplication/
/locksmith/doral/key-duplication/
/locksmith/hollywood/key-duplication/

GeoArticle:
/miami/what-to-do-locked-out-of-house/
/miami/emergency-locksmith-cost-guide/
/miami/how-fast-can-locksmith-arrive/


## URL Rules Checklist


| Check | Pregunta | Estado |
| --- | --- | --- |
| Dominio canónico | ¿Usa siempre www o non-www? | ✅ |
| HTTPS | ¿La URL usa HTTPS? | ✅ |
| Trailing slash | ¿Todas las URLs siguen la misma regla? | ✅ |
| Slug limpio | ¿Está en minúsculas y con guiones? | ✅ |
| Page type claro | ¿Sabemos si es Service, GeoHub, Local Page o Article? | ✅ |
| Servicio único | ¿La página tiene un solo servicio principal? | ✅ |
| Ciudad única | ¿La página tiene una sola ciudad principal? | ✅ |
| No duplicación | ¿No existe otra URL con la misma intención? | ✅ |
| No “near me” | ¿Evita near-me en el slug principal? | ✅ |
| No adjetivos vacíos | ¿Evita best, cheap, top-rated en slug? | ✅ |
| GBP alignment | ¿Soporta la categoría principal o adicional? | ✅ |
| Escalable | ¿La URL puede multiplicarse por ciudad/servicio sin romperse? | ✅ |


## Output final del Paso 4


Reglas de dominio
Reglas de trailing slash
Patrones por tipo de página
Slugs aprobados
URLs prohibidas
URLs duplicadas evitadas
GeoHub URL style aprobado
GeoArticle URL style aprobado
Reglas anti-canibalización


# Paso 5 — Page Type Rules


## Objetivo del Paso 5


En el Paso 4 definimos cómo deben ser las URLs.

Ahora definimos qué debe contener cada tipo de página.

Este paso convierte la arquitectura en plantillas de producción. Es decir, cada página tendrá reglas claras de:

H1
Meta Title
Meta Description
Intro
H2/H3
FAQs
CTA
Schema
Internal links
Contenido mínimo
Objetivo SEO
Objetivo GBP
Objetivo AI Overview

En GMB Crush, cada tipo de página cumple una función distinta: la homepage actúa como raíz de entidad, las Service Overview Pages crean autoridad temática, las Location-Based Service Pages convierten búsquedas locales, las Additional Category Pages soportan categorías GBP adicionales, los GeoHubs agrupan señales de ciudad y los GeoArticles funcionan como boosters semánticos.


## Lo que tienes que rellenar


Business Name:

Website Root Domain:

Primary GBP Category:

Primary Category Slug:

Main City:

Main State / Province:

Primary Service:

Core Services:
1.
2.
3.
4.
5.

Target Cities:
1.
2.
3.
4.
5.

Additional GBP Categories that need pages:
1.
2.
3.

Phone:

Email:

GBP URL:

NAP:
- Name:
- Address:
- Phone:

Physical Location City:

Service Area Cities:

Trust Signals:
- Years in business:
- Reviews:
- Certifications:
- Awards:
- Guarantees:
- Emergency / same-day / mobile service:

Preferred CTA:
Option A: Call now
Option B: Book online
Option C: Request estimate
Option D: Contact us

Brand tone:
Option A: Professional
Option B: Friendly
Option C: Premium
Option D: Urgent / emergency
Option E: Local and conversational


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

Main State / Province:
Florida

Primary Service:
Locksmith Services

Core Services:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying

Target Cities:
1. Miami
2. Hialeah
3. Coral Gables
4. Doral
5. Hollywood

Additional GBP Categories that need pages:
1. Key Duplication Service

Phone:
+1 305 000 0000

Email:
info@abclocksmith.com

GBP URL:
https://google.com/business/abc-locksmith

NAP:
- Name: ABC Locksmith
- Address: 123 Main St, Miami, FL
- Phone: +1 305 000 0000

Physical Location City:
Miami

Service Area Cities:
Miami, Hialeah, Coral Gables, Doral, Hollywood

Trust Signals:
- Years in business: 10+
- Reviews: 250+ Google reviews
- Certifications: Licensed locksmith technicians
- Awards: Local service award
- Guarantees: Workmanship guarantee
- Emergency / same-day / mobile service: Yes

Preferred CTA:
Call now

Brand tone:
Friendly, professional, local and urgent when needed


## Los 6 tipos de página


1. Homepage
2. Service Overview Page
3. Location-Based Service Page
4. Additional Category Page
5. GeoHub Page
6. GeoArticle Page


# 1. Homepage Rules


## Función


La homepage es la Root Entity Anchor.

Su objetivo es decirle a Google, al usuario y a los sistemas de IA:

Quién es la marca
Cuál es la categoría principal
Cuál es la ciudad principal
Qué servicios ofrece
Dónde opera
Cómo contactar
Por qué confiar en ella


## Lo que tienes que rellenar


Homepage URL:

Brand Name:

Primary Service:

Primary GBP Category:

Main City:

Main State:

Main CTA:

Core Services to highlight:
1.
2.
3.
4.
5.
6.

Trust Signals:
1.
2.
3.
4.

NAP:
- Name:
- Address:
- Phone:

Main GeoHub URL:

Top Service URLs:
1.
2.
3.

Additional Category URLs:
1.
2.


## Ejemplo rellenado


Homepage URL:
/

Brand Name:
ABC Locksmith

Primary Service:
Locksmith Services

Primary GBP Category:
Locksmith

Main City:
Miami

Main State:
Florida

Main CTA:
Call now

Core Services to highlight:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying
6. Key Duplication

Trust Signals:
1. 10+ years in business
2. 250+ Google reviews
3. Licensed locksmith technicians
4. Same-day mobile service

NAP:
- Name: ABC Locksmith
- Address: 123 Main St, Miami, FL
- Phone: +1 305 000 0000

Main GeoHub URL:
/miami/

Top Service URLs:
1. /locksmith/emergency-locksmith/
2. /locksmith/car-locksmith/
3. /locksmith/residential-locksmith/

Additional Category URLs:
1. /locksmith/miami/key-duplication/


## Homepage output rules


URL:
/

H1:
[Brand Name] – Trusted [Primary Service] in [Main City, ST]

Meta Title:
Top-Rated [Primary Service] in [Main City, ST] | [Brand Name]

Meta Description:
Need trusted [Primary Service] in [Main City]? [Brand Name] provides reliable local service, expert support, and fast response. Call today.

Word Count:
900–1,300 words

Schema:
Organization
WebSite
LocalBusiness only if physical presence exists in main city
FAQPage
Speakable
BreadcrumbList optional


## Homepage section structure


H1: Brand + Primary Service + Main City

Intro:
100–150 words explaining who the business is, what it does, and where it operates.

Quick Answer:
2-sentence AI Overview-friendly summary.

Core Services:
3–6 service blocks with internal links.

Why Choose Us:
Trust signals, reviews, guarantees, credentials.

Service Area Overview:
Brief explanation of main city and nearby service areas.

FAQ Section:
5–7 FAQ-style H2/H3 questions.

Reviews / Social Proof:
Google review highlights or testimonials.

NAP Block:
Clickable phone, address, business name.

CTA:
Call, book, or request estimate.

Internal Links:
Service pages, GeoHub, Additional Category pages.


## Ejemplo para ABC Locksmith


H1:
ABC Locksmith – Trusted Locksmith Services in Miami, FL

Meta Title:
Top-Rated Locksmith in Miami, FL | ABC Locksmith

Meta Description:
Need a trusted locksmith in Miami? ABC Locksmith offers emergency, car, residential, commercial and rekeying services. Call today.

Quick Answer:
ABC Locksmith provides trusted locksmith services in Miami, including emergency lockouts, car locksmith support, residential lock repairs, commercial security solutions, and lock rekeying. Our mobile team helps local customers get secure access quickly, safely, and professionally.

Core Service Blocks:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying
6. Key Duplication

Schema:
Organization
WebSite
LocalBusiness
FAQPage
Speakable


# 2. Service Overview Page Rules


## Función


La Service Overview Page es una página de autoridad temática sin ciudad.

No intenta rankear directamente para:

emergency locksmith in Miami

Su objetivo es rankear y construir autoridad para:

emergency locksmith
emergency locksmith service
lockout assistance
urgent locksmith support

Y después empujar sus versiones locales:

/locksmith/miami/emergency-locksmith/
/locksmith/hialeah/emergency-locksmith/
/locksmith/coral-gables/emergency-locksmith/


## Lo que tienes que rellenar


Service Name:

Service Slug:

Primary Category:

Primary Category Slug:

Brand Name:

Service Overview URL:

Related Services:
1.
2.
3.

Top City Versions:
1.
2.
3.

Helpful Resource / GeoArticle:


## Ejemplo rellenado


Service Name:
Emergency Locksmith

Service Slug:
emergency-locksmith

Primary Category:
Locksmith

Primary Category Slug:
locksmith

Brand Name:
ABC Locksmith

Service Overview URL:
/locksmith/emergency-locksmith/

Related Services:
1. Car Locksmith
2. Residential Locksmith
3. Lock Rekeying

Top City Versions:
1. /locksmith/miami/emergency-locksmith/
2. /locksmith/hialeah/emergency-locksmith/
3. /locksmith/coral-gables/emergency-locksmith/

Helpful Resource / GeoArticle:
/miami/emergency-locksmith-cost-guide/


## Service Overview output rules


URL:
/[primary-category-slug]/[service-slug]/

H1:
Professional [Service] Services by [Brand Name]

Meta Title:
[Service] by [Brand Name] | [Primary Category] Experts

Meta Description:
Need trusted [Service]? [Brand Name] delivers expert solutions with speed, quality, and care. Explore our process, benefits, and support.

Word Count:
850–1,000 words

Location References:
No city references

Schema:
Service
WebPage
BreadcrumbList
Speakable


## Service Overview section structure


H1:
Professional [Service] Services by [Brand Name]

Intro:
Introduce the service as part of the brand’s mission. No local references.

H2 – Authority:
Credentials, experience, training, trust signals.

H2 – Uniqueness:
What makes the service different.

H2 – Depth:
Step-by-step process, deliverables, what is included.

H2 – Intent:
Who needs the service and what problems it solves.

H2 – Optimization:
Related services, comparisons, next steps.

FAQ Section:
3–5 realistic questions.

CTA:
Low-pressure call to action.

Internal Links:
Homepage
Related service pages
2–3 city-specific versions
1 helpful GeoArticle


## Ejemplo para ABC Locksmith


URL:
/locksmith/emergency-locksmith/

H1:
Professional Emergency Locksmith Services by ABC Locksmith

Meta Title:
Emergency Locksmith by ABC Locksmith | Locksmith Experts

Meta Description:
Need trusted emergency locksmith help? ABC Locksmith delivers fast, careful and professional lockout support when access can’t wait.

Main H2s:
1. Reliable Emergency Locksmith Support When Access Matters
2. What Makes Our Emergency Locksmith Process Different
3. What’s Included in Emergency Locksmith Service
4. When You Should Call an Emergency Locksmith
5. Related Locksmith Services That May Help

FAQs:
1. What’s included in emergency locksmith service?
2. Can an emergency locksmith help with broken keys?
3. Is emergency locksmith service suitable for homes and cars?
4. How do I know if I need rekeying after a lockout?
5. What should I do before calling a locksmith?

Internal Links:
- /
- /locksmith/car-locksmith/
- /locksmith/residential-locksmith/
- /locksmith/miami/emergency-locksmith/
- /locksmith/hialeah/emergency-locksmith/
- /miami/emergency-locksmith-cost-guide/

Schema:
Service
WebPage
BreadcrumbList
Speakable


# 3. Location-Based Service Page Rules


## Función


La Location-Based Service Page es una página comercial para una combinación exacta:

Servicio + Ciudad

Ejemplo:

Emergency Locksmith + Miami

Esta página sí está pensada para rankear búsquedas como:

emergency locksmith in Miami
Miami emergency locksmith
locksmith near me in Miami
locked out of house Miami


## Lo que tienes que rellenar


Service Name:

Service Slug:

City:

City Slug:

Primary Category:

Primary Category Slug:

Brand Name:

Location-Based Service URL:

Parent Service Overview URL:

GeoHub URL:

Related Services in Same City:
1.
2.
3.

Related GeoArticles:
1.
2.
3.

Local Notes:
- Neighborhoods:
- Local concerns:
- Common customer scenarios:
- Physical office in this city? Yes / No


## Ejemplo rellenado


Service Name:
Emergency Locksmith

Service Slug:
emergency-locksmith

City:
Miami

City Slug:
miami

Primary Category:
Locksmith

Primary Category Slug:
locksmith

Brand Name:
ABC Locksmith

Location-Based Service URL:
/locksmith/miami/emergency-locksmith/

Parent Service Overview URL:
/locksmith/emergency-locksmith/

GeoHub URL:
/miami/

Related Services in Same City:
1. /locksmith/miami/car-locksmith/
2. /locksmith/miami/residential-locksmith/
3. /locksmith/miami/lock-rekeying/

Related GeoArticles:
1. /miami/what-to-do-locked-out-of-house/
2. /miami/emergency-locksmith-cost-guide/
3. /miami/how-fast-can-locksmith-arrive/

Local Notes:
- Neighborhoods: Brickell, Wynwood, Little Havana, Coral Way
- Local concerns: apartment lockouts, car lockouts, late-night access issues
- Common customer scenarios: locked out, broken key, urgent rekey
- Physical office in this city? Yes


## Location-Based Service output rules


URL:
/[primary-category-slug]/[city-slug]/[service-slug]/

H1:
[Brand Name] – [Service] in [City]

Meta Title:
Top [Service] in [City] | [Brand Name]

Meta Description:
Need [Service] in [City]? [Brand Name] helps with [problem], [problem], and [problem]. Call for trusted local support.

Word Count:
800–1,000 words

Schema:
LocalBusiness
BreadcrumbList
FAQPage optional
Speakable optional


## Ejemplo para ABC Locksmith


URL:
/locksmith/miami/emergency-locksmith/

H1:
ABC Locksmith – Emergency Locksmith in Miami

Meta Title:
Top Emergency Locksmith in Miami | ABC Locksmith

Meta Description:
Locked out in Miami? ABC Locksmith helps with urgent lockouts, broken keys, rekeying and secure access support. Call today.

Intro angle:
Miami residents often need urgent locksmith help after apartment lockouts, car lockouts, broken keys, or access problems after a long day downtown, in Brickell, Wynwood or nearby neighborhoods.

Main H2s:
1. Trusted Emergency Locksmith Help for Miami Lockouts
2. What Makes Our Miami Emergency Locksmith Service Different
3. What’s Included When You Call for Urgent Locksmith Support
4. When Miami Residents Should Call an Emergency Locksmith
5. Other Locksmith Services Available in Miami

FAQs:
1. Can an emergency locksmith help if I’m locked out of my apartment in Miami?
2. How fast can a locksmith arrive in Miami?
3. Can you help with car lockouts in Miami?
4. Should I rekey my lock after losing keys?
5. Do you provide locksmith help outside regular business hours?

Internal Links:
- /locksmith/emergency-locksmith/
- /miami/
- /locksmith/miami/car-locksmith/
- /locksmith/miami/residential-locksmith/
- /miami/emergency-locksmith-cost-guide/

Schema:
LocalBusiness
BreadcrumbList
FAQPage
Speakable


# 4. Additional Category Page Rules


## Función


La Additional Category Page soporta una categoría adicional del GBP.

Ejemplo:

Primary GBP Category:
Locksmith

Additional GBP Category:
Key Duplication Service

Si esa categoría adicional no está cubierta por un servicio principal, se crea una página local propia.


## Lo que tienes que rellenar


Additional GBP Category:

Service Name for Page:

Service Slug:

City:

City Slug:

Primary Category:

Primary Category Slug:

Brand Name:

Additional Category URL:

GeoHub URL:

Related Location-Based Service Pages:
1.
2.
3.

Related GeoArticles:
1.
2.

Local Problem / Scenario:

Physical office in this city? Yes / No


## Ejemplo rellenado


Additional GBP Category:
Key Duplication Service

Service Name for Page:
Key Duplication

Service Slug:
key-duplication

City:
Miami

City Slug:
miami

Primary Category:
Locksmith

Primary Category Slug:
locksmith

Brand Name:
ABC Locksmith

Additional Category URL:
/locksmith/miami/key-duplication/

GeoHub URL:
/miami/

Related Location-Based Service Pages:
1. /locksmith/miami/residential-locksmith/
2. /locksmith/miami/commercial-locksmith/
3. /locksmith/miami/lock-rekeying/

Related GeoArticles:
1. /miami/key-duplication-vs-rekeying/
2. /miami/how-many-spare-keys-should-you-have/

Local Problem / Scenario:
Miami homeowners, renters and business owners often need spare keys for family members, staff, tenants or emergency access.

Physical office in this city?
Yes


## Additional Category output rules


URL:
/[primary-category-slug]/[city-slug]/[additional-category-slug]/

H1:
[Brand Name] – Expert [Service] in [City]

Meta Title:
[Service] in [City] | [Brand Name]

Meta Description:
Need [Service] in [City]? [Brand Name] provides reliable help for [problem], [use case], and [use case]. Call today.

Word Count:
800–1,000 words

Schema:
Service with areaServed
BreadcrumbList
FAQPage optional
Speakable optional


# 5. GeoHub Page Rules


## Función


La GeoHub Page es el contenedor de ciudad. No es una landing de un servicio concreto.

Debe agrupar:

Servicios en esa ciudad
Categorías adicionales en esa ciudad
GeoArticles de esa ciudad
Trust signals locales
Barrios o zonas cubiertas
Enlaces internos
CTA


## Lo que tienes que rellenar


City:

City Slug:

Brand Name:

Primary Category:

Industry / Service Group:

GeoHub URL:

Services available in this city:
1.
2.
3.
4.
5.

Additional Category Pages in this city:
1.
2.

GeoArticles for this city:
1.
2.
3.
4.
5.

Neighborhoods / Nearby Areas:
1.
2.
3.
4.

Local Trust Signals:
1.
2.
3.

Physical office in this city? Yes / No

Contact Page URL:


## Ejemplo rellenado


City:
Miami

City Slug:
miami

Brand Name:
ABC Locksmith

Primary Category:
Locksmith

Industry / Service Group:
Locksmith Services

GeoHub URL:
/miami/

Services available in this city:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying

Additional Category Pages in this city:
1. Key Duplication

GeoArticles for this city:
1. What to Do If You’re Locked Out of Your House in Miami
2. Emergency Locksmith Cost Guide in Miami
3. How Fast Can a Locksmith Arrive in Miami?
4. Key Duplication vs Rekeying in Miami
5. Car Key Replacement Guide for Miami Drivers

Neighborhoods / Nearby Areas:
1. Brickell
2. Wynwood
3. Little Havana
4. Coral Way

Local Trust Signals:
1. 250+ Google reviews
2. Same-day mobile locksmith support
3. Licensed locksmith technicians

Physical office in this city?
Yes

Contact Page URL:
/contact/


## GeoHub output rules


URL:
/[city-slug]/

H1:
[Brand Name] – [Industry] Services in [City]

Meta Title:
[Industry] Services in [City] | [Brand Name]

Meta Description:
Explore trusted [Industry] services in [City] from [Brand Name]. View local services, helpful resources and ways to contact our team.

Word Count:
700–1,100 words

Schema:
CollectionPage
BreadcrumbList
LocalBusiness optional if physical presence exists


# 6. GeoArticle Page Rules


## Función


La GeoArticle Page no es una landing comercial.

Es un semantic booster.

Su objetivo es reforzar una combinación específica:

Servicio + Ciudad + Intención long-tail

Ejemplo:

Emergency Locksmith + Miami + Cost Guide


## Lo que tienes que rellenar


Service:

City:

Article Topic:

Long-Tail Keyword:

Intent Type:
Informational / Pain Point / Navigational / Comparison / Awareness

Article URL:

Matching Location-Based Service Page:

Matching GeoHub Page:

Related GeoArticle:

Brand Name:

Can mention physical location in this city?
Yes / No

Local references:
1.
2.
3.

Main CTA:


## Ejemplo rellenado


Service:
Emergency Locksmith

City:
Miami

Article Topic:
Emergency Locksmith Cost Guide

Long-Tail Keyword:
how much does an emergency locksmith cost in Miami

Intent Type:
Informational / Commercial Research

Article URL:
/miami/emergency-locksmith-cost-guide/

Matching Location-Based Service Page:
/locksmith/miami/emergency-locksmith/

Matching GeoHub Page:
/miami/

Related GeoArticle:
/miami/what-to-do-locked-out-of-house/

Brand Name:
ABC Locksmith

Can mention physical location in this city?
Yes

Local references:
1. Brickell
2. Wynwood
3. Little Havana

Main CTA:
Call ABC Locksmith for emergency locksmith help in Miami


## GeoArticle output rules


URL:
/[city-slug]/[article-topic-slug]/

H1:
[Article Topic] in [City]

Meta Title:
[Article Topic] in [City] | [Brand Name]

Meta Description:
Learn about [Article Topic] in [City], including what to expect, common mistakes and when to call [Brand Name].

Word Count:
1,000–1,500 words

Schema:
Article
FAQPage
BreadcrumbList
Speakable


## Matriz resumen del Paso 5


| Page Type | URL Pattern | Word Count | Main Purpose | Schema |
| --- | --- | --- | --- | --- |
| Homepage | / | 900–1,300 | Root entity anchor | Organization, WebSite, LocalBusiness optional, FAQPage, Speakable |
| Service Overview | /category/service/ | 850–1,000 | Topical authority | Service, WebPage, BreadcrumbList, Speakable |
| Location-Based Service | /category/city/service/ | 800–1,000 | Local conversion | LocalBusiness, BreadcrumbList, FAQPage optional |
| Additional Category | /category/city/service/ | 800–1,000 | GBP category support | Service with areaServed, BreadcrumbList |
| GeoHub | /city/ | 700–1,100 | City silo container | CollectionPage, BreadcrumbList |
| GeoArticle | /city/article-topic/ | 1,000–1,500 | Semantic booster | Article, FAQPage, BreadcrumbList, Speakable |


## Reglas anti-error del Paso 5


No confundir Service Overview con Location-Based Service.

Incorrecto:

/locksmith/emergency-locksmith/

usada como página para Miami.

Correcto:

/locksmith/emergency-locksmith/

Página general del servicio.

/locksmith/miami/emergency-locksmith/

Página local del servicio en Miami.

No convertir GeoArticles en landings.

No inventar oficina física.

No crear páginas vacías o thin content.


## Output final del Paso 5


Homepage template
Service Overview template
Location-Based Service template
Additional Category template
GeoHub template
GeoArticle template
Schema rules por tipo de página
Word count por tipo de página
H1 rules
Meta title rules
Meta description rules
FAQ rules
CTA rules
Internal link requirements base


# Paso 6 — Internal Linking Rules


## Objetivo del Paso 6


Ahora vamos a definir cómo se conectan todas las páginas entre sí.

Este paso es crítico porque una web GMB Crush no funciona solo por tener muchas URLs. Funciona porque cada URL empuja a otra dentro de un silo lógico:

Homepage → Service Overview Pages
Homepage → Main GeoHub
Service Overview → City + Service Pages
GeoHub → Todas las páginas de una ciudad
Location-Based Service → Servicio padre + GeoHub + artículos
GeoArticle → Página comercial + GeoHub
Additional Category → GeoHub + servicios relacionados


## Lo que tienes que rellenar


Business Name:

Website Root Domain:

Homepage URL:

Primary GBP Category:

Primary Category Slug:

Main City:

Main GeoHub URL:

Service Overview Pages:
1.
2.
3.
4.
5.

GeoHub Pages:
1.
2.
3.
4.
5.

Location-Based Service Pages:
1.
2.
3.
4.
5.

Additional Category Pages:
1.
2.
3.

GeoArticle Pages:
1.
2.
3.
4.
5.

Contact Page URL:

GBP URL:

Top Priority Services:
1.
2.
3.

Top Priority Cities:
1.
2.
3.

Preferred CTA Anchor:
Example: Call ABC Locksmith today

Preferred Informational Anchor:
Example: Learn more about emergency locksmith services

Preferred Local Anchor:
Example: locksmith services in Miami


## Ejemplo rellenado


Business Name:
ABC Locksmith

Website Root Domain:
https://www.abclocksmith.com

Homepage URL:
/

Primary GBP Category:
Locksmith

Primary Category Slug:
locksmith

Main City:
Miami

Main GeoHub URL:
/miami/

Service Overview Pages:
1. /locksmith/emergency-locksmith/
2. /locksmith/car-locksmith/
3. /locksmith/residential-locksmith/
4. /locksmith/commercial-locksmith/
5. /locksmith/lock-rekeying/

GeoHub Pages:
1. /miami/
2. /hialeah/
3. /coral-gables/
4. /doral/
5. /hollywood/

Location-Based Service Pages:
1. /locksmith/miami/emergency-locksmith/
2. /locksmith/miami/car-locksmith/
3. /locksmith/miami/residential-locksmith/
4. /locksmith/hialeah/emergency-locksmith/
5. /locksmith/coral-gables/emergency-locksmith/

Additional Category Pages:
1. /locksmith/miami/key-duplication/
2. /locksmith/hialeah/key-duplication/
3. /locksmith/coral-gables/key-duplication/

GeoArticle Pages:
1. /miami/what-to-do-locked-out-of-house/
2. /miami/emergency-locksmith-cost-guide/
3. /miami/how-fast-can-locksmith-arrive/
4. /hialeah/what-to-do-locked-out-of-house/
5. /coral-gables/emergency-locksmith-cost-guide/

Contact Page URL:
/contact/

GBP URL:
https://google.com/business/abc-locksmith

Top Priority Services:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith

Top Priority Cities:
1. Miami
2. Hialeah
3. Coral Gables

Preferred CTA Anchor:
Call ABC Locksmith today

Preferred Informational Anchor:
Learn more about emergency locksmith services

Preferred Local Anchor:
locksmith services in Miami


## La regla madre del enlazado interno


Cada página debe enlazar hacia arriba, hacia abajo y lateralmente.

Es decir:

Hacia arriba = página padre
Hacia abajo = páginas hijas
Lateralmente = páginas relacionadas del mismo silo

Ejemplo:

/locksmith/miami/emergency-locksmith/

Debe enlazar:

Hacia arriba:
- /locksmith/emergency-locksmith/
- /miami/

Lateralmente:
- /locksmith/miami/car-locksmith/
- /locksmith/miami/residential-locksmith/
- /locksmith/miami/lock-rekeying/

Hacia abajo / soporte:
- /miami/what-to-do-locked-out-of-house/
- /miami/emergency-locksmith-cost-guide/


## Mapa general de enlazado


| Source Page | Debe enlazar a | Objetivo |
| --- | --- | --- |
| Homepage | Service Overview Pages | Reforzar servicios principales |
| Homepage | Main GeoHub | Reforzar ciudad principal |
| Homepage | Additional Category Pages principales | Soportar categorías GBP adicionales |
| Service Overview | Todas las versiones ciudad + servicio | Empujar páginas locales |
| Service Overview | Homepage | Reforzar entidad raíz |
| Service Overview | Servicios relacionados | Construir autoridad temática |
| Location-Based Service | Servicio padre | Conectar página local con pilar temático |
| Location-Based Service | GeoHub de ciudad | Conectar con silo local |
| Location-Based Service | Otros servicios de la misma ciudad | Crear cluster local |
| Location-Based Service | GeoArticles relacionados | Reforzar long-tail |
| Additional Category | GeoHub | Integrar categoría adicional en ciudad |
| Additional Category | Servicios relacionados | Evitar página aislada |
| GeoHub | Todas las páginas de esa ciudad | Crear contenedor local fuerte |
| GeoArticle | Página servicio + ciudad | Pasar relevancia al convertidor |
| GeoArticle | GeoHub | Reforzar ciudad |
| GeoArticle | Otro GeoArticle relacionado | Crear cluster semántico |


# 1. Homepage Internal Linking Rules


La homepage es la raíz de la entidad. Desde ahí se distribuye autoridad hacia:

Servicios principales
Ciudad principal
Categorías adicionales
Contacto


## Lo que tienes que rellenar


Homepage URL:

Main GeoHub URL:

Core Service Overview URLs:
1.
2.
3.
4.
5.

Additional Category URLs:
1.
2.

Contact URL:

Preferred homepage anchors:
1.
2.
3.
4.
5.


## Ejemplo rellenado


Homepage URL:
/

Main GeoHub URL:
/miami/

Core Service Overview URLs:
1. /locksmith/emergency-locksmith/
2. /locksmith/car-locksmith/
3. /locksmith/residential-locksmith/
4. /locksmith/commercial-locksmith/
5. /locksmith/lock-rekeying/

Additional Category URLs:
1. /locksmith/miami/key-duplication/

Contact URL:
/contact/

Preferred homepage anchors:
1. Emergency locksmith services
2. Car locksmith support
3. Residential locksmith services
4. Commercial locksmith solutions
5. Locksmith services in Miami


## Homepage must link to


| Target | URL | Anchor recomendado |
| --- | --- | --- |
| Emergency Locksmith Service | /locksmith/emergency-locksmith/ | emergency locksmith services |
| Car Locksmith Service | /locksmith/car-locksmith/ | car locksmith support |
| Residential Locksmith Service | /locksmith/residential-locksmith/ | residential locksmith services |
| Commercial Locksmith Service | /locksmith/commercial-locksmith/ | commercial locksmith solutions |
| Lock Rekeying Service | /locksmith/lock-rekeying/ | lock rekeying services |
| Main GeoHub | /miami/ | locksmith services in Miami |
| Additional Category | /locksmith/miami/key-duplication/ | key duplication in Miami |
| Contact | /contact/ | contact ABC Locksmith |


# 2. Service Overview Internal Linking Rules


Las Service Overview Pages son pilares temáticos.

Ejemplo:

/locksmith/emergency-locksmith/

Esta página debe empujar todas sus versiones locales:

/locksmith/miami/emergency-locksmith/
/locksmith/hialeah/emergency-locksmith/
/locksmith/coral-gables/emergency-locksmith/
/locksmith/doral/emergency-locksmith/
/locksmith/hollywood/emergency-locksmith/


## Service Overview must link to


| Target | URL | Anchor recomendado |
| --- | --- | --- |
| Homepage | / | ABC Locksmith |
| Miami version | /locksmith/miami/emergency-locksmith/ | emergency locksmith in Miami |
| Hialeah version | /locksmith/hialeah/emergency-locksmith/ | emergency locksmith in Hialeah |
| Coral Gables version | /locksmith/coral-gables/emergency-locksmith/ | emergency locksmith in Coral Gables |
| Doral version | /locksmith/doral/emergency-locksmith/ | emergency locksmith in Doral |
| Hollywood version | /locksmith/hollywood/emergency-locksmith/ | emergency locksmith in Hollywood |
| Related Service | /locksmith/car-locksmith/ | car locksmith services |
| Related Service | /locksmith/residential-locksmith/ | residential locksmith services |
| Related Article | /miami/emergency-locksmith-cost-guide/ | emergency locksmith cost guide |


# 3. Location-Based Service Internal Linking Rules


Las Location-Based Service Pages son páginas comerciales de conversión local.

Ejemplo:

/locksmith/miami/emergency-locksmith/

Debe conectar tres niveles:

Servicio padre
Ciudad
Artículos de soporte


## Location-Based Service must link to


| Target | URL | Anchor recomendado |
| --- | --- | --- |
| Parent Service | /locksmith/emergency-locksmith/ | emergency locksmith services |
| GeoHub | /miami/ | locksmith services in Miami |
| Related Same City | /locksmith/miami/car-locksmith/ | car locksmith help in Miami |
| Related Same City | /locksmith/miami/residential-locksmith/ | residential locksmith services in Miami |
| Related Same City | /locksmith/miami/lock-rekeying/ | lock rekeying in Miami |
| Nearby City Version | /locksmith/hialeah/emergency-locksmith/ | emergency locksmith in Hialeah |
| GeoArticle | /miami/what-to-do-locked-out-of-house/ | what to do if you are locked out in Miami |
| GeoArticle | /miami/emergency-locksmith-cost-guide/ | emergency locksmith cost in Miami |
| Contact | /contact/ | call ABC Locksmith |


# 4. Additional Category Internal Linking Rules


Ejemplo:

/locksmith/miami/key-duplication/

No debe quedar como página suelta. Debe integrarse en el silo local de la ciudad.


## Additional Category must link to


| Target | URL | Anchor recomendado |
| --- | --- | --- |
| GeoHub | /miami/ | locksmith services in Miami |
| Related Service | /locksmith/miami/residential-locksmith/ | residential locksmith services in Miami |
| Related Service | /locksmith/miami/commercial-locksmith/ | commercial locksmith services in Miami |
| Related Service | /locksmith/miami/lock-rekeying/ | lock rekeying in Miami |
| Related Article | /miami/key-duplication-vs-rekeying/ | key duplication vs rekeying in Miami |
| Service Overview | /locksmith/lock-rekeying/ | lock rekeying services |


# 5. GeoHub Internal Linking Rules


El GeoHub es el contenedor de ciudad.

Ejemplo:

/miami/

Debe enlazar a todo lo importante dentro de Miami:

Servicios en Miami
Categorías adicionales en Miami
Artículos de Miami
Homepage
Contacto


## GeoHub must link to


| Target | URL | Anchor recomendado |
| --- | --- | --- |
| Homepage | / | ABC Locksmith |
| Emergency Locksmith Miami | /locksmith/miami/emergency-locksmith/ | emergency locksmith in Miami |
| Car Locksmith Miami | /locksmith/miami/car-locksmith/ | car locksmith in Miami |
| Residential Locksmith Miami | /locksmith/miami/residential-locksmith/ | residential locksmith in Miami |
| Commercial Locksmith Miami | /locksmith/miami/commercial-locksmith/ | commercial locksmith in Miami |
| Lock Rekeying Miami | /locksmith/miami/lock-rekeying/ | lock rekeying in Miami |
| Key Duplication Miami | /locksmith/miami/key-duplication/ | key duplication in Miami |
| GeoArticle | /miami/emergency-locksmith-cost-guide/ | emergency locksmith cost guide in Miami |
| GeoArticle | /miami/what-to-do-locked-out-of-house/ | locked out of your house in Miami |
| Contact | /contact/ | contact ABC Locksmith |


# 6. GeoArticle Internal Linking Rules


Los GeoArticles son boosters semánticos.

Ejemplo:

/miami/emergency-locksmith-cost-guide/

No deben vivir aislados como posts de blog genéricos. Cada GeoArticle debe enlazar a:

La página servicio + ciudad correspondiente
El GeoHub de la ciudad
Otro artículo relacionado


## GeoArticle must link to


| Target | URL | Anchor recomendado |
| --- | --- | --- |
| Matching Service Page | /locksmith/miami/emergency-locksmith/ | emergency locksmith in Miami |
| GeoHub | /miami/ | locksmith services in Miami |
| Related Article | /miami/what-to-do-locked-out-of-house/ | what to do if you are locked out in Miami |
| Optional Related Service | /locksmith/miami/lock-rekeying/ | lock rekeying in Miami |
| Contact | /contact/ | call ABC Locksmith |


# 7. Contact Page Linking Rules


La página de contacto también importa.


## Contact page should link to


Homepage
Main GeoHub
Top 3 Service Overview Pages
GBP URL


# Anchor Text Rules


No queremos que todos los enlaces usen exactamente el mismo anchor.

Mal:

emergency locksmith Miami
emergency locksmith Miami
emergency locksmith Miami
emergency locksmith Miami

Mejor:

emergency locksmith in Miami
urgent locksmith help in Miami
Miami lockout assistance
learn more about emergency locksmith services
get help from a Miami locksmith


## Tipos de anchor text


| Tipo | Ejemplo | Cuándo usar |
| --- | --- | --- |
| Exact match | emergency locksmith in Miami | 1–2 veces por página importante |
| Partial match | urgent locksmith help in Miami | Para variar semánticamente |
| Branded | ABC Locksmith | Para homepage y contacto |
| CTA | call ABC Locksmith today | Para conversión |
| Informational | learn what to do if you’re locked out | Para GeoArticles |
| Local entity | locksmith services in Miami | Para GeoHubs |
| Related service | car locksmith help in Miami | Para páginas relacionadas |


## Minimum internal links per page


| Page Type | Minimum Internal Links | Ideal Internal Links |
| --- | --- | --- |
| Homepage | 6 | 8–12 |
| Service Overview | 6 | 8–10 |
| Location-Based Service | 5 | 7–9 |
| Additional Category | 4 | 6–8 |
| GeoHub | 8 | 12–20 |
| GeoArticle | 3 | 4–6 |
| Contact Page | 4 | 5–7 |


## Internal link placement rules


Lugares recomendados:

Intro section
Service blocks
Contextual body paragraphs
FAQ answers
Related services section
Related articles section
CTA block
Breadcrumbs
Footer

Prioridad:

1. Contextual body links
2. Service blocks
3. Related resources
4. Breadcrumbs
5. Footer


## Breadcrumb Rules


Homepage:
Home

Service Overview:
Home > Locksmith > Emergency Locksmith

Location-Based Service:
Home > Locksmith > Miami > Emergency Locksmith

Additional Category:
Home > Miami > Key Duplication in Miami

GeoHub:
Home > Miami

GeoArticle:
Home > Miami > Emergency Locksmith Cost Guide


## Matriz completa para ABC Locksmith


Homepage `/` debe enlazar a:

/locksmith/emergency-locksmith/
/locksmith/car-locksmith/
/locksmith/residential-locksmith/
/locksmith/commercial-locksmith/
/locksmith/lock-rekeying/
/miami/
/locksmith/miami/key-duplication/
/contact/

Service Overview `/locksmith/emergency-locksmith/` debe enlazar a:

/
/locksmith/miami/emergency-locksmith/
/locksmith/hialeah/emergency-locksmith/
/locksmith/coral-gables/emergency-locksmith/
/locksmith/doral/emergency-locksmith/
/locksmith/hollywood/emergency-locksmith/
/locksmith/car-locksmith/
/locksmith/residential-locksmith/
/miami/emergency-locksmith-cost-guide/

GeoHub `/miami/` debe enlazar a:

/
/contact/
/locksmith/miami/emergency-locksmith/
/locksmith/miami/car-locksmith/
/locksmith/miami/residential-locksmith/
/locksmith/miami/commercial-locksmith/
/locksmith/miami/lock-rekeying/
/locksmith/miami/key-duplication/
/miami/what-to-do-locked-out-of-house/
/miami/emergency-locksmith-cost-guide/
/miami/how-fast-can-locksmith-arrive/


## Reglas anti-error


Error 1 — Enlazar todo con todo.

Correcto:

Cada página enlaza a páginas relacionadas por servicio, ciudad o intención.

Error 2 — No enlazar de vuelta.

Correcto:

Service Overview ↔ City Service Page

Error 3 — GeoArticles sin enlaces comerciales.

Correcto:

Cada GeoArticle enlaza a su Location-Based Service Page correspondiente.

Error 4 — GeoHub débil.

Correcto:

/miami/

Debe listar y enlazar:

Servicios en Miami
Categorías adicionales en Miami
Artículos de Miami
Contacto


## Sistema de enlaces por prioridad


P1 links:

Homepage → top services
Homepage → main GeoHub
Service Overview → city versions
Location-Based Service → parent service + GeoHub
GeoArticle → matching service page
GeoHub → all city-service pages

P2 links:

Location-Based Service → related services same city
Service Overview → related services
Additional Category → related services
GeoArticle → related article

P3 links:

Same service in nearby cities
Older articles
Comparison content
FAQ support pages


## Cómo añadir esto a la matriz del Paso 3


Añadimos estas columnas:

Internal Links Required
Internal Links Optional
Inbound Links Expected
Anchor Text Suggestions
Breadcrumb Path
Link Priority


## Output final del Paso 6


Reglas de enlaces internos por tipo de página
Anchors recomendados
Links obligatorios
Links opcionales
Inbound links esperados
Breadcrumb paths
Matriz de enlazado para homepage
Matriz de enlazado para servicios
Matriz de enlazado para GeoHubs
Matriz de enlazado para Location-Based Service Pages
Matriz de enlazado para Additional Category Pages
Matriz de enlazado para GeoArticles
Reglas anti-canibalización
Reglas anti-silo roto


# Paso 7 — Priority Score


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


# Paso 8 — QA Checklist


## Objetivo del Paso 8


Ahora creamos la checklist de control antes de publicar cualquier página.

Hasta ahora hemos definido:

Qué páginas crear
Qué URLs usar
Qué debe contener cada tipo de página
Cómo enlazarlas
Qué publicar primero

Pero antes de publicar, cada página debe pasar una revisión de calidad para evitar errores como:

Páginas duplicadas
URLs mal construidas
H1s genéricos
Metas sin ciudad o servicio
Contenido thin
Schema incorrecto
Falta de enlaces internos
Falta de CTA
Falta de NAP
Fingir ubicación física
Canibalización entre páginas


## Lo que tienes que rellenar


Para cada página, rellenas esta ficha:

Page ID:

Page Type:
Homepage / Service Overview / Location-Based Service / Additional Category / GeoHub / GeoArticle

URL:

Target Service:

Target City:

Primary GBP Category:

Additional GBP Category Supported:
Yes / No
Category:

Priority:
P1 / P2 / P3 / P4

Status:
Draft / Ready for QA / Approved / Published / Needs Revision

Reviewer:

QA Date:

Physical office in this city?
Yes / No

Can the page mention “office”, “location” or “visit us” in this city?
Yes / No

Main Parent Page:

Required Internal Links:
1.
2.
3.
4.
5.

Required Schema:

Notes:


## Ejemplo rellenado


Page ID:
LBS-001

Page Type:
Location-Based Service

URL:
/locksmith/miami/emergency-locksmith/

Target Service:
Emergency Locksmith

Target City:
Miami

Primary GBP Category:
Locksmith

Additional GBP Category Supported:
Yes
Category:
Emergency Locksmith Service

Priority:
P1

Status:
Ready for QA

Reviewer:
SEO Manager

QA Date:
2026-04-23

Physical office in this city?
Yes

Can the page mention “office”, “location” or “visit us” in this city?
Yes

Main Parent Page:
/locksmith/emergency-locksmith/

Required Internal Links:
1. /locksmith/emergency-locksmith/
2. /miami/
3. /locksmith/miami/car-locksmith/
4. /locksmith/miami/residential-locksmith/
5. /miami/emergency-locksmith-cost-guide/

Required Schema:
LocalBusiness
BreadcrumbList
FAQPage
Speakable

Notes:
This page supports the core Emergency Locksmith service, the Miami GeoHub, and the additional GBP category Emergency Locksmith Service.


## QA Checklist general


| Check | Pregunta | Estado |
| --- | --- | --- |
| URL correcta | ¿La URL sigue las reglas del Paso 4? | ⬜ |
| Page type correcto | ¿La página corresponde al tipo correcto? | ⬜ |
| Servicio único | ¿La página se centra en un solo servicio? | ⬜ |
| Ciudad única | ¿La página se centra en una sola ciudad, si aplica? | ⬜ |
| H1 correcto | ¿El H1 incluye marca, servicio y/o ciudad según el tipo de página? | ⬜ |
| Meta title | ¿Incluye servicio, ciudad y marca cuando corresponde? | ⬜ |
| Meta description | ¿Tiene intención clara y menos de 160 caracteres? | ⬜ |
| Contenido mínimo | ¿Cumple el word count del tipo de página? | ⬜ |
| AUDIO structure | ¿Incluye Authority, Uniqueness, Depth, Intent y Optimization cuando aplica? | ⬜ |
| FAQs | ¿Incluye preguntas reales, útiles y orientadas a AI Overview? | ⬜ |
| CTA | ¿Tiene una llamada a la acción clara? | ⬜ |
| Internal links | ¿Incluye todos los enlaces obligatorios? | ⬜ |
| Breadcrumbs | ¿La ruta de navegación es lógica? | ⬜ |
| Schema | ¿El schema coincide con el tipo de página? | ⬜ |
| NAP | ¿El NAP es correcto y consistente? | ⬜ |
| No ubicación falsa | ¿No afirma oficina física donde no existe? | ⬜ |
| No canibalización | ¿No compite con otra URL existente? | ⬜ |
| GBP alignment | ¿Apoya la categoría principal o adicional del GBP? | ⬜ |
| Publish ready | ¿La página está lista para publicar? | ⬜ |


# 1. Homepage QA Checklist


## Lo que tienes que rellenar


Homepage URL:

Brand Name:

Primary Service:

Primary GBP Category:

Main City:

H1:

Meta Title:

Meta Description:

Core Services Included:
1.
2.
3.
4.
5.

NAP Present?
Yes / No

Main CTA Present?
Yes / No

Trust Signals Included?
Yes / No

Service Overview Links Included?
Yes / No

Main GeoHub Link Included?
Yes / No

Additional Category Links Included?
Yes / No

Schema Added:
Organization / WebSite / LocalBusiness / FAQPage / Speakable

Homepage Approved?
Yes / No


## Ejemplo rellenado


Homepage URL:
/

Brand Name:
ABC Locksmith

Primary Service:
Locksmith Services

Primary GBP Category:
Locksmith

Main City:
Miami

H1:
ABC Locksmith – Trusted Locksmith Services in Miami, FL

Meta Title:
Top-Rated Locksmith in Miami, FL | ABC Locksmith

Meta Description:
Need a trusted locksmith in Miami? ABC Locksmith offers emergency, car, residential, commercial and rekeying services. Call today.

Core Services Included:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying

NAP Present?
Yes

Main CTA Present?
Yes

Trust Signals Included?
Yes

Service Overview Links Included?
Yes

Main GeoHub Link Included?
Yes

Additional Category Links Included?
Yes

Schema Added:
Organization
WebSite
LocalBusiness
FAQPage
Speakable

Homepage Approved?
Yes


# 2. Service Overview QA Checklist


## Lo que tienes que rellenar


Service Overview URL:

Service Name:

Primary Category:

Contains city in URL?
Yes / No

Contains city as main target?
Yes / No

H1:

Meta Title:

Meta Description:

Word Count:

AUDIO Sections Present?
Authority: Yes / No
Uniqueness: Yes / No
Depth: Yes / No
Intent: Yes / No
Optimization: Yes / No

FAQs Included?
Yes / No

Links to city-specific versions?
Yes / No

Links to related services?
Yes / No

Schema Added:
Service / WebPage / BreadcrumbList / Speakable

Approved?
Yes / No


## Ejemplo rellenado


Service Overview URL:
/locksmith/emergency-locksmith/

Service Name:
Emergency Locksmith

Primary Category:
Locksmith

Contains city in URL?
No

Contains city as main target?
No

H1:
Professional Emergency Locksmith Services by ABC Locksmith

Meta Title:
Emergency Locksmith by ABC Locksmith | Locksmith Experts

Meta Description:
Need trusted emergency locksmith help? ABC Locksmith delivers fast, careful and professional lockout support when access can’t wait.

Word Count:
950

AUDIO Sections Present?
Authority: Yes
Uniqueness: Yes
Depth: Yes
Intent: Yes
Optimization: Yes

FAQs Included?
Yes

Links to city-specific versions?
Yes

Links to related services?
Yes

Schema Added:
Service
WebPage
BreadcrumbList
Speakable

Approved?
Yes


# 3. Location-Based Service QA Checklist


## Lo que tienes que rellenar


Location-Based Service URL:

Service:

City:

Primary Category:

H1:

Meta Title:

Meta Description:

Word Count:

Does URL follow /category/city/service/?
Yes / No

One service only?
Yes / No

One city only?
Yes / No

Local intro present?
Yes / No

Neighborhoods or local references included?
Yes / No

AUDIO Sections Present?
Authority: Yes / No
Uniqueness: Yes / No
Depth: Yes / No
Intent: Yes / No
Optimization: Yes / No

FAQs Included?
Yes / No

CTA Included?
Yes / No

Parent Service linked?
Yes / No

GeoHub linked?
Yes / No

Related same-city services linked?
Yes / No

GeoArticles linked?
Yes / No

Physical office in this city?
Yes / No

Any false office/location claim?
Yes / No

Schema Added:
LocalBusiness / BreadcrumbList / FAQPage / Speakable

Approved?
Yes / No


## Ejemplo rellenado


Location-Based Service URL:
/locksmith/miami/emergency-locksmith/

Service:
Emergency Locksmith

City:
Miami

Primary Category:
Locksmith

H1:
ABC Locksmith – Emergency Locksmith in Miami

Meta Title:
Top Emergency Locksmith in Miami | ABC Locksmith

Meta Description:
Locked out in Miami? ABC Locksmith helps with urgent lockouts, broken keys, rekeying and secure access support. Call today.

Word Count:
925

Does URL follow /category/city/service/?
Yes

One service only?
Yes

One city only?
Yes

Local intro present?
Yes

Neighborhoods or local references included?
Yes

AUDIO Sections Present?
Authority: Yes
Uniqueness: Yes
Depth: Yes
Intent: Yes
Optimization: Yes

FAQs Included?
Yes

CTA Included?
Yes

Parent Service linked?
Yes

GeoHub linked?
Yes

Related same-city services linked?
Yes

GeoArticles linked?
Yes

Physical office in this city?
Yes

Any false office/location claim?
No

Schema Added:
LocalBusiness
BreadcrumbList
FAQPage
Speakable

Approved?
Yes


# 4. Additional Category Page QA Checklist


Additional Category Page URL:

Additional GBP Category:

Service Name Used on Page:

City:

Primary Category:

H1:

Meta Title:

Meta Description:

Word Count:

Does this category already exist as a core service?
Yes / No

If yes, should this page exist?
Yes / No

One city only?
Yes / No

One service/category only?
Yes / No

Local problem/scenario in intro?
Yes / No

AUDIO Sections Present?
Authority: Yes / No
Uniqueness: Yes / No
Depth: Yes / No
Intent: Yes / No
Optimization: Yes / No

FAQs Included?
Yes / No

GeoHub linked?
Yes / No

Related services linked?
Yes / No

Related GeoArticles linked?
Yes / No

Schema Added:
Service with areaServed / BreadcrumbList / FAQPage / Speakable

Approved?
Yes / No


# 5. GeoHub Page QA Checklist


GeoHub URL:

City:

Industry / Service Group:

H1:

Meta Title:

Meta Description:

Word Count:

Does URL follow /city/ or /category/city/?
Yes / No

Is this page focused on one city only?
Yes / No

Does it list all services in this city?
Yes / No

Does it list additional category pages?
Yes / No

Does it list GeoArticles?
Yes / No

Does it link to homepage?
Yes / No

Does it link to contact page?
Yes / No

Does it include neighborhoods / nearby areas?
Yes / No

Does it include trust signals?
Yes / No

Physical office in this city?
Yes / No

Any false office/location claim?
Yes / No

Schema Added:
CollectionPage / BreadcrumbList / LocalBusiness if valid

Approved?
Yes / No


# 6. GeoArticle QA Checklist


GeoArticle URL:

Article Topic:

Service Supported:

City:

Long-Tail Keyword:

Intent Type:
Informational / Pain Point / Navigational / Comparison / Awareness

H1:

Meta Title:

Meta Description:

Word Count:

One service only?
Yes / No

One city only?
Yes / No

One long-tail intent only?
Yes / No

Does it avoid acting like a landing page?
Yes / No

Local references included?
Yes / No

FAQs Included?
Yes / No

Matching Location-Based Service Page linked?
Yes / No

Matching GeoHub linked?
Yes / No

Related GeoArticle linked?
Yes / No

CTA links back to core service?
Yes / No

Physical office in this city?
Yes / No

Any false office/location claim?
Yes / No

Schema Added:
Article / FAQPage / BreadcrumbList / Speakable

Approved?
Yes / No


## Schema QA Checklist


| Page Type | Required Schema | QA Status |
| --- | --- | --- |
| Homepage | Organization, WebSite, LocalBusiness if valid, FAQPage, Speakable | ⬜ |
| Service Overview | Service, WebPage, BreadcrumbList, Speakable | ⬜ |
| Location-Based Service | LocalBusiness, BreadcrumbList, FAQPage optional, Speakable optional | ⬜ |
| Additional Category | Service with areaServed, BreadcrumbList, FAQPage optional | ⬜ |
| GeoHub | CollectionPage, BreadcrumbList, LocalBusiness if valid | ⬜ |
| GeoArticle | Article, FAQPage, BreadcrumbList, Speakable | ⬜ |


## Internal Linking QA Checklist


| Page Type | Must Link To | QA |
| --- | --- | --- |
| Homepage | Service Overviews, Main GeoHub, Additional Category Pages | ⬜ |
| Service Overview | City-specific versions, homepage, related services, GeoArticles | ⬜ |
| Location-Based Service | Parent service, GeoHub, same-city services, GeoArticles | ⬜ |
| Additional Category | GeoHub, related services, related GeoArticles | ⬜ |
| GeoHub | All services, additional categories and articles for that city | ⬜ |
| GeoArticle | Matching service page, GeoHub, related article | ⬜ |


## NAP QA Checklist


Business Name:
Must match GBP exactly.

Address:
Must match GBP if displayed.

Phone:
Must match GBP and be clickable.

City:
Must not imply false office location.

GBP URL:
Should be used in sameAs where appropriate.

Footer NAP:
Should be consistent sitewide.

Contact page NAP:
Should match homepage and schema.


## Canibalización QA Checklist


Antes de publicar una página, hay que comprobar que no existe otra URL atacando la misma intención.

Does another page target the same service + city?
Does another page have the same H1 intent?
Does another page have nearly identical meta title?
Does a GeoArticle compete with a Location-Based Service Page?
Does an Additional Category Page duplicate a Core Service Page?
Does a Service Overview accidentally target a city?


## False Location QA Checklist


Si no hay oficina física en esa ciudad, no usar:

Our [City] office
Visit our [City] location
Our storefront in [City]
Located in downtown [City]
Come see us in [City]

Frases permitidas para service areas:

We serve customers in [City]
Our mobile team helps customers across [City]
We provide [Service] in [City]
Customers in [City] can contact us for support


## Final Publish Gate


URL approved:
Yes / No

Content approved:
Yes / No

SEO metadata approved:
Yes / No

Schema approved:
Yes / No

Internal links approved:
Yes / No

NAP approved:
Yes / No

No canibalization:
Yes / No

No false location claim:
Yes / No

CTA approved:
Yes / No

Ready to publish:
Yes / No


## Cómo añadirlo a la matriz del Paso 3


QA Status
URL Approved
H1 Approved
Metadata Approved
Word Count Approved
Schema Approved
Internal Links Approved
NAP Approved
No Canibalization
No False Location Claim
CTA Approved
Final Approval
Reviewer
QA Date
Revision Notes


## Resultado final del Paso 8


Homepage
Service Overview Pages
Location-Based Service Pages
Additional Category Pages
GeoHub Pages
GeoArticle Pages
Schema
Internal links
NAP
Canibalización
Falsas ubicaciones
Publicación final


# Paso 9 — Producción en fases


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


# Paso 10 — Pseudocódigo del sistema


## Objetivo del Paso 10


Ahora convertimos todo lo anterior en una lógica casi automática.

Hasta ahora hemos diseñado el sistema manualmente:

Inputs
Arquitectura
URLs
Tipos de página
Enlaces internos
Prioridades
QA
Fases

En este paso lo convertimos en un motor lógico que pueda generar una matriz completa para cualquier negocio local.


## Lo que tienes que rellenar


Business Name:

Website Root Domain:

Canonical Domain:
https://www.domain.com or https://domain.com

Primary GBP Category:

Primary Category Slug:

Main City:

Physical Location City:

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

Service Slugs:
1.
2.
3.
4.
5.

Additional GBP Categories:
1.
2.
3.

Additional Category Slugs:
1.
2.
3.

Additional Categories Already Covered by Core Services:
1.
2.

Effective Additional Categories That Need Pages:
1.
2.

GeoArticles per Service x City:
Default: 3

GeoHub URL Style:
/city/ or /category/city/

GeoArticle URL Style:
/city/article-topic/ or /category/city/article-topic/

Phone:

Email:

NAP:
- Name:
- Address:
- Phone:

GBP URL:

Top Priority Services:
1.
2.
3.

Top Priority Cities:
1.
2.
3.

Publishing Capacity:
Pages per week:

Tracking Tools:
GMB Crush / GSC / GA4 / Other


## Ejemplo rellenado


Business Name:
ABC Locksmith

Website Root Domain:
https://www.abclocksmith.com

Canonical Domain:
https://www.abclocksmith.com

Primary GBP Category:
Locksmith

Primary Category Slug:
locksmith

Main City:
Miami

Physical Location City:
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

Service Slugs:
1. emergency-locksmith
2. car-locksmith
3. residential-locksmith
4. commercial-locksmith
5. lock-rekeying

Additional GBP Categories:
1. Emergency Locksmith Service
2. Key Duplication Service

Additional Category Slugs:
1. emergency-locksmith
2. key-duplication

Additional Categories Already Covered by Core Services:
1. Emergency Locksmith Service

Effective Additional Categories That Need Pages:
1. Key Duplication Service

GeoArticles per Service x City:
3

GeoHub URL Style:
/city/

GeoArticle URL Style:
/city/article-topic/

Phone:
+1 305 000 0000

Email:
info@abclocksmith.com

NAP:
- Name: ABC Locksmith
- Address: 123 Main St, Miami, FL
- Phone: +1 305 000 0000

GBP URL:
https://google.com/business/abc-locksmith

Top Priority Services:
1. Emergency Locksmith
2. Car Locksmith
3. Commercial Locksmith

Top Priority Cities:
1. Miami
2. Hialeah
3. Coral Gables

Publishing Capacity:
5 pages per week

Tracking Tools:
GMB Crush Geo Grid, Google Search Console, GA4


## Pseudocódigo general


START

1. Load business inputs
2. Normalize all names and slugs
3. Validate GBP category alignment
4. Detect duplicate additional categories
5. Generate Homepage
6. Generate Service Overview Pages
7. Generate GeoHub Pages
8. Generate Location-Based Service Pages
9. Generate Additional Category Pages
10. Generate GeoArticle Ideas
11. Assign schema by page type
12. Assign internal links by page type
13. Calculate Priority Score
14. Assign publishing phase
15. Run QA checklist
16. Output URL Matrix
17. Output Internal Linking Matrix
18. Output Schema Map
19. Output Publishing Plan
20. Output QA Status

END


## 1. Cargar inputs


INPUT business_name
INPUT website_root_domain
INPUT canonical_domain
INPUT primary_gbp_category
INPUT primary_category_slug
INPUT main_city
INPUT physical_location_city
INPUT target_cities[]
INPUT core_services[]
INPUT service_slugs[]
INPUT additional_gbp_categories[]
INPUT geoarticles_per_service_city
INPUT phone
INPUT email
INPUT nap
INPUT gbp_url


## 2. Normalizar slugs


FUNCTION generate_slug(text):
    text = lowercase(text)
    text = remove_accents(text)
    text = replace_spaces_with_hyphens(text)
    text = remove_symbols(text)
    text = remove_duplicate_hyphens(text)
    RETURN text

Ejemplo:

"Emergency Locksmith" → "emergency-locksmith"
"Coral Gables" → "coral-gables"
"Key Duplication Service" → "key-duplication"


## 3. Validar categorías adicionales


Objetivo: evitar duplicar páginas cuando una categoría adicional ya está cubierta por un servicio principal.

effective_additional_categories = []

FOR each additional_category IN additional_gbp_categories:
    IF additional_category matches core_service intent:
        mark_as_covered(additional_category)
    ELSE:
        add to effective_additional_categories

Ejemplo:

additional_gbp_categories = [
  "Emergency Locksmith Service",
  "Key Duplication Service"
]

core_services = [
  "Emergency Locksmith",
  "Car Locksmith",
  "Residential Locksmith",
  "Commercial Locksmith",
  "Lock Rekeying"
]

Result:
covered = ["Emergency Locksmith Service"]
effective_additional_categories = ["Key Duplication Service"]


## 4. Generar homepage


CREATE page
page.id = "HP-001"
page.type = "Homepage"
page.url = "/"
page.h1 = "[Business Name] – Trusted [Primary Service] in [Main City, ST]"
page.meta_title = "Top-Rated [Primary Service] in [Main City, ST] | [Business Name]"
page.schema = ["Organization", "WebSite", "LocalBusiness if valid", "FAQPage", "Speakable"]
page.priority = "P1"
page.phase = "Phase 1"
page.status = "Planned"


## 5. Generar Service Overview Pages


FOR each service IN core_services:

    service_slug = generate_slug(service)

    CREATE page
    page.id = "SO-" + counter
    page.type = "Service Overview"
    page.service = service
    page.city = null
    page.url = "/" + primary_category_slug + "/" + service_slug + "/"
    page.h1 = "Professional [Service] Services by [Business Name]"
    page.meta_title = "[Service] by [Business Name] | [Primary Category] Experts"
    page.schema = ["Service", "WebPage", "BreadcrumbList", "Speakable"]
    page.priority = calculate_service_priority(service)
    page.phase = assign_service_phase(priority)


## 6. Generar GeoHub Pages


FOR each city IN target_cities:

    city_slug = generate_slug(city)

    IF geohub_url_style == "/city/":
        url = "/" + city_slug + "/"
    ELSE:
        url = "/" + primary_category_slug + "/" + city_slug + "/"

    CREATE page
    page.id = "GH-" + counter
    page.type = "GeoHub"
    page.city = city
    page.url = url
    page.h1 = "[Business Name] – [Industry] Services in [City]"
    page.meta_title = "[Industry] Services in [City] | [Business Name]"
    page.schema = ["CollectionPage", "BreadcrumbList", "LocalBusiness if physical city"]
    page.priority = calculate_city_priority(city)
    page.phase = assign_geohub_phase(city)


## 7. Generar Location-Based Service Pages


FOR each city IN target_cities:
    FOR each service IN core_services:

        city_slug = generate_slug(city)
        service_slug = generate_slug(service)

        CREATE page
        page.id = "LBS-" + counter
        page.type = "Location-Based Service"
        page.service = service
        page.city = city
        page.url = "/" + primary_category_slug + "/" + city_slug + "/" + service_slug + "/"
        page.h1 = "[Business Name] – [Service] in [City]"
        page.meta_title = "Top [Service] in [City] | [Business Name]"
        page.schema = ["LocalBusiness", "BreadcrumbList", "FAQPage optional", "Speakable optional"]
        page.parent_service = "/" + primary_category_slug + "/" + service_slug + "/"
        page.geohub = "/" + city_slug + "/"
        page.priority_score = calculate_priority(service, city, page.type)
        page.phase = assign_phase(priority_score)


## 8. Generar Additional Category Pages


FOR each city IN target_cities:
    FOR each additional_category IN effective_additional_categories:

        city_slug = generate_slug(city)
        category_slug = generate_slug(additional_category)

        CREATE page
        page.id = "AC-" + counter
        page.type = "Additional Category"
        page.service = additional_category
        page.city = city
        page.url = "/" + primary_category_slug + "/" + city_slug + "/" + category_slug + "/"
        page.h1 = "[Business Name] – Expert [Service] in [City]"
        page.meta_title = "[Service] in [City] | [Business Name]"
        page.schema = ["Service with areaServed", "BreadcrumbList", "FAQPage optional"]
        page.geohub = "/" + city_slug + "/"
        page.priority_score = calculate_priority(additional_category, city, page.type)
        page.phase = assign_phase(priority_score)


## 9. Generar GeoArticle ideas


FOR each city IN target_cities:
    FOR each service IN core_services:
        FOR article_number FROM 1 TO geoarticles_per_service_city:

            article_topic = generate_article_topic(service, city, article_number)
            article_slug = generate_slug(article_topic)

            CREATE page
            page.id = "GA-" + counter
            page.type = "GeoArticle"
            page.service = service
            page.city = city
            page.url = "/" + city_slug + "/" + article_slug + "/"
            page.h1 = "[Article Topic] in [City]"
            page.meta_title = "[Article Topic] in [City] | [Business Name]"
            page.schema = ["Article", "FAQPage", "BreadcrumbList", "Speakable"]
            page.supports = "/" + primary_category_slug + "/" + city_slug + "/" + service_slug + "/"
            page.geohub = "/" + city_slug + "/"
            page.priority = assign_geoarticle_priority(service, city)
            page.phase = "Phase 3"


## 10. Asignar schema por tipo de página


FUNCTION assign_schema(page_type):

    IF page_type == "Homepage":
        RETURN ["Organization", "WebSite", "LocalBusiness if valid", "FAQPage", "Speakable"]

    IF page_type == "Service Overview":
        RETURN ["Service", "WebPage", "BreadcrumbList", "Speakable"]

    IF page_type == "Location-Based Service":
        RETURN ["LocalBusiness", "BreadcrumbList", "FAQPage optional", "Speakable optional"]

    IF page_type == "Additional Category":
        RETURN ["Service with areaServed", "BreadcrumbList", "FAQPage optional"]

    IF page_type == "GeoHub":
        RETURN ["CollectionPage", "BreadcrumbList", "LocalBusiness if valid"]

    IF page_type == "GeoArticle":
        RETURN ["Article", "FAQPage", "BreadcrumbList", "Speakable"]


## 11. Asignar enlaces internos


FUNCTION assign_internal_links(page):

    IF page.type == "Homepage":
        link_to Service Overview Pages
        link_to Main GeoHub
        link_to Main Additional Category Pages
        link_to Contact Page

    IF page.type == "Service Overview":
        link_to Homepage
        link_to all city-specific versions of same service
        link_to related Service Overview Pages
        link_to relevant GeoArticle

    IF page.type == "Location-Based Service":
        link_to parent Service Overview
        link_to matching GeoHub
        link_to other services in same city
        link_to same service in nearby cities
        link_to related GeoArticles
        link_to Contact Page

    IF page.type == "Additional Category":
        link_to matching GeoHub
        link_to related services in same city
        link_to related GeoArticles
        link_to Contact Page

    IF page.type == "GeoHub":
        link_to Homepage
        link_to all services in city
        link_to all additional categories in city
        link_to all GeoArticles in city
        link_to Contact Page

    IF page.type == "GeoArticle":
        link_to matching Location-Based Service Page
        link_to matching GeoHub
        link_to related GeoArticle
        link_to Contact Page


## 12. Calcular Priority Score


FUNCTION calculate_priority(service, city, page_type):

    revenue_value = get_revenue_value(service)
    search_intent = get_search_intent(service, page_type)
    gbp_relevance = get_gbp_relevance(service, primary_gbp_category, additional_categories)
    city_priority = get_city_priority(city)
    competition_gap = estimate_competition_gap(service, city)
    conversion_urgency = get_conversion_urgency(service)

    total_score =
        revenue_value
        + search_intent
        + gbp_relevance
        + city_priority
        + competition_gap
        + conversion_urgency

    IF total_score >= 26:
        priority = "P1"
    ELSE IF total_score >= 21:
        priority = "P2"
    ELSE IF total_score >= 16:
        priority = "P3"
    ELSE IF total_score >= 10:
        priority = "P4"
    ELSE:
        priority = "Hold"

    RETURN total_score, priority


## 13. Asignar fase de publicación


FUNCTION assign_publish_phase(page):

    IF page.type == "Homepage":
        RETURN "Phase 1"

    IF page.type == "Contact":
        RETURN "Phase 1"

    IF page.type == "Service Overview" AND page.priority == "P1":
        RETURN "Phase 1"

    IF page.type == "GeoHub" AND page.city == main_city:
        RETURN "Phase 1"

    IF page.type == "Location-Based Service" AND page.city == main_city:
        RETURN "Phase 2"

    IF page.type == "Additional Category" AND page.city == main_city:
        RETURN "Phase 2"

    IF page.type == "GeoHub" AND page.city != main_city:
        RETURN "Phase 2"

    IF page.type == "Location-Based Service" AND page.city != main_city:
        RETURN "Phase 2 or Phase 3 depending priority"

    IF page.type == "GeoArticle":
        RETURN "Phase 3"

    ELSE:
        RETURN "Phase 4 or Hold"


## 14. Comprobar dependencias


FUNCTION check_dependencies(page):

    IF page.type == "Location-Based Service":
        REQUIRE Homepage exists
        REQUIRE parent Service Overview exists
        REQUIRE matching GeoHub exists

    IF page.type == "Additional Category":
        REQUIRE Homepage exists
        REQUIRE matching GeoHub exists
        REQUIRE related services exist

    IF page.type == "GeoArticle":
        REQUIRE matching Location-Based Service Page exists
        REQUIRE matching GeoHub exists

    IF dependencies_missing:
        page.status = "Blocked"
    ELSE:
        page.status = "Ready for QA"


## 15. Ejecutar QA


FUNCTION run_qa(page):

    CHECK url_matches_page_type
    CHECK h1_matches_page_type
    CHECK meta_title_exists
    CHECK meta_description_exists
    CHECK word_count_matches_page_type
    CHECK one_service_only
    CHECK one_city_only_if_applicable
    CHECK schema_matches_page_type
    CHECK required_internal_links_exist
    CHECK nap_consistency
    CHECK no_false_location_claim
    CHECK no_canibalization
    CHECK cta_exists

    IF all_checks_pass:
        page.qa_status = "Approved"
    ELSE:
        page.qa_status = "Needs Revision"


## Output final del sistema


Debe generar 5 outputs:

1. URL Matrix
2. Internal Linking Matrix
3. Schema Map
4. Publishing Plan
5. QA Matrix


## Pseudocódigo completo en bloque único


START GMB_CRUSH_WEBSITE_BUILD_SYSTEM

INPUT:
    business_name
    website_root_domain
    canonical_domain
    primary_gbp_category
    primary_category_slug
    main_city
    physical_location_city
    target_cities[]
    core_services[]
    additional_gbp_categories[]
    phone
    email
    nap
    gbp_url
    geoarticles_per_service_city

NORMALIZE:
    Generate city_slugs[]
    Generate service_slugs[]
    Generate additional_category_slugs[]

VALIDATE:
    Confirm primary GBP category
    Confirm services support category
    Confirm cities are valid service areas
    Detect additional categories already covered by core services

GENERATE:
    Homepage
    Service Overview Pages for each core service
    GeoHub Pages for each target city
    Location-Based Service Pages for each service x city
    Additional Category Pages for each effective additional category x city
    GeoArticle ideas for each service x city x article count

ASSIGN:
    URL pattern by page type
    H1 by page type
    Meta title by page type
    Meta description by page type
    Schema by page type
    Internal links by page type
    Breadcrumb path by page type

SCORE:
    Calculate Revenue Value
    Calculate Search Intent
    Calculate GBP Category Relevance
    Calculate City Priority
    Calculate Competition Gap
    Calculate Conversion Urgency
    Generate Total Priority Score
    Assign P1 / P2 / P3 / P4 / Hold

PHASE:
    Assign Phase 1 Entity Foundation
    Assign Phase 2 Local Conversion Layer
    Assign Phase 3 Semantic Expansion Layer
    Assign Phase 4 Optimization Loop

CHECK DEPENDENCIES:
    Service pages require Homepage
    City-service pages require Service Overview + GeoHub
    GeoArticles require Location-Based Service Page + GeoHub
    Additional Category pages require GeoHub + related services

QA:
    Validate URL
    Validate page type
    Validate one service
    Validate one city
    Validate H1
    Validate metadata
    Validate schema
    Validate internal links
    Validate NAP
    Validate no false location claim
    Validate no canibalization
    Validate CTA

OUTPUT:
    URL Matrix
    Internal Linking Matrix
    Schema Map
    Publishing Plan
    QA Matrix

END


## Decisión final del Paso 10


A partir de este punto, el sistema ya no depende de memoria ni improvisación.

Para cualquier negocio local, el proceso será:

1. Rellenar inputs
2. Normalizar slugs
3. Generar arquitectura
4. Crear URLs
5. Asignar page type
6. Asignar schema
7. Asignar enlaces internos
8. Calcular prioridad
9. Asignar fase
10. Pasar QA
11. Publicar
12. Optimizar con tracking


# Paso 11 — Master Prompt reutilizable


## Objetivo del Paso 11


Ahora vamos a convertir todo el sistema en un prompt maestro que puedas reutilizar para cualquier negocio local.

Este prompt debe generar automáticamente:

Arquitectura completa
URL Matrix
Tipos de página
H1s
Meta titles
Meta descriptions
Schema recomendado
Internal linking map
Priority Score
Publishing phases
QA checklist
GeoArticle ideas

La idea es que puedas rellenar los datos de un negocio y obtener una estructura completa siguiendo GMB Crush.


## Lo que tienes que rellenar


Business Name:

Website Root Domain:

Canonical Domain:

Country:

State / Province:

Main City:

Physical Location City:

Full NAP:
- Business Name:
- Street Address:
- City:
- State / Province:
- ZIP / Postal Code:
- Country:
- Phone:

GBP URL:

Primary GBP Category:

Primary Category Slug:

Additional GBP Categories:
1.
2.
3.

Core Services:
1.
2.
3.
4.
5.

Service Slugs:
1.
2.
3.
4.
5.

Target Cities:
1.
2.
3.
4.
5.

City Slugs:
1.
2.
3.
4.
5.

Services available in every city?
Yes / No

If no, list exclusions:
- Service:
- City:
- Reason:

Additional Categories already covered by core services:
1.
2.

Additional Categories that need separate pages:
1.
2.

GeoArticles per Service x City:
Default: 3

GeoHub URL Style:
Option A: /city/
Option B: /category/city/

GeoArticle URL Style:
Option A: /city/article-topic/
Option B: /category/city/article-topic/

Top Priority Services:
1.
2.
3.

Top Priority Cities:
1.
2.
3.

Trust Signals:
- Years in business:
- Reviews:
- Certifications:
- Awards:
- Guarantees:
- Emergency / same-day / mobile service:

Preferred CTA:
Call now / Book online / Request estimate / Contact us

Publishing Capacity:
Pages per week:

CMS:
WordPress / Webflow / Shopify / Custom / Other

Can schema be added?
Yes / No

Can internal links be edited manually?
Yes / No

Tracking Tools:
GMB Crush / Google Search Console / GA4 / Rank Tracker / Other


## Ejemplo rellenado


Business Name:
ABC Locksmith

Website Root Domain:
https://www.abclocksmith.com

Canonical Domain:
https://www.abclocksmith.com

Country:
United States

State / Province:
Florida

Main City:
Miami

Physical Location City:
Miami

Full NAP:
- Business Name: ABC Locksmith
- Street Address: 123 Main St
- City: Miami
- State / Province: FL
- ZIP / Postal Code: 33101
- Country: United States
- Phone: +1 305 000 0000

GBP URL:
https://google.com/business/abc-locksmith

Primary GBP Category:
Locksmith

Primary Category Slug:
locksmith

Additional GBP Categories:
1. Emergency Locksmith Service
2. Key Duplication Service

Core Services:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying

Service Slugs:
1. emergency-locksmith
2. car-locksmith
3. residential-locksmith
4. commercial-locksmith
5. lock-rekeying

Target Cities:
1. Miami
2. Hialeah
3. Coral Gables
4. Doral
5. Hollywood

City Slugs:
1. miami
2. hialeah
3. coral-gables
4. doral
5. hollywood

Services available in every city?
Yes

Additional Categories already covered by core services:
1. Emergency Locksmith Service

Additional Categories that need separate pages:
1. Key Duplication Service

GeoArticles per Service x City:
3

GeoHub URL Style:
Option A: /city/

GeoArticle URL Style:
Option A: /city/article-topic/

Top Priority Services:
1. Emergency Locksmith
2. Car Locksmith
3. Commercial Locksmith

Top Priority Cities:
1. Miami
2. Hialeah
3. Coral Gables

Trust Signals:
- Years in business: 10+
- Reviews: 250+ Google reviews
- Certifications: Licensed locksmith technicians
- Awards: Local service award
- Guarantees: Workmanship guarantee
- Emergency / same-day / mobile service: Yes

Preferred CTA:
Call now

Publishing Capacity:
5 pages per week

CMS:
WordPress

Can schema be added?
Yes

Can internal links be edited manually?
Yes

Tracking Tools:
GMB Crush Geo Grid, Google Search Console, GA4


# Master Prompt reutilizable


Puedes copiarlo y usarlo para cualquier negocio local.

Actúa como Matteo de GMB Crush, especialista top 1% en Local SEO, Google Business Profile optimization, AI Overview visibility, semantic SEO, GeoHub architecture, internal linking y LocalBusiness site structure.

Quiero construir una web local desde cero siguiendo la metodología GMB Crush.

Usa exclusivamente esta jerarquía de páginas:

1. Homepage = Root Entity Anchor
2. Service Overview Pages = Topical Authority Pillars, no location
3. Location-Based Service Pages = Geo-Targeted Converters
4. Additional Category Pages = GBP additional category support
5. GeoHub Pages = City-Level Silo Containers
6. GeoArticle Pages = Semantic Boosters for service + city + long-tail intent

IMPORTANTE:
- No confundas Service Overview Pages con Location-Based Service Pages.
- No mezcles múltiples ciudades en una página local.
- No mezcles múltiples servicios en una página local.
- No crees páginas duplicadas para categorías adicionales que ya estén cubiertas por servicios principales.
- No afirmes que el negocio tiene oficina física en una ciudad si no se indica explícitamente.
- Cada categoría GBP, primaria o adicional, debe tener soporte mediante contenido local específico.
- Los GeoArticles no son landing pages; son boosters semánticos.
- Cada página debe tener función, URL, H1, metadata, schema, enlaces internos, prioridad y fase de publicación.

INPUTS DEL NEGOCIO:

Business Name:
[INSERT]

Website Root Domain:
[INSERT]

Canonical Domain:
[INSERT]

Country:
[INSERT]

State / Province:
[INSERT]

Main City:
[INSERT]

Physical Location City:
[INSERT]

Full NAP:
- Business Name: [INSERT]
- Street Address: [INSERT]
- City: [INSERT]
- State / Province: [INSERT]
- ZIP / Postal Code: [INSERT]
- Country: [INSERT]
- Phone: [INSERT]

GBP URL:
[INSERT]

Primary GBP Category:
[INSERT]

Primary Category Slug:
[INSERT]

Additional GBP Categories:
[INSERT LIST]

Core Services:
[INSERT LIST]

Service Slugs:
[INSERT LIST]

Target Cities:
[INSERT LIST]

City Slugs:
[INSERT LIST]

Services available in every city?
[YES / NO]

If no, list exclusions:
[INSERT]

Additional Categories already covered by core services:
[INSERT LIST]

Additional Categories that need separate pages:
[INSERT LIST]

GeoArticles per Service x City:
[INSERT NUMBER]

GeoHub URL Style:
[/city/ OR /category/city/]

GeoArticle URL Style:
[/city/article-topic/ OR /category/city/article-topic/]

Top Priority Services:
[INSERT LIST]

Top Priority Cities:
[INSERT LIST]

Trust Signals:
[INSERT LIST]

Preferred CTA:
[INSERT]

Publishing Capacity:
[INSERT NUMBER] pages per week

CMS:
[INSERT]

Can schema be added?
[YES / NO]

Can internal links be edited manually?
[YES / NO]

Tracking Tools:
[INSERT]

TASK:

Generate a complete GMB Crush website architecture system with the following outputs:

1. Executive summary
2. Inputs validation
3. Duplicate category detection
4. Total page count formula
5. Full URL Matrix
6. Page Type Rules
7. Homepage brief
8. Service Overview Pages
9. GeoHub Pages
10. Location-Based Service Pages
11. Additional Category Pages
12. GeoArticle ideas
13. Schema Map
14. Internal Linking Map
15. Priority Score
16. Publishing Phases
17. QA Checklist
18. Final implementation roadmap

OUTPUT REQUIREMENTS:

A. INPUT VALIDATION

Validate:
- Primary GBP category alignment
- Core services
- Additional GBP categories
- Cities
- Physical location city
- Service area cities
- Category duplication risks
- Missing slugs
- URL consistency

B. TOTAL PAGE COUNT

Use this formula:

1 Homepage
+ S Service Overview Pages
+ C GeoHub Pages
+ S × C Location-Based Service Pages
+ A × C Additional Category Pages
+ G × S × C GeoArticle Pages

Where:
S = number of core services
C = number of target cities
A = number of additional categories that need separate pages
G = number of GeoArticles per service x city

Return the total page count in a table.

C. URL RULES

Use these URL patterns:

Homepage:
/

Service Overview:
/[primary-category-slug]/[service-slug]/

Location-Based Service:
/[primary-category-slug]/[city-slug]/[service-slug]/

Additional Category:
/[primary-category-slug]/[city-slug]/[additional-category-slug]/

GeoHub:
Use selected style:
Option A: /[city-slug]/
Option B: /[primary-category-slug]/[city-slug]/

GeoArticle:
Use selected style:
Option A: /[city-slug]/[article-topic-slug]/
Option B: /[primary-category-slug]/[city-slug]/[article-topic-slug]/

D. URL MATRIX

Create a clean table with these columns:

ID
Page Type
Parent Page
Service
Service Slug
City
City Slug
Additional Category
URL
H1
Meta Title
Meta Description
Schema Type
Internal Links Required
Priority
Publish Phase
Status
Notes

E. PAGE TYPE RULES

For each page type, provide:
- Purpose
- URL pattern
- H1 formula
- Meta title formula
- Meta description formula
- Word count target
- Required sections
- FAQ requirements
- CTA requirements
- Schema required
- Internal links required

F. HOMEPAGE BRIEF

Generate:
- Homepage URL
- H1
- Meta title
- Meta description
- Quick Answer block
- Core service menu
- Trust blocks
- FAQ ideas
- Schema
- Internal links

G. SERVICE OVERVIEW PAGES

For each service, generate:
- URL
- H1
- Meta title
- Meta description
- Suggested H2s using AUDIO:
  Authority
  Uniqueness
  Depth
  Intent
  Optimization
- FAQs
- Internal links to city-specific versions
- Schema

H. GEOHUB PAGES

For each city, generate:
- URL
- H1
- Meta title
- Meta description
- Services available in this city
- Additional category pages in this city
- GeoArticle ideas for this city
- Internal links
- Schema

I. LOCATION-BASED SERVICE PAGES

For each Service × City combination, generate:
- URL
- H1
- Meta title
- Meta description
- Local intro angle
- AUDIO H2s
- FAQs
- CTA
- Parent service page
- Matching GeoHub page
- Related same-city services
- Related GeoArticles
- Schema

J. ADDITIONAL CATEGORY PAGES

For each Additional Category × City combination, generate:
- URL
- H1
- Meta title
- Meta description
- Local problem/scenario
- AUDIO H2s
- FAQs
- CTA
- Related services
- Matching GeoHub
- Schema

K. GEOARTICLE IDEAS

Generate [G] GeoArticle ideas for each Service × City pair.

For each GeoArticle, return:
- Page title
- H1
- URL
- Target long-tail keyword
- Intent type
- Summary
- Matching Location-Based Service Page
- Matching GeoHub Page
- Related GeoArticle
- Schema

L. SCHEMA MAP

Assign schema by page type:

Homepage:
Organization
WebSite
LocalBusiness if physical presence exists in main city
FAQPage
Speakable

Service Overview:
Service
WebPage
BreadcrumbList
Speakable

Location-Based Service:
LocalBusiness
BreadcrumbList
FAQPage optional
Speakable optional

Additional Category:
Service with areaServed
BreadcrumbList
FAQPage optional

GeoHub:
CollectionPage
BreadcrumbList
LocalBusiness only if physical presence exists in that city

GeoArticle:
Article
FAQPage
BreadcrumbList
Speakable

M. INTERNAL LINKING MAP

Apply this hierarchy:

Homepage links to:
- Service Overview Pages
- Main GeoHub
- Main Additional Category Pages
- Contact Page

Service Overview links to:
- Homepage
- All city-specific versions of that service
- Related Service Overview Pages
- Relevant GeoArticles

Location-Based Service links to:
- Parent Service Overview
- Matching GeoHub
- Other services in same city
- Same service in nearby cities
- Related GeoArticles
- Contact Page

Additional Category links to:
- Matching GeoHub
- Related services in same city
- Related GeoArticles
- Contact Page

GeoHub links to:
- Homepage
- All services in that city
- All additional category pages in that city
- All GeoArticles in that city
- Contact Page

GeoArticle links to:
- Matching Location-Based Service Page
- Matching GeoHub
- Related GeoArticle
- Optional related service
- Contact Page

For each source page, provide:
- Source URL
- Target URL
- Anchor text
- Link priority: P1 / P2 / P3
- Placement: intro, body, service block, FAQ, related resources, CTA, footer

N. PRIORITY SCORE

Calculate priority using:

Priority Score =
Revenue Value
+ Search Intent
+ GBP Category Relevance
+ City Priority
+ Competition Gap
+ Conversion Urgency

Each factor is scored from 1 to 5.

Priority tiers:
26–30 = P1
21–25 = P2
16–20 = P3
10–15 = P4
0–9 = Hold

O. PUBLISHING PHASES

Assign every page to one of these phases:

Phase 1: Entity Foundation
- Homepage
- Contact
- About
- Top Service Overview Pages
- Main GeoHub

Phase 2: Local Conversion Layer
- Main city service pages
- Additional category pages for main city
- Secondary GeoHubs
- High-intent service pages in secondary cities

Phase 3: Semantic Expansion Layer
- GeoArticles
- FAQ clusters
- Cost guides
- Comparison articles
- Mistake guides

Phase 4: Optimization Loop
- Internal link updates
- Metadata refresh
- FAQ expansion
- Schema QA
- Geo-grid review
- Search Console optimization

P. QA CHECKLIST

For each page, include QA checks:

- URL approved
- Page type correct
- One service only
- One city only if applicable
- H1 approved
- Meta title approved
- Meta description approved
- Word count approved
- AUDIO structure included
- FAQs included
- CTA included
- Schema approved
- Internal links approved
- NAP consistent
- No canibalization
- No false location claim
- Final approval status

Q. FINAL OUTPUT FORMAT

Return the answer in this structure:

1. Title + Summary Block
2. Inputs Validation
3. Page Count Formula
4. URL Matrix
5. Page Type Rules
6. Homepage Brief
7. Service Overview Matrix
8. GeoHub Matrix
9. Location-Based Service Matrix
10. Additional Category Matrix
11. GeoArticle Matrix
12. Schema Map
13. Internal Linking Map
14. Priority Score Table
15. Publishing Plan
16. QA Checklist
17. Final Takeaway

Use clean tables.
Be precise.
Do not invent physical locations.
Do not create duplicate pages.
Do not create pages with no clear parent, target, or internal link destination.


## Master Prompt rellenado con ABC Locksmith


Actúa como Matteo de GMB Crush, especialista top 1% en Local SEO, Google Business Profile optimization, AI Overview visibility, semantic SEO, GeoHub architecture, internal linking y LocalBusiness site structure.

Quiero construir una web local desde cero siguiendo la metodología GMB Crush.

INPUTS DEL NEGOCIO:

Business Name:
ABC Locksmith

Website Root Domain:
https://www.abclocksmith.com

Canonical Domain:
https://www.abclocksmith.com

Country:
United States

State / Province:
Florida

Main City:
Miami

Physical Location City:
Miami

Full NAP:
- Business Name: ABC Locksmith
- Street Address: 123 Main St
- City: Miami
- State / Province: FL
- ZIP / Postal Code: 33101
- Country: United States
- Phone: +1 305 000 0000

GBP URL:
https://google.com/business/abc-locksmith

Primary GBP Category:
Locksmith

Primary Category Slug:
locksmith

Additional GBP Categories:
1. Emergency Locksmith Service
2. Key Duplication Service

Core Services:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying

Service Slugs:
1. emergency-locksmith
2. car-locksmith
3. residential-locksmith
4. commercial-locksmith
5. lock-rekeying

Target Cities:
1. Miami
2. Hialeah
3. Coral Gables
4. Doral
5. Hollywood

City Slugs:
1. miami
2. hialeah
3. coral-gables
4. doral
5. hollywood

Services available in every city?
Yes

Additional Categories already covered by core services:
1. Emergency Locksmith Service

Additional Categories that need separate pages:
1. Key Duplication Service

GeoArticles per Service x City:
3

GeoHub URL Style:
/city/

GeoArticle URL Style:
/city/article-topic/

Top Priority Services:
1. Emergency Locksmith
2. Car Locksmith
3. Commercial Locksmith

Top Priority Cities:
1. Miami
2. Hialeah
3. Coral Gables

Trust Signals:
- 10+ years in business
- 250+ Google reviews
- Licensed locksmith technicians
- Local service award
- Workmanship guarantee
- Same-day mobile support

Preferred CTA:
Call now

Publishing Capacity:
5 pages per week

CMS:
WordPress

Can schema be added?
Yes

Can internal links be edited manually?
Yes

Tracking Tools:
GMB Crush Geo Grid, Google Search Console, GA4

TASK:
Generate a complete GMB Crush website architecture system with:
1. Executive summary
2. Inputs validation
3. Duplicate category detection
4. Total page count formula
5. Full URL Matrix
6. Page Type Rules
7. Homepage brief
8. Service Overview Pages
9. GeoHub Pages
10. Location-Based Service Pages
11. Additional Category Pages
12. GeoArticle ideas
13. Schema Map
14. Internal Linking Map
15. Priority Score
16. Publishing Phases
17. QA Checklist
18. Final implementation roadmap

Follow all GMB Crush rules exactly.
Return clean tables.
Do not invent physical locations.
Do not create duplicate pages.
Do not create pages with no clear parent, target, or internal link destination.


# Prompt auxiliar 1 — Solo para generar la URL Matrix


Actúa como Matteo de GMB Crush.

Con los inputs siguientes, genera únicamente la URL Matrix completa para una web local siguiendo la metodología GMB Crush.

Inputs:

Business Name:
[INSERT]

Website Root Domain:
[INSERT]

Primary GBP Category:
[INSERT]

Primary Category Slug:
[INSERT]

Main City:
[INSERT]

Physical Location City:
[INSERT]

Core Services:
[INSERT LIST]

Service Slugs:
[INSERT LIST]

Target Cities:
[INSERT LIST]

City Slugs:
[INSERT LIST]

Additional Categories that need separate pages:
[INSERT LIST]

Additional Category Slugs:
[INSERT LIST]

GeoArticles per Service x City:
[INSERT NUMBER]

GeoHub URL Style:
[INSERT]

GeoArticle URL Style:
[INSERT]

Generate rows for:

1. Homepage
2. Service Overview Pages
3. GeoHub Pages
4. Location-Based Service Pages
5. Additional Category Pages
6. GeoArticle Pages

Use these columns:

ID
Page Type
Parent Page
Service
Service Slug
City
City Slug
Additional Category
URL
H1
Meta Title
Schema Type
Priority
Publish Phase
Status
Notes

Rules:
- Homepage = /
- Service Overview = /category/service/
- Location-Based Service = /category/city/service/
- Additional Category = /category/city/service/
- GeoHub = /city/ or /category/city/
- GeoArticle = /city/article-topic/ or /category/city/article-topic/
- Do not create duplicate additional category pages if already covered by core services.
- Do not mix multiple services or cities.


# Prompt auxiliar 2 — Solo para generar contenidos por tipo de página


Actúa como Matteo de GMB Crush y como senior SEO content strategist.

Quiero generar contenido completo para esta página siguiendo GMB Crush, AIO, GEO y AUDIO.

Page Type:
[Homepage / Service Overview / Location-Based Service / Additional Category / GeoHub / GeoArticle]

Business Name:
[INSERT]

Primary GBP Category:
[INSERT]

Primary Category Slug:
[INSERT]

Service:
[INSERT]

Service Slug:
[INSERT]

City:
[INSERT]

City Slug:
[INSERT]

URL:
[INSERT]

Parent Service Page:
[INSERT]

GeoHub Page:
[INSERT]

Related Pages:
[INSERT]

Phone:
[INSERT]

Email:
[INSERT]

NAP:
[INSERT]

GBP URL:
[INSERT]

Physical office in this city?
Yes / No

Trust Signals:
[INSERT]

Preferred CTA:
[INSERT]

Generate:

1. H1
2. Meta title
3. Meta description
4. Quick Answer block if relevant
5. Full page outline
6. 3–5 H2s using AUDIO where applicable
7. 3–5 FAQs
8. CTA
9. Internal links with anchor text
10. Schema recommendation
11. Anti-canibalization note

Rules:
- If Service Overview, do not target a city.
- If Location-Based Service, use one service and one city.
- If Additional Category, support the additional GBP category with local relevance.
- If GeoHub, list all city services, categories and articles.
- If GeoArticle, write as semantic booster, not a landing page.
- Do not claim physical presence if false.


# Prompt auxiliar 3 — Solo para GeoArticles


Actúa como Matteo de GMB Crush, especialista en GeoArticles, AI Overview y semantic SEO local.

Quiero generar ideas de GeoArticle Pages para reforzar mis páginas de servicio local.

Inputs:

Primary Business Category Slug:
[INSERT]

Website Root Domain:
[INSERT]

Brand Name:
[INSERT]

Service:
[INSERT]

Service Slug:
[INSERT]

City:
[INSERT]

City Slug:
[INSERT]

Matching Location-Based Service Page:
[INSERT]

Matching GeoHub Page:
[INSERT]

Target Audience:
[INSERT]

Physical office in this city?
Yes / No

Generate 3 GeoArticle ideas.

For each idea, return:

1. Page Title
2. H1 Suggestion
3. Suggested URL
4. Target Long-Tail Keyword
5. Intent Type
6. 1–2 Sentence Summary
7. Matching Location-Based Service Page
8. Matching GeoHub Page
9. Related GeoArticle idea
10. Suggested CTA
11. Schema Type

Rules:
- Each article must support one service, one city and one long-tail intent.
- Each article must link to the matching /category/city/service/ page.
- Each article must link to the matching /city/ GeoHub page.
- Avoid pretending the business is physically located in the city unless true.
- GeoArticles are not landing pages.


# Prompt auxiliar 4 — Solo para auditoría QA


Actúa como Matteo de GMB Crush y haz QA de esta página antes de publicarla.

Page URL:
[INSERT]

Page Type:
[INSERT]

Business Name:
[INSERT]

Primary GBP Category:
[INSERT]

Target Service:
[INSERT]

Target City:
[INSERT]

Physical office in this city?
Yes / No

H1:
[INSERT]

Meta Title:
[INSERT]

Meta Description:
[INSERT]

Word Count:
[INSERT]

Schema Added:
[INSERT]

Internal Links Added:
[INSERT]

NAP Used:
[INSERT]

Check this page against the GMB Crush QA system:

1. URL approved
2. Page type correct
3. One service only
4. One city only if applicable
5. H1 approved
6. Meta title approved
7. Meta description approved
8. Word count approved
9. AUDIO structure included
10. FAQs included
11. CTA included
12. Schema approved
13. Internal links approved
14. NAP consistent
15. No canibalization
16. No false location claim
17. Final approval

Return:
- QA table
- Problems found
- Required fixes
- Final status: Approved / Needs Revision / Blocked


# Reglas no negociables


| Regla | Explicación |
| --- | --- |
| Homepage = entidad raíz | Debe establecer marca, servicio principal, ciudad principal, NAP y enlaces core. |
| Service Overview ≠ Service in City | Una página de servicio general no debe intentar ser una página local. |
| Una ciudad por landing local | No mezclar Miami, Hialeah y Coral Gables en una misma landing. |
| Un servicio por landing local | No mezclar emergency, car y residential en una misma página comercial. |
| Cada categoría GBP debe tener soporte | Primary y additional categories deben tener páginas relevantes. |
| GeoHub = contenedor de ciudad | Debe listar servicios, categorías y artículos de una ciudad. |
| GeoArticle = booster | Debe apoyar una landing, no competir con ella. |
| No ubicación falsa | No decir “oficina en X” si no existe. |
| Internal links obligatorios | Cada página debe tener padre, hijo o destino claro. |
| QA antes de publicar | Ninguna página se publica sin revisar URL, H1, schema, links, NAP y canibalización. |


## Resultado final del Paso 11


Master Prompt reutilizable
Prompt rellenado con ABC Locksmith
Prompt auxiliar para URL Matrix
Prompt auxiliar para contenidos
Prompt auxiliar para GeoArticles
Prompt auxiliar para QA
Reglas no negociables del sistema


# Paso 12 — Sistema final operativo


## Objetivo del Paso 12


Ahora unimos todo en un SOP final para construir cualquier web local desde cero siguiendo GMB Crush.

Este sistema convierte una web local en una máquina organizada de:

Entidad
Servicios
Ciudades
Categorías GBP
GeoHubs
GeoArticles
Enlaces internos
Schema
Prioridad
QA
Publicación
Tracking
Optimización

La estructura final se basa en la jerarquía GMB Crush:

Homepage
Service Overview Pages
Location-Based Service Pages
Additional Category Pages
GeoHub Pages
GeoArticle Pages

Cada tipo de página tiene una función concreta dentro del sistema de Local SEO, GBP support, AI Overview y autoridad semántica.


## Lo que tienes que rellenar


Business Name:

Website Root Domain:

Canonical Domain:

Country:

State / Province:

Main City:

Physical Location City:

Full NAP:
- Business Name:
- Street Address:
- City:
- State / Province:
- ZIP / Postal Code:
- Country:
- Phone:

GBP URL:

Primary GBP Category:

Additional GBP Categories:
1.
2.
3.

Core Services:
1.
2.
3.
4.
5.

Target Cities:
1.
2.
3.
4.
5.

Services available in every city?
Yes / No

Additional Categories already covered by core services:
1.
2.

Additional Categories that need separate pages:
1.
2.

GeoArticles per Service x City:

GeoHub URL Style:
/city/ or /category/city/

GeoArticle URL Style:
/city/article-topic/ or /category/city/article-topic/

Top Priority Services:
1.
2.
3.

Top Priority Cities:
1.
2.
3.

Trust Signals:
- Years in business:
- Reviews:
- Certifications:
- Awards:
- Guarantees:
- Emergency / same-day / mobile service:

Preferred CTA:

Publishing Capacity:
Pages per week:

CMS:

Can schema be added?
Yes / No

Can internal links be edited manually?
Yes / No

Tracking Tools:
GMB Crush / GSC / GA4 / Rank Tracker / Other


## Ejemplo rellenado


Business Name:
ABC Locksmith

Website Root Domain:
https://www.abclocksmith.com

Canonical Domain:
https://www.abclocksmith.com

Country:
United States

State / Province:
Florida

Main City:
Miami

Physical Location City:
Miami

Full NAP:
- Business Name: ABC Locksmith
- Street Address: 123 Main St
- City: Miami
- State / Province: FL
- ZIP / Postal Code: 33101
- Country: United States
- Phone: +1 305 000 0000

GBP URL:
https://google.com/business/abc-locksmith

Primary GBP Category:
Locksmith

Additional GBP Categories:
1. Emergency Locksmith Service
2. Key Duplication Service

Core Services:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying

Target Cities:
1. Miami
2. Hialeah
3. Coral Gables
4. Doral
5. Hollywood

Services available in every city?
Yes

Additional Categories already covered by core services:
1. Emergency Locksmith Service

Additional Categories that need separate pages:
1. Key Duplication Service

GeoArticles per Service x City:
3

GeoHub URL Style:
/city/

GeoArticle URL Style:
/city/article-topic/

Top Priority Services:
1. Emergency Locksmith
2. Car Locksmith
3. Commercial Locksmith

Top Priority Cities:
1. Miami
2. Hialeah
3. Coral Gables

Trust Signals:
- 10+ years in business
- 250+ Google reviews
- Licensed locksmith technicians
- Local service award
- Workmanship guarantee
- Same-day mobile support

Preferred CTA:
Call now

Publishing Capacity:
5 pages per week

CMS:
WordPress

Can schema be added?
Yes

Can internal links be edited manually?
Yes

Tracking Tools:
GMB Crush Geo Grid, Google Search Console, GA4


## El sistema final en una frase


Rellenas los inputs → generas arquitectura → creas matriz URL → aplicas reglas de página → enlazas → priorizas → produces → haces QA → publicas → mides → optimizas.

O más operativo:

Input → Architecture → URL Matrix → Page Briefs → Internal Links → Schema → Priority → QA → Publish → Track → Optimize


# 1. Intake System


## Qué hace


Recoge los datos base del negocio.

Sin esto no se puede generar una arquitectura fiable.


## Output


Business entity definida
Primary GBP Category definida
Additional GBP Categories definidas
Servicios definidos
Ciudades definidas
NAP definido
Ubicación física validada
Áreas de servicio validadas


## Regla


No se crea ninguna página antes de validar categoría GBP, servicios y ciudades.


# 2. Architecture Formula System


## Qué hace


Calcula cuántas páginas necesita la web.


## Fórmula


1 Homepage
+ S Service Overview Pages
+ C GeoHub Pages
+ S × C Location-Based Service Pages
+ A × C Additional Category Pages
+ G × S × C GeoArticle Pages

Donde:

S = servicios principales
C = ciudades objetivo
A = categorías adicionales que necesitan página propia
G = GeoArticles por servicio x ciudad


## Ejemplo ABC Locksmith


1 Homepage
+ 5 Service Overview Pages
+ 5 GeoHub Pages
+ 25 Location-Based Service Pages
+ 5 Additional Category Pages
+ 75 GeoArticle Pages
= 111 páginas estratégicas


## Regla


El número total de páginas se calcula antes de producir contenido.


# 3. URL Matrix System


## Qué hace


Convierte la arquitectura en una matriz operativa.


## Columnas obligatorias


ID
Page Type
Parent Page
Service
Service Slug
City
City Slug
Additional Category
URL
H1
Meta Title
Meta Description
Schema Type
Internal Links Required
Priority
Publish Phase
Status
Notes


## Ejemplo


| ID | Page Type | URL | Priority | Phase |
| --- | --- | --- | --- | --- |
| HP-001 | Homepage | / | P1 | Phase 1 |
| SO-001 | Service Overview | /locksmith/emergency-locksmith/ | P1 | Phase 1 |
| GH-001 | GeoHub | /miami/ | P1 | Phase 1 |
| LBS-001 | Location-Based Service | /locksmith/miami/emergency-locksmith/ | P1 | Phase 2 |
| GA-001 | GeoArticle | /miami/emergency-locksmith-cost-guide/ | P3 | Phase 3 |


## Regla


Cada página debe tener una fila, un tipo, una URL, una función y una fase.


# 4. URL Rules System


## Qué hace


Evita URLs caóticas, duplicadas o canibalizadas.


## Patrones aprobados


Homepage:
/

Service Overview:
/category/service/

Location-Based Service:
/category/city/service/

Additional Category:
/category/city/service/

GeoHub:
/city/

GeoArticle:
/city/article-topic/


## Ejemplo ABC Locksmith


/
/locksmith/emergency-locksmith/
/locksmith/miami/emergency-locksmith/
/locksmith/miami/key-duplication/
/miami/
/miami/emergency-locksmith-cost-guide/


## Regla


Una URL = una intención = un servicio o una ciudad principal.


# 5. Page Type System


## Qué hace


Define qué debe contener cada tipo de página.


| Page Type | Función | Word Count |
| --- | --- | --- |
| Homepage | Root Entity Anchor | 900–1.300 |
| Service Overview | Topical Authority Pillar | 850–1.000 |
| Location-Based Service | Local Converter | 800–1.000 |
| Additional Category | GBP Category Support | 800–1.000 |
| GeoHub | City Silo Container | 700–1.100 |
| GeoArticle | Semantic Booster | 1.000–1.500 |


## Regla


No todos los tipos de página se escriben igual.


# 6. Homepage Operating Rules


## Debe incluir


H1 con marca + servicio principal + ciudad
Intro con brand + service + main city
Quick Answer
Mini service menu
Trust blocks
NAP
CTA
Internal links
FAQPage + Speakable schema
Organization + WebSite schema


## Ejemplo


H1:
ABC Locksmith – Trusted Locksmith Services in Miami, FL

Meta Title:
Top-Rated Locksmith in Miami, FL | ABC Locksmith


## Enlaces obligatorios


/locksmith/emergency-locksmith/
/locksmith/car-locksmith/
/locksmith/commercial-locksmith/
/miami/
/locksmith/miami/key-duplication/
/contact/


## Regla


La homepage es la raíz de la entidad, no una página decorativa.


# 7. Service Overview Operating Rules


## Debe incluir


H1 con servicio
Sin ciudad como target principal
Intro 100–150 palabras
AUDIO sections
3–5 FAQs
CTA
Enlaces a versiones ciudad + servicio
Service + WebPage schema


## Ejemplo


URL:
/locksmith/emergency-locksmith/

H1:
Professional Emergency Locksmith Services by ABC Locksmith

Links to:
/locksmith/miami/emergency-locksmith/
/locksmith/hialeah/emergency-locksmith/
/locksmith/coral-gables/emergency-locksmith/


## Regla


La página de servicio general no debe intentar ser una página local.


# 8. Location-Based Service Operating Rules


## Debe incluir


Servicio + ciudad
Intro local
AUDIO sections
FAQs locales
CTA local
Enlaces al servicio padre
Enlaces al GeoHub
Enlaces a servicios relacionados
Enlaces a GeoArticles
LocalBusiness schema


## Ejemplo


URL:
/locksmith/miami/emergency-locksmith/

H1:
ABC Locksmith – Emergency Locksmith in Miami

Parent Service:
/locksmith/emergency-locksmith/

GeoHub:
/miami/


## Regla


Estas son las páginas comerciales más importantes para búsquedas “service in city”.


# 9. Additional Category Operating Rules


## Debe incluir


Categoría GBP adicional
Ciudad
Intro con problema local
AUDIO sections
FAQs
CTA
Enlaces al GeoHub
Enlaces a servicios relacionados
Service schema con areaServed


## Ejemplo


URL:
/locksmith/miami/key-duplication/

H1:
ABC Locksmith – Expert Key Duplication in Miami


## Regla


Solo se crean si la categoría adicional no está ya cubierta por un servicio principal.


# 10. GeoHub Operating Rules


## Debe incluir


Una ciudad
Todos los servicios de esa ciudad
Categorías adicionales de esa ciudad
GeoArticles de esa ciudad
Trust signals
CTA
Enlaces a homepage y contacto
CollectionPage schema


## Ejemplo


URL:
/miami/

H1:
ABC Locksmith – Locksmith Services in Miami


## Debe enlazar a


/locksmith/miami/emergency-locksmith/
/locksmith/miami/car-locksmith/
/locksmith/miami/commercial-locksmith/
/locksmith/miami/key-duplication/
/miami/emergency-locksmith-cost-guide/
/contact/


## Regla


El GeoHub es el índice de ciudad.


# 11. GeoArticle Operating Rules


## Debe incluir


Un servicio
Una ciudad
Una intención long-tail
1.000–1.500 palabras
3–5 H2
3–5 FAQs
CTA contextual
Enlace a página servicio + ciudad
Enlace al GeoHub
Enlace a otro GeoArticle
Article + FAQPage + Breadcrumb + Speakable schema


## Ejemplo


URL:
/miami/emergency-locksmith-cost-guide/

Supports:
/locksmith/miami/emergency-locksmith/

GeoHub:
/miami/


## Regla


GeoArticle = booster semántico, no landing page.


# 12. Internal Linking Operating System


## Jerarquía final


Homepage
→ Service Overview Pages
→ Main GeoHub
→ Main Additional Category Pages

Service Overview
→ Homepage
→ City-specific versions
→ Related services
→ GeoArticles

Location-Based Service
→ Parent Service Overview
→ Matching GeoHub
→ Same-city services
→ Nearby city versions
→ GeoArticles
→ Contact

Additional Category
→ Matching GeoHub
→ Related services
→ Related GeoArticles
→ Contact

GeoHub
→ Homepage
→ All city services
→ All city additional categories
→ All city GeoArticles
→ Contact

GeoArticle
→ Matching Location-Based Service
→ Matching GeoHub
→ Related GeoArticle
→ Contact


## Regla


Cada página debe enlazar hacia arriba, hacia abajo y lateralmente.


# 13. Priority Operating System


## Fórmula


Priority Score =
Revenue Value
+ Search Intent
+ GBP Category Relevance
+ City Priority
+ Competition Gap
+ Conversion Urgency


## Tiers


| Score | Prioridad |
| --- | --- |
| 26–30 | P1 |
| 21–25 | P2 |
| 16–20 | P3 |
| 10–15 | P4 |
| 0–9 | Hold |


## Ejemplo


/locksmith/miami/emergency-locksmith/

Revenue Value: 5
Search Intent: 5
GBP Category Relevance: 5
City Priority: 5
Competition Gap: 4
Conversion Urgency: 5

Total Score: 29
Priority: P1


## Regla


Primero páginas comerciales de alta intención. Después artículos.


# 14. Publishing Operating System


## Fase 1 — Entity Foundation


Homepage
Contact
About
Top Service Overview Pages
Main GeoHub
Schema base
NAP
Trust blocks


## Fase 2 — Local Conversion Layer


Main city + service pages
Additional category pages
Secondary GeoHubs
High-intent service pages in secondary cities


## Fase 3 — Semantic Expansion Layer


GeoArticles
FAQ clusters
Cost guides
Comparison articles
Mistake guides
How-to articles


## Fase 4 — Optimization Loop


Geo-grid tracking
Search Console review
Internal link updates
Schema QA
FAQ expansion
Metadata refresh
Content refresh


## Regla


No publicar GeoArticles antes de publicar la landing servicio + ciudad que deben apoyar.


# 15. QA Operating System


## Checklist final


URL approved
Page type correct
One service only
One city only
H1 approved
Meta title approved
Meta description approved
Word count approved
AUDIO structure included
FAQs included
CTA included
Schema approved
Internal links approved
NAP consistent
No canibalization
No false location claim
Final approval


## Regla


Ninguna página se publica sin pasar QA.


# 16. Tracking Operating System


## Qué medir


Geo-grid rankings
Local 3-Pack visibility
Organic rankings
Search Console impressions
CTR
Clicks
Calls
Form submissions
GBP interactions
Pages stuck on page 2
Pages with impressions but no clicks


## Qué hacer con los datos


| Problema | Acción |
| --- | --- |
| Página con impresiones pero bajo CTR | Mejorar meta title y meta description |
| Página local sin ranking | Añadir GeoArticles y enlaces internos |
| Servicio importante sin visibilidad | Reforzar Service Overview + páginas ciudad |
| Ciudad débil | Crear o mejorar GeoHub |
| Página con tráfico pero sin leads | Mejorar CTA, trust blocks y UX |
| Artículo sin impacto | Enlazarlo mejor o refrescar contenido |
| GBP category sin soporte | Crear Additional Category Page |


## Regla


Publicar no es el final. El sistema se optimiza con datos.


# Sistema final en formato SOP


1. Recoger inputs del negocio
2. Validar GBP category, servicios y ciudades
3. Detectar categorías adicionales duplicadas
4. Calcular número total de páginas
5. Crear URL Matrix
6. Aplicar reglas de URL
7. Asignar page type a cada URL
8. Crear brief por tipo de página
9. Asignar schema por tipo de página
10. Crear mapa de enlaces internos
11. Calcular Priority Score
12. Asignar fase de publicación
13. Producir contenidos por lote
14. Pasar QA
15. Publicar
16. Revisar indexación
17. Medir geo-grid, GSC y conversiones
18. Optimizar páginas débiles
19. Crear nuevos GeoArticles
20. Refrescar contenido cada 3–6 meses


# Sistema final aplicado a ABC Locksmith


## Arquitectura total


Business:
ABC Locksmith

Primary GBP Category:
Locksmith

Main City:
Miami

Target Cities:
Miami, Hialeah, Coral Gables, Doral, Hollywood

Core Services:
Emergency Locksmith
Car Locksmith
Residential Locksmith
Commercial Locksmith
Lock Rekeying

Effective Additional Category:
Key Duplication Service

Total Pages:
111


## Primera publicación


/
/contact/

/locksmith/emergency-locksmith/
/locksmith/car-locksmith/
/locksmith/commercial-locksmith/

/miami/

/locksmith/miami/emergency-locksmith/
/locksmith/miami/car-locksmith/
/locksmith/miami/commercial-locksmith/


## Segunda publicación


/locksmith/residential-locksmith/
/locksmith/lock-rekeying/

/locksmith/miami/residential-locksmith/
/locksmith/miami/lock-rekeying/

/locksmith/miami/key-duplication/

/hialeah/
/coral-gables/

/locksmith/hialeah/emergency-locksmith/
/locksmith/coral-gables/emergency-locksmith/


## Tercera publicación


/miami/emergency-locksmith-cost-guide/
/miami/what-to-do-locked-out-of-house/
/miami/how-fast-can-locksmith-arrive/

/miami/car-locksmith-cost-guide/
/miami/what-to-do-locked-out-of-car/
/miami/car-key-replacement-guide/


# Carpetas o pestañas recomendadas


Si lo montas en Google Sheets, Airtable o Notion, usaría estas pestañas:

1. Inputs
2. Services
3. Cities
4. Additional Categories
5. URL Matrix
6. Page Briefs
7. Internal Linking Map
8. Schema Map
9. Priority Score
10. Publishing Plan
11. QA Checklist
12. Tracking Log
13. Optimization Queue


## Qué genera cada pestaña


| Pestaña | Función |
| --- | --- |
| Inputs | Datos base del negocio |
| Services | Servicios, slugs, prioridad, valor |
| Cities | Ciudades, slugs, prioridad, ubicación física |
| Additional Categories | Categorías GBP adicionales y duplicados |
| URL Matrix | Todas las páginas del sistema |
| Page Briefs | H1, metas, estructura, secciones |
| Internal Linking Map | Source URL, target URL, anchor, placement |
| Schema Map | Schema requerido por página |
| Priority Score | P1, P2, P3, P4 |
| Publishing Plan | Fase, semana, orden, estado |
| QA Checklist | Control antes de publicar |
| Tracking Log | Rankings, GSC, leads, geo-grid |
| Optimization Queue | Acciones pendientes |


# Output final que debe entregar el sistema


1. Arquitectura total
2. Número total de páginas
3. URL Matrix completa
4. Brief de homepage
5. Briefs de Service Overview Pages
6. Briefs de Location-Based Service Pages
7. Briefs de Additional Category Pages
8. Briefs de GeoHub Pages
9. Ideas de GeoArticles
10. Schema Map
11. Internal Linking Map
12. Priority Score
13. Publishing Plan
14. QA Checklist
15. Tracking Plan
16. Optimization Queue


# Reglas finales no negociables


No crear páginas sin función clara.
No mezclar servicios en una landing local.
No mezclar ciudades en una landing local.
No crear categorías adicionales duplicadas.
No publicar artículos antes de sus páginas comerciales.
No fingir ubicación física.
No dejar páginas huérfanas.
No publicar sin schema.
No publicar sin CTA.
No publicar sin enlaces internos.
No publicar sin QA.
No dejar de medir después de publicar.


# El sistema completo resumido


Homepage = entidad raíz
Service Overview Pages = autoridad temática
Location-Based Service Pages = conversión local
Additional Category Pages = soporte GBP
GeoHub Pages = contenedores de ciudad
GeoArticle Pages = boosters semánticos
Internal Linking = distribución de autoridad
Schema = claridad para Google y AI
Priority Score = orden de ejecución
QA = control de calidad
Tracking = mejora continua


# Paso 12 completado


La estructura final queda así:

1. Intake Form
2. Fórmula maestra de arquitectura
3. Matriz base
4. URL Rules
5. Page Type Rules
6. Internal Linking Rules
7. Priority Score
8. QA Checklist
9. Producción en fases
10. Pseudocódigo del sistema
11. Master Prompt reutilizable
12. Sistema final operativo

Este es el workflow completo para construir una web local desde cero con metodología GMB Crush, preparada para GBP support, Local 3-Pack, orgánico, AI Overview y escalado por ciudad/servicio.