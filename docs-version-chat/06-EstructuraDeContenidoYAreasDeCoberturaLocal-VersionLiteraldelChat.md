# Paso 6 — Estructura de Contenido + Áreas de Cobertura Local

**Nombre recomendado del archivo:** `06_Estructura_De_Contenido_Y_Areas_De_Cobertura_Local.md`  
**Dónde va:** después del **Paso 5 — Page Type Rules** y antes del nuevo **Paso 7 — Internal Linking Rules**.  
**Objetivo:** simplificar la arquitectura local base y definir cómo estructurar el contenido real de cada tipo de página usando una sola ciudad principal y áreas de cobertura local.

---

## 0. Por qué existe este paso

En el sistema original hablábamos de:

```text
Target Cities
Secondary Cities
Neighborhoods / Districts
Service Areas
```

Para una implementación base de SEO local, estos términos pueden generar confusión porque mezclan conceptos distintos:

- ciudades principales,
- municipios cercanos,
- barrios,
- distritos,
- zonas donde se presta servicio,
- zonas que podrían tener página propia en el futuro.

Este paso simplifica todo con tres conceptos operativos:

```text
Main City
Local Coverage Areas
Approved Expansion Areas
```

La arquitectura base se construye sobre una sola **Main City**.  
Las **Local Coverage Areas** se usan dentro del contenido para reforzar contexto local y cobertura real.  
Las **Approved Expansion Areas** solo generan páginas propias si se aprueban como expansión posterior.

---

## 1. Principio base

```text
Main City = ciudad principal que genera la arquitectura base.
Local Coverage Areas = zonas reales donde el negocio atiende clientes y que se mencionan dentro del contenido.
Approved Expansion Areas = zonas que sí tendrán URLs propias, solo si se aprueban después.
```

Regla principal:

```text
La Main City crea la arquitectura.
Las Local Coverage Areas enriquecen el contenido.
Las Local Coverage Areas no generan páginas propias por defecto.
Solo las Approved Expansion Areas generan URLs propias.
```

Esto mantiene el sistema limpio, evita páginas innecesarias y reduce el riesgo de canibalización, thin content o falsas señales de ubicación.

---

## 2. Terminología final

| Término | Qué significa | ¿Genera páginas en la base? |
|---|---|---|
| Main City | Ciudad principal de la arquitectura local. Es la ciudad que aparece en la homepage, GeoHub principal y páginas servicio + ciudad. | Sí |
| Local Coverage Areas | Zonas reales donde el negocio atiende clientes. Pueden ser barrios, distritos, municipios cercanos, códigos postales, urbanizaciones o zonas de servicio. | No por defecto |
| Approved Expansion Areas | Zonas de cobertura aprobadas para tener URLs propias. Se usan solo cuando hay demanda, competencia, valor comercial o justificación estratégica. | Sí, solo en módulo de expansión |

---

## 3. Qué eliminamos de la versión base

En la versión base del sistema ya no usamos estos conceptos como inputs principales:

```text
Target Cities
Secondary Cities
Top Priority Cities
Neighborhoods / Districts como bloque separado
Service Areas como bloque separado
```

En su lugar usamos:

```text
Main City
Local Coverage Areas
Approved Expansion Areas
```

Esto no significa que no podamos trabajar otras ciudades o zonas. Significa que no las metemos automáticamente en la arquitectura base.

---

## 4. Input inicial corregido

Este bloque debe añadirse o sustituir la parte geográfica del **Paso 1 — Intake Form**.

### Lo que tienes que rellenar

```text
Business Name:

Website URL:

Full NAP:
- Name:
- Address:
- Phone:

Primary GBP Category:

Additional GBP Categories:

Main City:
The primary city that will generate the base architecture.

Physical Location City:
The city where the business is physically located, if applicable.

Core Services:
1.
2.
3.
4.
5.

Local Coverage Areas:
Real areas where the business serves customers.
These can be neighborhoods, districts, municipalities, nearby towns, ZIP codes, urbanizations, or service zones.

Primary Local Coverage Areas:
Recommended: start with 3–5 strongest areas to mention most often.
1.
2.
3.
4.
5.

Additional Local Coverage Areas:
Optional.
1.
2.
3.
4.
5.

Should Local Coverage Areas generate pages?
Default: No.

Approved Expansion Areas for dedicated pages:
Optional. Only list areas that deserve their own URLs.
1.
2.
3.

Additional Categories already covered by core services:

Additional Categories that need separate pages:

GeoArticles per Service:
Default: 3

Preferred CTA:

Trust Signals:

GBP URL:
```

