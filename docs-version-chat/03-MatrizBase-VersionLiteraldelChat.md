**GMB Crush — Paso 03: Matriz Base**
Versión literal del chat · Sistema GMB Crush para webs locales

Documento generado a partir de la conversación paso a paso sobre el sistema GMB Crush para construir una web local desde cero.


# Índice

**1. Paso 03 — Matriz Base**


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