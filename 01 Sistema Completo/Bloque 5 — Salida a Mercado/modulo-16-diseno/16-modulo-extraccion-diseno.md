# Módulo 16 — Extracción de diseño

Versión añadida · Capa de Salida al Mercado · Sistema GMB Crush  
Este módulo no modifica la arquitectura SEO. Extrae diseño, tokens y layout para construir la web.

---

## Índice del módulo

1. Objetivo del Módulo 16  
2. Cuándo se ejecuta  
3. Lo que tienes que rellenar  
4. Ejemplo rellenado — Cerrajeros Madrid 24h  
5. Cuerpo operativo  
6. Checklist de verificación  
7. Outputs del módulo  

---

# 1. Objetivo del Módulo 16

El objetivo del Módulo 16 es transformar una referencia visual aprobada en un sistema de diseño ejecutable.

Este módulo produce:

```text
Design Tokens
UI Kit
Layout Map
Component Map
Responsive Rules
Image Ratio Rules
Typography Rules
```

No redacta contenido.  
No decide URLs.  
No cambia arquitectura.  
No decide qué páginas existen.

Solo responde:

```text
cómo debe verse la web
qué diseño se debe construir
qué tokens debe usar el constructor
qué layouts corresponden a cada tipo de página
```

---

# 2. Cuándo se ejecuta

Ejecutar después de:

```text
Módulo 15 — Redacción final por URL
```

y antes de:

```text
Módulo 17 — Construcción web
```

No ejecutar si falta:

```text
referencia visual
capturas full-page
logos si existen
preferencias de marca
Content Pack
tipos de página aprobados
```

---

# 3. Lo que tienes que rellenar

## 3.1 — Datos de diseño

| Campo | Valor |
|---|---|
| Web de referencia | [URL_REFERENCIA] |
| Tipo de referencia | [Competidor / Plantilla / Web propia / Inspiración] |
| Logo disponible | [SÍ / NO] |
| Paleta existente | [SÍ / NO] |
| Tipografía existente | [SÍ / NO] |
| Estilo deseado | [Sobrio / Urgente / Premium / Técnico / Minimalista] |
| Stack de diseño | [Tailwind / CSS / otro] |

---

## 3.2 — Capturas requeridas

| Página | Captura full-page | Estado |
|---|---|---|
| Homepage referencia | [UPLOAD] | ⬜ |
| Service Page referencia | [UPLOAD] | ⬜ |
| Location Page referencia | [UPLOAD] | ⬜ |
| Blog / Article referencia | [UPLOAD] | ⬜ |
| Mobile screenshot | [UPLOAD] | ⬜ |

---

## 3.3 — Elementos visuales a extraer

| Elemento | Valor |
|---|---|
| Color primario | [HEX] |
| Color secundario | [HEX] |
| Color acento | [HEX] |
| Color fondo | [HEX] |
| Color texto principal | [HEX] |
| Fuente heading | [FONT] |
| Fuente body | [FONT] |
| H1 desktop | [PX] |
| H1 mobile | [PX] |
| H2 desktop | [PX] |
| Body size | [PX] |
| Button radius | [PX] |
| Card radius | [PX] |
| Card shadow | [CSS] |

---

# 4. Ejemplo rellenado — Cerrajeros Madrid 24h

| Campo | Valor |
|---|---|
| Web de referencia | [pendiente de aportar] |
| Tipo de referencia | Web de inspiración |
| Logo disponible | Pendiente |
| Paleta existente | Pendiente |
| Tipografía existente | Pendiente |
| Estilo deseado | Urgente, claro, profesional, móvil primero |
| Stack de diseño | Tailwind CSS |

Capturas requeridas:

```text
Homepage referencia
Service Page referencia
Location Page referencia
Article referencia
Mobile screenshot
```

---

# 5. Cuerpo operativo

## Regla 1 — No estimar diseño sin capturas

### Explicación

El diseño debe salir de una referencia visual, no de una preferencia inventada.

### Patrón

```text
Screenshot → extracción → tokens → propuesta → aprobación → layout definitivo
```

### Ejemplo correcto

```text
Color primario extraído: #0F172A
Button radius observado: 8px
Card shadow observado: 0 10px 25px rgba(...)
```