### Nota sobre las Primary Local Coverage Areas

```text
Primary Local Coverage Areas are not a mandatory GMB Crush page-count rule.
They are an operational simplification.
Start with the 3–5 strongest coverage areas inside content.
```

Es decir:

```text
No generan páginas por defecto.
Solo ayudan a priorizar qué zonas mencionar más a menudo dentro del contenido.
```

---

## 5. Ejemplo rellenado

```text
Business Name:
Cerrajeros Madrid 24h

Website URL:
https://www.cerrajerosmadrid24h.com

Full NAP:
- Name: Cerrajeros Madrid 24h
- Address: Calle Ejemplo 123, Madrid
- Phone: +34 600 000 000

Primary GBP Category:
Cerrajero

Additional GBP Categories:
1. Servicio de cerrajería de urgencia
2. Servicio de duplicado de llaves

Main City:
Madrid

Physical Location City:
Madrid

Core Services:
1. Apertura de puertas
2. Cerrajero urgente
3. Cambio de cerraduras
4. Duplicado de llaves
5. Instalación de cerraduras de seguridad

Primary Local Coverage Areas:
1. Chamberí
2. Salamanca
3. Retiro

Additional Local Coverage Areas:
1. Tetuán
2. Chamartín
3. Centro
4. Arganzuela
5. Alcobendas
6. Pozuelo
7. Getafe

Should Local Coverage Areas generate pages?
No, not in the base build.

Approved Expansion Areas:
None in Phase 1.

Additional Categories already covered by core services:
1. Servicio de cerrajería de urgencia

Additional Categories that need separate pages:
1. Duplicado de llaves

GeoArticles per Service:
3

Preferred CTA:
Llamar ahora

Trust Signals:
- Servicio 24h
- Técnicos locales
- Atención urgente
- Reseñas en Google

GBP URL:
[URL del GBP]
```

---

## 6. Fórmula base simplificada

La fórmula original con múltiples ciudades era útil para expansión, pero para una implementación local simple usamos:

```text
C = 1 Main City
```

### Base Formula — One Main City Build

```text
1 Homepage
+ S Service Overview Pages
+ 1 Main City GeoHub
+ S Main City Location-Based Service Pages
+ A Main City Additional Category Pages
+ G × S Main City GeoArticles
```

Donde:

```text
S = core services
A = additional categories that need separate pages
G = GeoArticles per service
```

### Ejemplo con 5 servicios

```text
1 Homepage
+ 5 Service Overview Pages
+ 1 Madrid GeoHub
+ 5 Madrid Service Pages
+ 1 Madrid Additional Category Page
+ 15 GeoArticles
= 28 páginas base
```

---

## 7. Local Coverage Areas y fórmula base

Las **Local Coverage Areas** no entran en la fórmula base.

Se usan en:

```text
Contenido
FAQs
Ejemplos locales
Secciones de cobertura
Schema areaServed
GeoArticles
Intro local
Bloques de confianza
```

No generan automáticamente:

```text
/area/
/category/area/service/
/area/article-topic/
```

Solo generan URLs si pasan a:

```text
Approved Expansion Areas
```

---

## 8. Optional Expansion Module

Este paso solo se activa cuando una Local Coverage Area merece sus propias URLs.

Una Local Coverage Area puede convertirse en **Approved Expansion Area** si cumple varias de estas condiciones:

```text
- Tiene demanda real de búsqueda.
- Tiene valor comercial.
- Los competidores tienen páginas dedicadas para esa zona.
- El negocio atiende realmente esa zona.
- Se puede escribir contenido único sin duplicar la página de Main City.
- No hace falta fingir una ubicación física.
- Hay intención hiperlocal clara.
```

### Ejemplo

```text
Approved Expansion Area:
Alcobendas
```

Podría generar:

