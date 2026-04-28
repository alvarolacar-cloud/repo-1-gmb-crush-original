# Módulo 17 — Construcción web

Versión añadida · Capa de Salida al Mercado · Sistema GMB Crush  
Este módulo construye la web real a partir de arquitectura, contenido y diseño aprobados.

---

## Índice del módulo

1. Objetivo del Módulo 17  
2. Cuándo se ejecuta  
3. Lo que tienes que rellenar  
4. Ejemplo rellenado — Cerrajeros Madrid 24h  
5. Cuerpo operativo  
6. Checklist de verificación  
7. Outputs del módulo  

---

# 1. Objetivo del Módulo 17

El objetivo del Módulo 17 es convertir el sistema aprobado en una web funcional.

Este módulo implementa:

```text
rutas
layouts
componentes
contenido
metadata
schema
sitemap
robots
forms
internal linking
responsive
build
```

No decide:

```text
nuevas URLs
nuevos servicios
nuevas zonas
nuevas categorías GBP
nuevos contenidos
nuevo diseño
```

Si algo no está en los módulos anteriores, se bloquea y se pregunta.

---

# 2. Cuándo se ejecuta

Ejecutar después de:

```text
Módulo 15 — Redacción final por URL
Módulo 16 — Extracción de diseño
```

No ejecutar si falta:

```text
URL Matrix aprobada
Content Pack aprobado
Design Tokens aprobados
Layout Map aprobado
Internal Linking Map
Schema Map
NAP definitivo o placeholders marcados
```

---

# 3. Lo que tienes que rellenar

## 3.1 — Stack del proyecto

| Campo | Valor |
|---|---|
| Framework | [Astro / WordPress / Webflow / Otro] |
| CSS | [Tailwind / CSS / Otro] |
| Package manager | [pnpm / npm / yarn] |
| Hosting | [Cloudflare Pages / Otro] |
| Build command | [COMMAND] |
| Repo GitHub | [REPO_URL] |
| Dominio producción | [DOMAIN] |

---

## 3.2 — Fuentes de verdad

| Fuente | Estado |
|---|---|
| URL Matrix | [VALIDADA / PENDIENTE] |
| Content Pack | [VALIDADA / PENDIENTE] |
| Design Tokens | [VALIDADA / PENDIENTE] |
| Layout Map | [VALIDADA / PENDIENTE] |
| Internal Linking Map | [VALIDADA / PENDIENTE] |
| Schema Map | [VALIDADA / PENDIENTE] |
| QA base | [VALIDADA / PENDIENTE] |

---

## 3.3 — Componentes requeridos

| Componente | Estado |
|---|---|
| Header | ⬜ |
| Footer | ⬜ |
| Layout | ⬜ |
| SEO Component | ⬜ |
| Hero | ⬜ |
| Service Card | ⬜ |
| CTA Block | ⬜ |
| FAQ | ⬜ |
| Breadcrumbs | ⬜ |
| Contact Form | ⬜ |
| Schema Component | ⬜ |

---

# 4. Ejemplo rellenado — Cerrajeros Madrid 24h

| Campo | Valor |
|---|---|
| Framework | Astro 5 |
| CSS | Tailwind v3 |
| Package manager | pnpm |
| Hosting | Cloudflare Pages |
| Build command | `pnpm run build` |
| Dominio producción | `https://www.cerrajerosmadrid24h.com` |
| URL contacto | `/contacto/` |

---

# 5. Cuerpo operativo

## Regla 1 — Construir desde fuentes de verdad

### Explicación

El constructor no inventa. Solo implementa.

### Orden de lectura

```text
1. URL Matrix
2. Content Pack
3. Design Tokens
4. Layout Map
5. Internal Linking Map
6. Schema Map
7. QA base
```

### Ejemplo correcto

```text
URL Matrix dice:
/cerrajero/madrid/cerrajero-urgente/

El constructor crea exactamente esa ruta.
```

### Ejemplo incorrecto

```text
Crear /servicios/cerrajero-urgente-madrid/ porque parece más natural.
```

### Regla final

```text
La estructura de carpetas no decide URLs; la URL Matrix decide URLs.
```

---

## Regla 2 — Acta de lectura antes de construir

### Explicación

Antes de crear el proyecto, hay que copiar los valores críticos.

### Tabla de acta

