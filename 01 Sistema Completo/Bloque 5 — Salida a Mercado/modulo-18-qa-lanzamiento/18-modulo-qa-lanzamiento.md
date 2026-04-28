# Módulo 18 — QA de lanzamiento

Versión añadida · Capa de Salida al Mercado · Sistema GMB Crush  
Este módulo valida que la web se puede publicar sin errores críticos.

---

## Índice del módulo

1. Objetivo del Módulo 18  
2. Cuándo se ejecuta  
3. Lo que tienes que rellenar  
4. Ejemplo rellenado — Cerrajeros Madrid 24h  
5. Cuerpo operativo  
6. Checklist de verificación  
7. Outputs del módulo  

---

# 1. Objetivo del Módulo 18

El objetivo del Módulo 18 es decidir si la web está lista para salir al mercado.

Este módulo audita:

```text
URLs
canonical
metadata
schema
contenido
diseño
responsive
formularios
internal linking
sitemap
robots
performance básica
rastros de IA
despliegue
indexación inicial
```

El resultado final debe ser:

```text
GO
NO-GO
GO con incidencias menores
```

---

# 2. Cuándo se ejecuta

Ejecutar después de:

```text
Módulo 17 — Construcción web
```

No ejecutar si:

```text
la web no compila
faltan páginas
faltan metadatos
faltan contenidos
faltan design tokens
no hay URL de staging o preview
```

---

# 3. Lo que tienes que rellenar

## 3.1 — Datos de QA

| Campo | Valor |
|---|---|
| Proyecto | [PROJECT] |
| Dominio | [DOMAIN] |
| URL staging | [STAGING_URL] |
| Fecha QA | [DATE] |
| Responsable QA | [NAME] |
| Framework | [ASTRO / WORDPRESS / OTRO] |
| Build aprobado | [SÍ / NO] |

---

## 3.2 — Inventario de URLs

| URL | Page Type | Estado QA |
|---|---|---|
| [URL] | [TYPE] | [PENDIENTE] |

---

# 4. Ejemplo rellenado — Cerrajeros Madrid 24h

| Campo | Valor |
|---|---|
| Proyecto | Cerrajeros Madrid 24h |
| Dominio | `https://www.cerrajerosmadrid24h.com` |
| URL staging | [pendiente] |
| Fecha QA | [pendiente] |
| Responsable QA | SEO / Dev |
| Framework | Astro 5 + Tailwind v3 |
| Build aprobado | Pendiente |

---

# 5. Cuerpo operativo

## Regla 1 — QA técnico obligatorio

### Checks

| Elemento | Criterio |
|---|---|
| URLs | Coinciden con URL Matrix |
| 404 | No hay errores |
| Canonical | Cada página apunta a sí misma |
| Sitemap | Incluye todas las URLs SEO |
| Robots | No bloquea URLs SEO |
| Header/Footer | Enlaces correctos |
| Formulario | Funciona |
| Teléfono | `tel:` correcto |
| Build | Sin errores |

### Ejemplo incorrecto

```text
/madrid/ existe en sitemap pero devuelve 404.
```

### Regla final

```text
Sin QA técnico aprobado, no se publica.
```

---

## Regla 2 — QA de contenido

### Checks

| Elemento | Criterio |
|---|---|
| H1 | Único por página |
| Copy | Coincide con Content Pack |
| FAQs | Presentes si aplican |
| CTA | Visible y funcional |
| NAP | Consistente |
| Trust | Solo datos confirmados |
| No duplicación | No hay copy clonado entre páginas |
| Local | No hay falsa ubicación |

### Ejemplo incorrecto

```text
Página de Salamanca dice que hay oficina física sin prueba.
```

### Regla final

```text
El contenido debe respetar decisiones y fuentes.
```

---

## Regla 3 — QA visual

### Checks

| Elemento | Criterio |
|---|---|
| Colores | Coinciden con tokens |
| Tipografías | Coinciden con tokens |
| Hero | No rompe mobile |
| Cards | Consistentes |
| CTAs | Visibles |
| Imágenes | Ratios correctos |
| Layout | Coincide con layout-map |

### Regla final

```text
La web debe verse como el diseño aprobado, no como una interpretación libre.
```

---

## Regla 4 — QA responsive

### Breakpoints mínimos

```text
375px
768px
1280px
```

### Checks

```text
sin overflow horizontal
menú usable
CTA visible
formulario usable
cards apiladas
texto legible
```

### Regla final

```text
Mobile roto = no-go.
```

---

## Regla 5 — QA de schema

### Validar por tipo

| Page Type | Schema requerido |
|---|---|
| Homepage | Organization + WebSite |
| Service Overview | Service + BreadcrumbList |
| LBS | LocalBusiness + FAQPage + BreadcrumbList |
| Additional Category | Service + BreadcrumbList |
| GeoHub | CollectionPage + BreadcrumbList |
| GeoArticle | Article + FAQPage + BreadcrumbList + Speakable |
| Contacto | ContactPage |

### Regla final

```text
Schema debe coincidir con Page Type.
```

---

## Regla 6 — QA de internal linking

### Checks

```text
Homepage enlaza a páginas principales
Service Overview enlaza a LBS
LBS enlaza a Service Overview + GeoHub + GeoArticles
GeoArticles enlazan a LBS + GeoHub
GeoHub enlaza a LBS + Additional Category + GeoArticles
No hay páginas huérfanas
No se enlazan URLs inexistentes
```

### Regla final

```text
Una web local sin interlinking aprobado no está lista.
```

---

## Regla 7 — QA de rastros IA

### Revisar

```text
CopyEdit
placeholder
Lorem ipsum
ChatGPT
AI-generated
instrucciones internas
comentarios de prompt
starter kit
meta generator
```

### Regla final

```text
No publicar rastros del proceso.
```

---

## Regla 8 — Clasificación GO / NO-GO

| Estado | Condición |
|---|---|
| GO | 0 errores críticos |
| GO con incidencias menores | Solo errores no bloqueantes |
| NO-GO | Cualquier error crítico |

### Errores críticos

```text
404 en URL SEO
canonical incorrecto
schema crítico ausente
formulario roto
teléfono incorrecto
NAP inconsistente
copy con datos inventados
mobile roto
URLs no aprobadas
```

### Regla final

```text
Un error crítico bloquea el lanzamiento.
```

---

# 6. Checklist de verificación

| Área | Check | Estado |
|---|---|---|
| Técnica | URLs, canonical, sitemap, robots, build | ⬜ |
| Contenido | H1, copy, FAQs, CTA, NAP, no invención | ⬜ |
| Visual | tokens, layout, responsive, imágenes | ⬜ |
| Schema | schema por tipo validado | ⬜ |
| Links | internal linking aprobado | ⬜ |
| Forms | contacto y teléfono funcionan | ⬜ |
| IA traces | sin rastros IA | ⬜ |
| Deploy | staging listo | ⬜ |

---

# 7. Outputs del Módulo 18

Al terminar este módulo deben existir:

```text
Launch QA Matrix
Issue Log
Critical Errors List
Minor Fixes List
GO / NO-GO decision
Deployment Approval
Post-launch checklist
```
