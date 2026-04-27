# Reglas más relevantes del sistema GMB Crush

Documento de referencia rápida para mantener estable el sistema GMB Crush de webs locales.

Sistema actual:

```text
Web-first
GBP después
14 pasos
Main City = base de arquitectura
Local Coverage Areas = señales GEO, no URLs por defecto
Approved Expansion Areas = URLs solo si se aprueban
```

---

# 1. Regla de dirección física

La dirección física es el ancla inicial del sistema.

A partir de una dirección como:

```text
Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí, Madrid
```

el sistema debe hacer esto:

```text
1. Fijar NAP.
2. Extraer Main City.
3. Construir la arquitectura sobre la ciudad.
4. Usar barrios, zonas o landmarks como señales GEO dentro del contenido.
5. No crear páginas por calle, barrio o distrito automáticamente.
```

## Regla final

```text
La dirección física fija el NAP y la Main City; no crea URLs por barrio automáticamente.
```

---

# 2. Regla de Main City

La arquitectura base se construye sobre una sola ciudad principal.

En el ejemplo:

```text
Main City = Madrid
```

La Main City genera:

```text
/madrid/
/cerrajero/madrid/cerrajero-urgente/
/cerrajero/madrid/apertura-puertas/
/madrid/cuanto-cuesta-un-cerrajero-urgente/
```

## Regla final

```text
La Main City crea la arquitectura base.
```

---

# 3. Regla de Local Coverage Areas

Se mantiene el término:

```text
Local Coverage Areas
```

No usar:

```text
Local Positioning Areas
```

Las Local Coverage Areas son zonas, barrios, distritos o landmarks seleccionados desde:

```text
dirección física
Main City
coherencia GEO
proximidad
datos de búsqueda
competidores
lógica GMB Crush
```

Sirven para reforzar contenido local, FAQs, GeoHub, GeoArticles y schema `areaServed`.

## Regla final

```text
Local Coverage Areas son señales GEO. No generan URLs por defecto.
```

---

# 4. Regla Direct / Candidate / Approved

Las Local Coverage Areas se dividen en tres niveles.

## Direct Local Coverage Areas

Zonas que salen directamente de la dirección física.

Ejemplo:

```text
Almagro
Chamberí
```

## Candidate Local Coverage Areas

Zonas que pueden tener sentido GEO, pero deben validarse.

Ejemplo:

```text
Salamanca
Retiro
Centro
Tetuán
Chamartín
Arganzuela
Moncloa
Prosperidad
```

## Approved Expansion Areas

Zonas que sí pueden generar URLs propias.

Ejemplo:

```text
None in Phase 1
```

## Regla final

```text
Direct = sale del NAP.
Candidate = se evalúa.
Approved Expansion = puede generar URL.
```

---

# 5. Regla del test de coherencia GEO

Una Candidate Local Coverage Area puede usarse como señal GEO activa si cumple al menos 3 de estos criterios:

| Criterio | Pregunta |
|---|---|
| Ancla física | ¿Sale directamente o está conectada a la dirección? |
| Main City | ¿Pertenece claramente a la Main City? |
| Proximidad | ¿Está cerca o conectada al punto físico? |
| Intención local | ¿Ayuda a explicar una necesidad local real del servicio? |
| Demanda o competencia | ¿Hay búsquedas o competidores trabajando esa zona? |
| No falsa ubicación | ¿Puede mencionarse sin afirmar oficina física allí? |

## Regla final

```text
Una zona no entra por relleno; entra porque tiene coherencia GEO.
```

---

# 6. Regla de no URLs para Local Coverage Areas

No crear URLs para zonas, barrios o distritos salvo que estén aprobados como Approved Expansion Areas.

## Correcto

```text
/cerrajero/madrid/cerrajero-urgente/
```

Dentro del contenido se pueden mencionar:

```text
Almagro
Chamberí
Salamanca
Retiro
```

## Incorrecto

```text
/almagro/
/chamberi/
/cerrajero/almagro/cerrajero-urgente/
```

si esas zonas no están aprobadas como expansión.

## Regla final

```text
Mencionar una zona no significa crear una página para esa zona.
```

---

# 7. Regla de fórmula base

La fórmula base del sistema es:

```text
1 Homepage
+ S Service Overview Pages
+ 1 Main City GeoHub
+ S Main City Location-Based Service Pages
+ A Main City Additional Category Pages
+ G × S Main City GeoArticles
```

En el ejemplo:

```text
S = 5 servicios
A = 1 categoría adicional efectiva
G = 3 GeoArticles por servicio
```

Resultado:

```text
1 + 5 + 1 + 5 + 1 + 15 = 28 páginas SEO base
```

`/contacto/` es página auxiliar, no parte del inventario SEO base.

## Regla final

```text
El inventario SEO base son 28 páginas; /contacto/ es auxiliar.
```

---

# 8. Regla de tipos de página

El sistema usa estos seis tipos principales:

