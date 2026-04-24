**GMB Crush — Paso 04: URL Rules**
Versión literal del chat · Sistema GMB Crush para webs locales

Documento generado a partir de la conversación paso a paso sobre el sistema GMB Crush para construir una web local desde cero.


# Índice

**1. Paso 04 — URL Rules**


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