```text
/alcobendas/
/cerrajero/alcobendas/apertura-puertas/
/alcobendas/cuanto-cuesta-un-cerrajero-urgente/
```

Si la zona aprobada es un barrio o distrito dentro de la Main City:

```text
Approved Expansion Area:
Chamberí
```

Podría generar:

```text
/madrid/chamberi/
/cerrajero/madrid/chamberi/apertura-puertas/
/madrid/chamberi/cuanto-cuesta-un-cerrajero-urgente/
```

Pero esto es expansión, no arquitectura base.

---

## 9. Content Structure by Page Type

Este es el núcleo del módulo.

Define cómo se estructura el contenido dentro de cada página y dónde usar las Local Coverage Areas.

---

# 9.1 Homepage

## Función

La homepage es el **Root Entity Anchor**.

Debe establecer:

```text
Marca
Categoría principal GBP
Servicio principal
Main City
NAP
Servicios principales
Confianza
CTA
Enlaces internos
```

## Estructura recomendada

```text
H1:
[Brand Name] – Trusted [Primary Service] in [Main City]

Intro:
Marca + servicio principal + Main City.

Quick Answer:
2 frases pensadas para AI Overview.

Core Services:
3–6 servicios principales con enlaces a Service Overview Pages.

Local Coverage Preview:
Mención breve de 3–5 Local Coverage Areas.

Trust Blocks:
Reviews, años de experiencia, certificaciones, garantías.

FAQ Section:
5–7 preguntas sobre servicio + Main City.

NAP Block:
Nombre, dirección, teléfono.

CTA:
Llamar, reservar, pedir presupuesto o contactar.

Internal Links:
Service Overview Pages
Main City GeoHub
Additional Category Page
Contact Page
```

## Uso de Local Coverage Areas en homepage

La homepage puede mencionar Local Coverage Areas, pero de forma ligera.

Ejemplo:

```text
Cerrajeros Madrid 24h ofrece servicios de cerrajería en Madrid para viviendas, locales y comunidades. Atendemos solicitudes en zonas como Chamberí, Salamanca, Retiro, Tetuán y Centro, siempre según disponibilidad y tipo de servicio.
```

## Regla

```text
La homepage no debe convertirse en una lista masiva de zonas.
La prioridad sigue siendo marca + servicio + Main City.
```

---

# 9.2 Service Overview Page

## Función

La Service Overview Page es un pilar temático sin ubicación.

No debe intentar posicionar para:

```text
servicio + ciudad
```

Debe construir autoridad sobre:

```text
servicio
problemas
proceso
beneficios
intención comercial e informacional
```

## Estructura recomendada

```text
H1:
Professional [Service] Services by [Brand Name]

Intro:
Qué es el servicio, a quién ayuda y qué problema resuelve.

H2 Authority:
Experiencia, credenciales, procesos, confianza.

H2 Uniqueness:
Qué diferencia este servicio.

H2 Depth:
Cómo funciona, qué incluye, pasos, entregables.

H2 Intent:
Quién necesita este servicio y cuándo.

H2 Optimization:
Servicios relacionados, comparativas, próximos pasos.

FAQs:
3–5 preguntas generales del servicio.

CTA:
Contacto o consulta.

Internal Links:
Homepage
Related Service Overview Pages
Main City Location-Based Service Page
Relevant GeoArticle
```

## Uso de Local Coverage Areas en Service Overview

```text
No mencionar Main City.
No mencionar Local Coverage Areas.
No mencionar barrios, distritos ni municipios.
```

## Regla

```text
Service Overview = no geolocalizada.
```

---

# 9.3 Location-Based Service Page

## Función

La Location-Based Service Page es la página comercial principal para:

```text
Servicio + Main City
```

Ejemplo:

```text
/cerrajero/madrid/apertura-puertas/
```

## Estructura recomendada