```text
Homepage
Service Overview Pages
Location-Based Service Pages
Additional Category Pages
GeoHub Pages
GeoArticle Pages
```

## Regla final

```text
Cada página debe tener un tipo, una función, una URL, un schema, enlaces internos y una fase.
```

---

# 9. Regla de Homepage

La homepage es la raíz de entidad.

Debe establecer:

```text
quién es la marca
qué hace
dónde opera
servicios principales
NAP
CTA
trust blocks
enlaces internos
```

Patrón:

```text
/
```

H1 recomendado:

```text
[Brand] + [Primary Service] + [Main City]
```

## Regla final

```text
La homepage no es una landing genérica; es el ancla de entidad.
```

---

# 10. Regla de Service Overview Pages

Las Service Overview Pages son páginas de servicio sin ciudad.

Patrón:

```text
/cerrajero/cerrajero-urgente/
/cerrajero/apertura-puertas/
```

No deben orientarse a Madrid como target principal.

## Regla final

```text
Service Overview = servicio sin ciudad.
```

---

# 11. Regla de Location-Based Service Pages

Las LBS son páginas comerciales servicio + ciudad.

Patrón:

```text
/cerrajero/madrid/cerrajero-urgente/
/cerrajero/madrid/apertura-puertas/
```

Deben tener:

```text
servicio + ciudad
intro local
H2s AUDIO
FAQs
CTA
LocalBusiness schema
enlaces a Service Overview
enlaces a GeoHub
enlaces a GeoArticles
```

## Regla final

```text
Location-Based Service = un servicio + una ciudad.
```

---

# 12. Regla de Additional Category Pages

Las Additional Category Pages soportan categorías adicionales del futuro GBP.

Ejemplo:

```text
Servicio de duplicado de llaves
```

URL:

```text
/cerrajero/madrid/duplicado-llaves/
```

No convertir automáticamente en core service.

## Regla final

```text
Duplicado de llaves es Additional Category Page, no core service de la fórmula base.
```

---

# 13. Regla de GeoHub

El GeoHub es el contenedor de ciudad.

Patrón:

```text
/madrid/
```

Debe agrupar:

```text
servicios de Madrid
categoría adicional
GeoArticles
Local Coverage Areas
enlaces internos
CTA
```

## Regla final

```text
GeoHub = índice de ciudad.
```

---

# 14. Regla de GeoArticles

Los GeoArticles son boosters semánticos, no landings.

Cada GeoArticle debe tener:

```text
un servicio
una ciudad
una intención long-tail
enlace a su LBS
enlace al GeoHub
schema Article / FAQPage / Breadcrumb / Speakable
```

En el sistema actual:

```text
5 servicios × 3 artículos = 15 GeoArticles
```

## Regla final

```text
GeoArticle = servicio + ciudad + intención long-tail.
```

---

# 15. Regla de una intención por URL

No crear dos URLs para la misma intención.

## Correcto

```text
/madrid/cuanto-cuesta-un-cerrajero-urgente/
```

## Incorrecto

```text
/madrid/guia-precios-cerrajero-urgente/
/madrid/cuanto-cuesta-un-cerrajero-urgente/
```

si ambas atacan la misma intención.

## Regla final

```text
Una intención long-tail debe tener una sola URL.
```

---

# 16. Regla de contacto

La URL canónica de contacto es:

```text
/contacto/
```

No usar:

```text
/contact/
```

Si `/contact/` existe, debe redirigir a `/contacto/`.

## Regla final

```text
/contacto/ es la única URL de contacto.
```

---

# 17. Regla de GBP web-first

El GBP no existe al inicio.

Estado inicial:

```text
GBP Status = Not Created
GBP URL = N/A
GBP Verification Status = Not Started
```

La web se construye primero.

El GBP se crea después, en el Paso 14.

## Regla final

```text
Primero web; después GBP.
```

---

# 18. Regla de categorías GBP planificadas

Mientras no exista el GBP, se trabaja con categorías planificadas.

Ejemplo:

```text
Planned Primary GBP Category:
Cerrajero

Planned Additional GBP Categories:
Servicio de cerrajería de urgencia
Servicio de duplicado de llaves
```

## Regla final

```text
Antes del GBP usamos categorías planificadas; después del GBP se confirman.
```

---

# 19. Regla de no categorías GBP sin soporte

No añadir una categoría adicional al GBP si la web no la soporta.

## Correcto

```text
Servicio de duplicado de llaves
→ /cerrajero/madrid/duplicado-llaves/
```

## Incorrecto

```text
Proveedor de sistemas de seguridad
```

si no existe página, servicio real o soporte web.

## Regla final

```text
Cada categoría adicional confirmada debe tener soporte web real.
```

---

# 20. Regla de no inventar GBP URL

No usar `sameAs` con GBP hasta que exista el perfil.

Antes del Paso 14:

```text
GBP URL = N/A
sameAs GBP = no usar
```

