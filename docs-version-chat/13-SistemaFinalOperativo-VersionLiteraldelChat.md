**GMB Crush — Paso 13: Sistema Final Operativo**
Versión literal del chat · Sistema GMB Crush para webs locales

Documento generado a partir de la conversación paso a paso sobre el sistema GMB Crush para construir una web local desde cero.


# Índice

**1. Paso 13 — Sistema Final Operativo**


# Paso 13 — Sistema final operativo


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