```text
H1:
[Brand Name] – [Service] in [Main City]

Intro local:
100–150 palabras con servicio + Main City + problema local.

Quick Local Answer:
2 frases que respondan la intención principal.

H2 Authority:
Por qué la empresa es fiable para este servicio en Main City.

H2 Uniqueness:
Qué diferencia el servicio en Main City.

H2 Depth:
Qué incluye el servicio y cómo funciona.

H2 Local Pain Points:
Problemas reales de clientes en Main City.

H2 Local Coverage Areas Served:
Zonas reales donde se atiende el servicio.

H2 Related Services in [Main City]:
Otros servicios relacionados en la ciudad.

FAQs:
3–5 preguntas locales.

CTA:
CTA local con intención comercial.

Internal Links:
Parent Service Overview Page
Main City GeoHub
Related services in Main City
Relevant GeoArticles
Contact Page

Schema:
LocalBusiness
BreadcrumbList
FAQPage optional
Speakable optional
```

## Dónde usar Local Coverage Areas

### Intro local

Mencionar 2–4 áreas si encaja de forma natural.

Ejemplo:

```text
Si necesitas apertura de puertas en Madrid, podemos ayudarte en situaciones habituales en pisos, locales y comunidades. Atendemos solicitudes en zonas como Chamberí, Salamanca, Retiro y Centro, siempre según disponibilidad y tipo de servicio.
```

### Sección específica

```md
## Apertura de puertas en Madrid y zonas de cobertura

Atendemos solicitudes de apertura de puertas en Madrid en zonas como Chamberí, Salamanca, Retiro, Tetuán, Chamartín, Centro y Arganzuela. También podemos cubrir áreas cercanas como Alcobendas o Pozuelo según disponibilidad y tipo de servicio.

Estas zonas ayudan a contextualizar la cobertura local, pero la página sigue siendo una página de apertura de puertas en Madrid.
```

### FAQs

```md
### ¿Atendéis apertura de puertas en Chamberí, Salamanca y Retiro?

Sí. Si estás en Madrid y necesitas apertura de puertas en zonas como Chamberí, Salamanca, Retiro, Centro o Tetuán, puedes contactar con nuestro equipo para recibir asistencia según disponibilidad y cobertura.
```

## Regla

```text
Local Coverage Areas refuerzan la página de Main City.
No sustituyen la intención principal de la página.
```

La intención principal sigue siendo:

```text
[Service] in [Main City]
```

---

# 9.4 Additional Category Page

## Función

La Additional Category Page da soporte a una categoría adicional del GBP.

Ejemplo:

```text
/cerrajero/madrid/duplicado-llaves/
```

## Estructura recomendada

```text
H1:
[Brand Name] – Expert [Additional Category Service] in [Main City]

Intro con problema local:
100–150 palabras con un escenario real.

H2 Authority:
Experiencia, confianza, formación, proceso.

H2 Uniqueness:
Qué diferencia este servicio en Main City.

H2 Depth:
Cómo funciona el servicio paso a paso.

H2 Intent:
Quién necesita este servicio y por qué.

H2 Optimization:
Comparaciones, servicios relacionados, próximos pasos.

H2 Local Coverage Use Case:
Cómo aplica el servicio en diferentes zonas atendidas.

FAQs:
3–5 preguntas.

CTA:
CTA local.

Internal Links:
Main City GeoHub
Related Location-Based Service Pages
Relevant GeoArticles
Contact Page

Schema:
Service with areaServed
BreadcrumbList
FAQPage optional
```

## Uso de Local Coverage Areas

Las Local Coverage Areas se usan para contextualizar la categoría adicional dentro de la Main City.

Ejemplo:

```text
El duplicado de llaves en Madrid puede ser útil para propietarios, inquilinos, comunidades y negocios en zonas como Chamberí, Salamanca, Retiro, Tetuán o Centro. Esta página está enfocada en duplicado de llaves en Madrid; las zonas mencionadas sirven para reforzar la cobertura local real del servicio.
```

## Regla

```text
No crear páginas de Additional Category por cada Local Coverage Area en la base.
```

---

# 9.5 GeoHub Page

## Función

El GeoHub es el contenedor local de la Main City.

Ejemplo:

```text
/madrid/
```

Debe agrupar:

```text
Servicios principales en Main City
Additional Category Pages en Main City
GeoArticles de Main City
Local Coverage Areas
Trust signals
CTA
Internal links
```

## Estructura recomendada