Después del Paso 14:

```text
Añadir GBP URL real
Actualizar sameAs
Actualizar schema
Actualizar página de contacto
Actualizar homepage
```

## Regla final

```text
No se inventa GBP URL.
```

---

# 21. Regla de no inventar reseñas

Si el GBP no existe, no se pueden declarar reseñas de Google.

## Correcto

```text
Reseñas iniciales pendientes tras crear y verificar el GBP.
```

## Incorrecto

```text
250+ reseñas
5 estrellas en Google
```

si todavía no existen.

## Regla final

```text
No se inventan reseñas, estrellas ni social proof de Google.
```

---

# 22. Regla de internal linking

Cada página debe enlazar según su función.

## Jerarquía base

```text
Homepage → Service Overview + GeoHub + Contacto
Service Overview → LBS + servicios relacionados
LBS → Service Overview + GeoHub + GeoArticles
GeoHub → todas las páginas de Madrid
GeoArticle → LBS + GeoHub + artículo relacionado
Additional Category → GeoHub + servicios relacionados
```

## Regla final

```text
No debe haber páginas huérfanas.
```

---

# 23. Regla de no enlaces a URLs inexistentes

No enlazar Local Coverage Areas si no tienen URL aprobada.

## Incorrecto

```text
Enlace a /almagro/
```

si `/almagro/` no existe.

## Correcto

```text
Mencionar Almagro en el texto sin enlazar.
```

## Regla final

```text
Solo se enlaza a URLs reales y aprobadas.
```

---

# 24. Regla de schema

El schema debe ajustarse al tipo de página.

## Base

```text
Homepage:
Organization + WebSite

Service Overview:
Service + WebPage + BreadcrumbList

Location-Based Service:
LocalBusiness + BreadcrumbList + FAQPage

Additional Category:
Service + BreadcrumbList

GeoHub:
CollectionPage + BreadcrumbList

GeoArticle:
Article + FAQPage + BreadcrumbList + Speakable
```

## Regla final

```text
Schema por tipo de página, no schema genérico para todo.
```

---

# 25. Regla de areaServed

`areaServed` debe reflejar cobertura real o validada.

Puede incluir:

```text
Madrid
zonas validadas
Local Coverage Areas activas
```

No debe incluir zonas decorativas, inventadas o no validadas.

## Regla final

```text
Contenido puede usar señales GEO; areaServed solo debe usar cobertura real o validada.
```

---

# 26. Regla de prioridad

Cada URL SEO del inventario base debe tener prioridad.

La fórmula usa:

```text
Revenue Value
Search Intent
GBP Category Relevance
Local Relevance
Competition Gap
Conversion Urgency
```

El ejemplo canónico:

```text
/cerrajero/madrid/cerrajero-urgente/
Score: 29
Priority: P1
```

## Regla final

```text
Cada URL SEO debe tener score y prioridad.
```

---

# 27. Regla de QA

Ninguna URL se publica sin QA.

QA mínimo:

```text
URL correcta
Page type correcto
H1 correcto
Metadata correcta
Schema correcto
Internal links correctos
NAP consistente
CTA presente
No falsa ubicación
No canibalización
```

## Regla final

```text
No publicar sin QA.
```

---

# 28. Regla de producción por fases

La publicación se hace por fases:

```text
Phase 1: Entity Foundation
Phase 2: Main City Conversion Layer
Phase 3: Semantic Expansion
Phase 4: Optimization Loop
Phase 5: Optional Expansion Module
Phase 14: GBP Creation & Website Alignment
```

## Regla final

```text
No publicar GeoArticles antes de tener sus páginas padre.
```

---

# 29. Regla de Approved Expansion Areas

Las Approved Expansion Areas son la única vía para crear URLs fuera de la Main City.

Ejemplo:

```text
Approved Expansion Areas:
None in Phase 1
```

Si una zona se aprueba, puede generar:

```text
/area/
/cerrajero/area/service/
/area/article-topic/
```

## Regla final

```text
Sin aprobación, no hay URL de zona.
```

---

# 30. Regla de GBP Creation & Website Alignment

El Paso 14 convierte el plan web en GBP real.

Debe confirmar:

```text
NAP
modelo de negocio
categoría principal
categorías adicionales
servicios del GBP
URL web
URL de contacto
horarios
fotos
Q&A
posts
reseñas reales
UTM
schema updates
```

## Regla final

```text
El Paso 14 termina cuando web, GBP, schema y tracking están sincronizados.
```

---

# 31. Regla de base estable

No rehacer el sistema desde cero si solo hay inconsistencias editoriales.

Base estable:

```text
14 pasos
web-first
GBP después
Main City = Madrid
Local Coverage Areas
28 páginas SEO base
/contacto/
Duplicado de llaves como Additional Category Page
15 GeoArticles
```

## Regla final

```text
Corregir inconsistencias puntuales; no rediseñar la arquitectura sin motivo.
```