### Ejemplo incorrecto

```text
Usar azul porque parece profesional.
```

### Regla final

```text
Sin captura, no hay extracción.
```

---

## Regla 2 — Separar identidad visual de layout

### Explicación

Los colores y tipografías no son lo mismo que el layout. Hay que extraer ambas cosas.

### Identidad visual

```text
colores
tipografías
tamaños
radios
shadows
estados de botones
```

### Layout

```text
hero
cards
grid
secciones
espaciado
imágenes
CTA blocks
formulario
footer
```

### Regla final

```text
Design Tokens ≠ Layout Map.
```

---

## Regla 3 — Tokens primero, CSS después

### Explicación

Antes de construir componentes, hay que convertir el diseño en tokens.

### Output esperado

```text
primary
secondary
accent
bg-light
bg-dark
text-primary
text-light
font-heading
font-body
btn-radius
card-radius
card-shadow
container-width
section-padding
```

### Ejemplo correcto

```text
primary: #111827
accent: #F59E0B
font-heading: Inter
btn-radius: 8px
```

### Ejemplo incorrecto

```text
Usar clases sueltas sin sistema: text-blue-600, bg-yellow-400, shadow-lg.
```

### Regla final

```text
Un diseño se construye con tokens, no con decisiones sueltas.
```

---

## Regla 4 — Layout por tipo de página

### Explicación

Cada tipo de página tiene secciones distintas. El layout debe adaptarse a la función de cada página.

### Homepage

```text
Hero
Servicios
Autoridad
Cobertura
Trust
CTA
```

### Service Overview

```text
Hero Servicio
Problema
Proceso
Materiales
FAQs
CTA a LBS
```

### Location-Based Service

```text
Hero Local
Contexto local
Servicio en ciudad
Zonas
Confianza
FAQs
CTA conversión
```

### GeoArticle

```text
Article Hero
Intro
Desarrollo
Bloques de apoyo
Puentes narrativos
CTA suave
```

### GeoHub

```text
Hero Ciudad
Listado de servicios
Coverage
GeoArticles
CTA suave
```

### Regla final

```text
El layout debe respetar el Page Type.
```

---

## Regla 5 — Mobile-first obligatorio

### Explicación

Las webs locales convierten mucho desde móvil. El diseño debe funcionar primero en 375px.

### Checklist mobile

```text
CTA visible
teléfono clicable
hero no saturado
cards apiladas
menú usable
formulario simple
sin overflow horizontal
```

### Ejemplo correcto

```text
Hero mobile:
H1 corto
CTA visible
tel: enlazado
sin imagen que empuje el CTA fuera del viewport
```

### Ejemplo incorrecto

```text
Hero desktop adaptado a móvil sin revisar.
```

### Regla final

```text
Si no funciona en móvil, no está aprobado.
```

---

## Regla 6 — Propuesta antes de output definitivo

### Explicación

El diseño necesita aprobación. No se debe construir directamente con tokens no aprobados.

### Flujo

```text
Extracción 4.1
Layout 4.2
Propuesta 4.3
Aprobación
Tokens definitivos 4.4
```

### Regla final

```text
El constructor solo recibe diseño aprobado.
```

---

# 6. Checklist de verificación

| Check | Pregunta | Estado |
|---|---|---|
| Capturas | ¿Hay screenshots full-page suficientes? | ⬜ |
| Colores | ¿Todos los colores tienen HEX? | ⬜ |
| Tipografía | ¿Las fuentes están identificadas? | ⬜ |
| Tokens | ¿Hay tokens Tailwind/CSS claros? | ⬜ |
| Layout | ¿Cada Page Type tiene layout-map? | ⬜ |
| Mobile | ¿Hay reglas responsive? | ⬜ |
| Imágenes | ¿Ratios y posiciones están definidos? | ⬜ |
| CTA | ¿Los botones tienen estilos definidos? | ⬜ |
| Aprobación | ¿El usuario aprobó la propuesta? | ⬜ |

---

# 7. Outputs del Módulo 16

Al terminar este módulo deben existir:

```text
Design Tokens
Layout Map por Page Type
UI Kit base
Component Map
Responsive Rules
Image Ratio Rules
Design Approval
```