| Dato | Valor copiado | Fuente |
|---|---|---|
| Business Name | [COPIAR] | Paso 1 |
| NAP | [COPIAR] | Paso 1 |
| Main City | [COPIAR] | Paso 1 |
| Servicios | [COPIAR] | URL Matrix |
| Total URLs | [COPIAR] | URL Matrix |
| Design Tokens | [COPIAR] | Módulo 16 |
| CTA principal | [COPIAR] | Módulo 15 |

### Regla final

```text
Si el acta de lectura tiene contradicciones, no se construye.
```

---

## Regla 3 — Setup técnico

### Stack recomendado por defecto

```text
Astro 5
Tailwind CSS v3
pnpm
Cloudflare Pages
```

### Comandos base

```bash
pnpm create astro@latest
pnpm astro add tailwind
pnpm install
pnpm run build
```

### Regla final

```text
El build debe funcionar antes de publicar.
```

---

## Regla 4 — Componentes UI

### Componentes mínimos

```text
Button
Card
Badge
Hero
FAQ
Breadcrumb
CTA
ContactForm
Header
Footer
Layout
SEO
Schema
```

### Ejemplo correcto

```text
Hero.astro recibe props:
title
subtitle
ctaLabel
ctaHref
pageType
```

### Ejemplo incorrecto

```text
Hero hardcodeado para una sola página.
```

### Regla final

```text
Componentes reutilizables, no bloques hardcodeados.
```

---

## Regla 5 — Construcción de páginas

### Orden recomendado

```text
Homepage
Contacto
Service Overview Pages
GeoHub
Location-Based Service Pages
Additional Category Pages
GeoArticles
```

### Verificación por página

| Campo | Obligatorio |
|---|---|
| Ruta exacta | Sí |
| H1 único | Sí |
| Metadata | Sí |
| Copy aprobado | Sí |
| CTA | Sí |
| Internal links | Sí |
| Schema | Sí |
| Responsive | Sí |

### Regla final

```text
Una página no está construida si le falta contenido, metadata, enlaces o schema.
```

---

## Regla 6 — SEO técnico

### Elementos obligatorios

```text
title
meta description
canonical
Open Graph
schema
sitemap
robots.txt
breadcrumbs
```

### Ejemplo correcto

```text
canonical de /madrid/ apunta a /madrid/
```

### Ejemplo incorrecto

```text
Todas las páginas usan el canonical de la homepage.
```

### Regla final

```text
Cada URL SEO debe tener SEO técnico propio.
```

---

## Regla 7 — Schema por tipo de página

| Page Type | Schema |
|---|---|
| Homepage | Organization + WebSite |
| Service Overview | Service + WebPage + BreadcrumbList |
| LBS | LocalBusiness + FAQPage + BreadcrumbList |
| Additional Category | Service + BreadcrumbList |
| GeoHub | CollectionPage + BreadcrumbList |
| GeoArticle | Article + FAQPage + BreadcrumbList + Speakable |
| Contacto | ContactPage + Organization |

### Regla final

```text
Schema genérico para todo el sitio = incorrecto.
```

---

## Regla 8 — Limpieza de rastros de IA

### Revisar

```text
comentarios de instrucciones
prompts internos
texto placeholder
nombres de starter kit
meta generator
commits con referencias IA
package name genérico
```

### Comandos útiles

```bash
grep -R "ChatGPT\\|AI\\|placeholder\\|TODO\\|CopyEdit" .
```

### Regla final

```text
La web publicada no debe contener rastros del proceso de generación.
```

---

# 6. Checklist de verificación

| Check | Pregunta | Estado |
|---|---|---|
| Acta | ¿Se copiaron valores literales de fuentes de verdad? | ⬜ |
| Setup | ¿El proyecto compila? | ⬜ |
| URLs | ¿Todas las rutas coinciden con URL Matrix? | ⬜ |
| Contenido | ¿Cada página usa Content Pack aprobado? | ⬜ |
| Diseño | ¿Tokens y layout coinciden con Módulo 16? | ⬜ |
| Links | ¿Internal linking coincide con mapa? | ⬜ |
| Schema | ¿Schema por tipo correcto? | ⬜ |
| SEO | ¿Metadata y canonical por URL? | ⬜ |
| Contacto | ¿Formulario y teléfono funcionan? | ⬜ |
| IA traces | ¿No hay rastros IA? | ⬜ |
| Build | ¿`pnpm run build` pasa? | ⬜ |

---

# 7. Outputs del Módulo 17

Al terminar este módulo deben existir:

```text
Repositorio construido
Componentes UI
Páginas implementadas
SEO técnico implementado
Schema implementado
Sitemap
Robots
Build aprobado
Issue Log técnico
Sitio listo para QA de lanzamiento
```