```text
H1:
[Brand Name] – [Industry] Services in [Main City]

City intro:
Contexto de la ciudad y necesidades locales.

Service Menu:
Listado de todos los servicios en Main City.

Additional Category Menu:
Listado de categorías adicionales en Main City.

Local Coverage Areas Section:
Zonas reales donde se atienden clientes.

GeoArticle Resources:
Guías y artículos relacionados con la ciudad.

Trust Signals:
Reviews, experiencia, casos, imágenes, garantías.

CTA:
Contactar, llamar, reservar o pedir presupuesto.

Internal Links:
Homepage
All Main City service pages
Additional Category Pages
GeoArticles
Contact Page

Schema:
CollectionPage
BreadcrumbList
LocalBusiness only if physical presence is real
```

## Sección recomendada de Local Coverage Areas

```md
## Zonas de cobertura local en [Main City]

Atendemos servicios de [Primary Service] en [Main City] y zonas como [Local Coverage Area 1], [Local Coverage Area 2], [Local Coverage Area 3], [Local Coverage Area 4] y [Local Coverage Area 5]. Estas áreas representan cobertura real del negocio y ayudan a reforzar el contexto GEO de la página.

Desde esta página puedes acceder a los servicios principales disponibles en [Main City], incluyendo [Service 1], [Service 2], [Service 3] y recursos útiles relacionados con problemas frecuentes de clientes locales.
```

## Ejemplo

```md
## Zonas de cobertura local en Madrid

Atendemos servicios de cerrajería en Madrid y zonas como Chamberí, Salamanca, Retiro, Tetuán, Chamartín, Centro y Arganzuela. También podemos cubrir áreas cercanas como Alcobendas, Pozuelo o Getafe según disponibilidad.

Desde esta página puedes acceder a los servicios principales disponibles en Madrid, incluyendo apertura de puertas, cerrajero urgente, cambio de cerraduras, duplicado de llaves e instalación de cerraduras de seguridad.
```

## Regla

```text
El GeoHub es el mejor lugar para explicar cobertura local.
```

Pero:

```text
No debe enlazar a Local Coverage Areas si no existen URLs aprobadas.
```

---

# 9.6 GeoArticle Page

## Función

El GeoArticle es un booster semántico.

No es una landing comercial.

Debe reforzar:

```text
Servicio + Main City + intención long-tail
```

Ejemplo:

```text
/madrid/cuanto-cuesta-un-cerrajero-urgente/
```

## Estructura recomendada

```text
H1:
[Article Topic] in [Main City]

Intro contextual:
Situación real + Main City + intención del usuario.

H2 Problem:
Explicar el problema o duda.

H2 Local Context:
Cómo afecta en Main City.

H2 Options / Mistakes:
Opciones, errores, comparativas o decisiones.

H2 When to Call:
Cuándo contactar con un profesional.

H2 Local Examples:
Ejemplos usando Local Coverage Areas, landmarks o escenarios reales.

FAQs:
3–5 preguntas.

CTA:
Enlace contextual a la página servicio + Main City.

Internal Links:
Matching Location-Based Service Page
Main City GeoHub
Related GeoArticle
Contact Page

Schema:
Article
FAQPage
BreadcrumbList
Speakable
```

## Uso de Local Coverage Areas

Las Local Coverage Areas se usan como ejemplos locales.

Ejemplo:

```text
El precio de un cerrajero urgente en Madrid puede variar según el tipo de cerradura, la hora, el desplazamiento y la zona. Una apertura sencilla en Chamberí puede no requerir el mismo trabajo que una intervención en un local de Salamanca, una comunidad en Retiro o una vivienda en Tetuán.
```

## Regla

```text
Usar Local Coverage Areas como referencias semánticas.
No afirmar ubicación física si no existe.
No convertir el GeoArticle en una landing de zona.
```

---

## 10. Tabla de uso por tipo de página

| Page Type | ¿Usa Local Coverage Areas? | Cómo las usa |
|---|---|---|
| Homepage | Sí, ligero | Service area preview, 3–5 zonas máximo |
| Service Overview | No | No debe ser local ni mencionar zonas |
| Location-Based Service | Sí | Intro, local pain points, sección de cobertura, FAQs |
| Additional Category | Sí | Escenarios locales, casos de uso y cobertura |
| GeoHub | Sí, recomendado | Sección principal de cobertura local |
| GeoArticle | Sí | Ejemplos, contexto, landmarks, FAQs |

---

## 11. Ejemplo práctico completo con Madrid

### Inputs

```text
Main City:
Madrid

Primary Category:
Cerrajero

Service:
Apertura de puertas

Primary Local Coverage Areas:
1. Chamberí
2. Salamanca
3. Retiro

Additional Local Coverage Areas:
1. Tetuán
2. Chamartín
3. Centro
4. Arganzuela
5. Alcobendas
6. Pozuelo
```

### URL principal

```text
/cerrajero/madrid/apertura-puertas/
```

### H1

```text
Cerrajeros Madrid 24h – Apertura de puertas en Madrid
```

### Sección de cobertura

```md
## Apertura de puertas en Madrid y zonas de cobertura

Atendemos solicitudes de apertura de puertas en Madrid en zonas como Chamberí, Salamanca, Retiro, Tetuán, Chamartín, Centro y Arganzuela. También podemos cubrir áreas cercanas como Alcobendas o Pozuelo según disponibilidad y tipo de servicio.

Estas zonas representan cobertura real del negocio y ayudan a contextualizar el servicio dentro de Madrid. La página sigue estando enfocada en apertura de puertas en Madrid, no en una zona concreta.
```

### FAQ

```md
### ¿Atendéis apertura de puertas en Chamberí, Salamanca y Retiro?

Sí. Si estás en Madrid y necesitas apertura de puertas en zonas como Chamberí, Salamanca, Retiro, Centro o Tetuán, puedes contactar con nuestro equipo para recibir asistencia según disponibilidad y cobertura.

### ¿También ofrecéis apertura de puertas en Alcobendas o Pozuelo?

Podemos atender algunas áreas cercanas a Madrid según disponibilidad, distancia y tipo de servicio. Si estás en Alcobendas, Pozuelo u otra zona cercana, lo mejor es llamar para confirmar cobertura.
```

### CTA

```md
¿Necesitas apertura de puertas en Madrid? Contacta con Cerrajeros Madrid 24h para recibir asistencia según disponibilidad, tipo de cerradura y zona de cobertura.
```

---

## 12. Anti-Error Rules

```text
Do not create pages for every Local Coverage Area by default.
Do not treat Local Coverage Areas as Target Cities in the base build.
Do not create internal links to Local Coverage Areas unless they have approved URLs.
Do not claim physical offices in Local Coverage Areas unless true.
Do not list dozens of areas unnaturally on every page.
Do not let Local Coverage Areas replace the Main City.
Do not create duplicate pages with the same intent.
Do not publish Local Coverage Area pages before the Main City architecture is complete.
```

---

## 13. Local Coverage Areas QA Checklist

| Check | Status |
|---|---|
| Main City is clear? | ⬜ |
| Local Coverage Areas are real service areas? | ⬜ |
| Primary Local Coverage Areas are limited to 3–5? | ⬜ |
| Local Coverage Areas are used naturally? | ⬜ |
| No fake office/location claim? | ⬜ |
| No unnecessary coverage-area URLs created? | ⬜ |
| No duplicate intent with Main City pages? | ⬜ |
| Schema areaServed matches real coverage? | ⬜ |
| Internal links only point to real approved URLs? | ⬜ |
| Page remains focused on one service and one Main City? | ⬜ |
| Approved Expansion Areas are clearly separated from base coverage areas? | ⬜ |

---

## 14. Prompt block para actualizar el Master Prompt

Añadir este bloque al **Paso 11 — Master Prompt reutilizable**.

```text
Main City:
[INSERT]

Physical Location City:
[INSERT]

Local Coverage Areas:
Real areas where the business serves customers. These may include neighborhoods, districts, nearby towns, municipalities, ZIP codes, urbanizations, or service zones.
[INSERT LIST]

Primary Local Coverage Areas:
Start with the 3–5 strongest areas to mention most often.
[INSERT LIST]

Additional Local Coverage Areas:
Optional secondary coverage areas to mention naturally.
[INSERT LIST]

Should Local Coverage Areas generate pages?
Default: No.

Approved Expansion Areas:
Only list areas that should receive dedicated URLs.
[INSERT LIST]

Rules:
- Build the base architecture around one Main City.
- Use Local Coverage Areas as GEO content signals.
- Do not create URLs for Local Coverage Areas unless they are approved as Expansion Areas.
- Do not use Target Cities or Secondary Cities in the base build.
- Do not claim a physical location in any Local Coverage Area unless true.
- Local Coverage Areas may appear in homepage, GeoHub, Location-Based Service Pages, Additional Category Pages and GeoArticles.
- Service Overview Pages must not mention Main City or Local Coverage Areas.
```

---

## 15. Cómo actualizar la fórmula del sistema principal

Sustituir la fórmula original de múltiples ciudades por esta en la versión base:

```text
1 Homepage
+ S Service Overview Pages
+ 1 Main City GeoHub
+ S Main City Location-Based Service Pages
+ A Main City Additional Category Pages
+ G × S Main City GeoArticles
```

Mantener como módulo opcional:

```text
Expansion Module:
+ E Expansion GeoHub Pages
+ S × E Expansion Location-Based Service Pages
+ A × E Expansion Additional Category Pages
+ G × S × E Expansion GeoArticles
```

Donde:

```text
E = Approved Expansion Areas
```

---

## 16. Cómo actualizar el internal linking

### Base build

```text
Homepage
→ Service Overview Pages
→ Main City GeoHub
→ Main City Additional Category Page
→ Contact

Service Overview
→ Homepage
→ Main City Service Page
→ Related Service Overview Pages
→ Relevant GeoArticle

Main City GeoHub
→ Homepage
→ All Main City Service Pages
→ Main City Additional Category Pages
→ Main City GeoArticles
→ Contact

Location-Based Service
→ Parent Service Overview
→ Main City GeoHub
→ Related services in Main City
→ Related GeoArticles
→ Contact

Additional Category
→ Main City GeoHub
→ Related Main City services
→ Related GeoArticles
→ Contact

GeoArticle
→ Matching Location-Based Service Page
→ Main City GeoHub
→ Related GeoArticle
→ Contact
```

### Local Coverage Areas

```text
Local Coverage Areas do not receive internal links unless they have approved URLs.
```

### Approved Expansion Areas

If an area becomes approved for dedicated URLs:

```text
Main City GeoHub
→ Approved Expansion Area Hub

Approved Expansion Area Hub
→ Expansion Service Pages

Expansion Service Page
→ Parent Service Overview
→ Main City GeoHub
→ Related Expansion Pages
→ Contact
```

---

## 17. Final Rules

```text
Main City creates the base architecture.
Local Coverage Areas enrich local relevance.
Approved Expansion Areas create additional URLs only when justified.
Mentioning an area does not mean creating a page for it.
Service Overview Pages stay non-local.
Location-Based Service Pages focus on one service and one Main City.
GeoHub is the best page for explaining coverage.
GeoArticles use Local Coverage Areas as examples, not as landing targets.
Never fake physical presence.
Never create internal links to URLs that do not exist.
Never let Local Coverage Areas replace the Main City.
```

---

## 18. Resumen operativo

La versión simplificada del sistema queda así:

```text
1. Main City = genera la arquitectura.
2. Local Coverage Areas = enriquecen contenido y cobertura.
3. Approved Expansion Areas = generan páginas solo si se aprueban.
4. La fórmula base usa una sola ciudad.
5. Las páginas de servicio + ciudad mencionan áreas de cobertura de forma natural.
6. El GeoHub explica la cobertura local con más detalle.
7. Los GeoArticles usan áreas de cobertura como ejemplos semánticos.
8. Service Overview Pages no usan localización.
9. No se crean páginas por cada zona por defecto.
10. La expansión se activa solo cuando hay demanda, competencia o justificación comercial.
```

---

## 19. Dónde insertar este paso dentro del sistema

Insertar este paso justo después de:

```text
Paso 5 — Page Type Rules
```

y antes de:

```text
Paso 7 — Internal Linking Rules
```

Nombre recomendado:

```text
Paso 6 — Content Architecture by Page Type + Local Coverage Areas
```

o:

```text
Paso 6 — Estructura de Contenido y Áreas de Cobertura Local
```
