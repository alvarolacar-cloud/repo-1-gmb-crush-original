# Módulo 15 — Redacción final por URL

Versión añadida · Capa de Salida al Mercado · Sistema GMB Crush  
Este módulo no modifica la arquitectura SEO. Convierte las URLs aprobadas en contenido final listo para diseño y construcción.

---

## Índice del módulo

1. Objetivo del Módulo 15  
2. Cuándo se ejecuta  
3. Lo que tienes que rellenar  
4. Ejemplo rellenado — Cerrajeros Madrid 24h  
5. Cuerpo operativo  
6. Checklist de verificación  
7. Outputs del módulo  

---

# 1. Objetivo del Módulo 15

El objetivo del Módulo 15 es transformar la arquitectura aprobada en **contenido final por URL**.

Los pasos anteriores ya deciden:

```text
qué páginas existen
qué tipo de página es cada una
qué URL tiene cada página
qué servicio o ciudad ataca
qué schema requiere
qué enlaces internos necesita
qué prioridad tiene
qué decisiones están respaldadas y cuáles siguen pendientes
```

Este módulo decide:

```text
qué texto final va en cada página
qué H1, H2, FAQs, CTA y metadata se usan
qué entidades se insertan
qué Local Coverage Areas se mencionan
qué trust signals se pueden usar
qué bloques necesitan prueba humana antes de publicar
```

Este módulo no inventa servicios, categorías, horarios, años de experiencia, reseñas ni precios. Si un dato está marcado como `IA sin respaldo` en decisiones/fuentes, aquí debe quedar como:

```text
pendiente de validación
placeholder bloqueado
no publicable hasta confirmación
```

---

# 2. Cuándo se ejecuta

Ejecutar solo cuando estén cerrados:

```text
Paso 1 — Intake
Paso 2 — Fórmula
Paso 3 — URL Matrix
Paso 4 — URL Rules
Paso 5 — Page Type Rules
Paso 6 — Content Architecture + Local Coverage Areas
Paso 7 — Internal Linking
Paso 8 — Priority Score
Paso 9 — QA base
Paso 10 — Producción en fases
Paso 14 — GBP planificado si aplica
```

No ejecutar si falta:

```text
URL Matrix
Page Type por URL
Servicios aprobados
Main City
NAP
CTA principal
Internal Linking Map
Schema Map
Estado de datos sin respaldo
```

---

# 3. Lo que tienes que rellenar

## 3.1 — Datos base del proyecto

| Campo | Valor |
|---|---|
| Business Name | [BUSINESS_NAME] |
| Website Root Domain | [DOMAIN] |
| Main City | [MAIN_CITY] |
| Primary GBP Category planificada | [PRIMARY_CATEGORY] |
| NAP final | [NAP] |
| Email | [EMAIL] |
| Teléfono | [PHONE] |
| CTA principal | [CTA] |
| Estado del GBP | [GBP_STATUS] |

---

## 3.2 — Fuentes internas obligatorias

| Fuente | Estado |
|---|---|
| URL Matrix | [VALIDADA / PENDIENTE] |
| Page Type Rules | [VALIDADA / PENDIENTE] |
| Content Architecture | [VALIDADA / PENDIENTE] |
| Internal Linking Map | [VALIDADA / PENDIENTE] |
| Schema Map | [VALIDADA / PENDIENTE] |
| Priority Score | [VALIDADA / PENDIENTE] |
| Decisiones y fuentes | [VALIDADA / PENDIENTE] |

---

## 3.3 — Inventario de URLs a redactar

| ID | URL | Page Type | Servicio | Ciudad | Estado |
|---|---|---|---|---|---|
| [ID] | [URL] | [TYPE] | [SERVICE] | [CITY] | [PENDIENTE] |

---

## 3.4 — Datos que NO se pueden inventar

| Dato | Estado |
|---|---|
| Años de experiencia | [CONFIRMADO / BLOQUEADO] |
| Reseñas | [CONFIRMADO / BLOQUEADO] |
| Precios | [CONFIRMADO / BLOQUEADO] |
| Horarios | [CONFIRMADO / BLOQUEADO] |
| Garantías | [CONFIRMADO / BLOQUEADO] |
| Certificaciones | [CONFIRMADO / BLOQUEADO] |
| Fotos / casos reales | [CONFIRMADO / BLOQUEADO] |

---

# 4. Ejemplo rellenado — Cerrajeros Madrid 24h

## 4.1 — Datos base

| Campo | Valor |
|---|---|
| Business Name | Cerrajeros Madrid 24h |
| Website Root Domain | `https://www.cerrajerosmadrid24h.com` |
| Main City | Madrid |
| Primary GBP Category planificada | Cerrajero |
| NAP final | Cerrajeros Madrid 24h · Calle Rafael Calvo 12 · Madrid · +34 600 000 000 |
| Email | `info@cerrajerosmadrid24h.com` |
| Teléfono | +34 600 000 000 |
| CTA principal | Llamar ahora |
| Estado del GBP | Not Created |

## 4.2 — URLs ejemplo a redactar

| ID | URL | Page Type | Servicio | Ciudad | Estado |
|---|---|---|---|---|---|
| HP-001 | `/` | Homepage | Cerrajero | Madrid | Pendiente |
| SO-001 | `/cerrajero/cerrajero-urgente/` | Service Overview | Cerrajero urgente | Sin ciudad | Pendiente |
| LBS-001 | `/cerrajero/madrid/cerrajero-urgente/` | Location-Based Service | Cerrajero urgente | Madrid | Pendiente |
| AC-001 | `/cerrajero/madrid/duplicado-llaves/` | Additional Category | Duplicado de llaves | Madrid | Pendiente |
| GH-001 | `/madrid/` | GeoHub | Cerrajería | Madrid | Pendiente |
| GA-001 | `/madrid/cuanto-cuesta-un-cerrajero-urgente/` | GeoArticle | Cerrajero urgente | Madrid | Pendiente |

## 4.3 — Datos bloqueados en el ejemplo

| Dato | Estado |
|---|---|
| Reseñas Google | Bloqueado hasta crear GBP |
| 10+ años de experiencia | Pendiente de confirmación |
| Garantía de trabajo | Pendiente de confirmación |
| Teléfono | Placeholder pendiente |
| Email | Placeholder pendiente |
| Precios | Pendiente de datos reales |

---

# 5. Cuerpo operativo

## Regla 1 — El contenido se redacta por URL, no por servicio genérico

### Explicación

Cada URL tiene una función distinta. Una Service Overview no debe sonar igual que una Location-Based Service Page. Un GeoArticle no debe vender como una landing. Un GeoHub no debe ser solo un índice de enlaces.

### Patrón

```text
URL → Page Type → función → estructura → copy final
```

### Ejemplo correcto

```text
/cerrajero/cerrajero-urgente/
```

Debe explicar el servicio sin orientar el contenido principal a Madrid.

```text
/cerrajero/madrid/cerrajero-urgente/
```

Debe convertir búsquedas de cerrajero urgente en Madrid.

### Ejemplo incorrecto

```text
Usar el mismo texto en /cerrajero/cerrajero-urgente/ y /cerrajero/madrid/cerrajero-urgente/.
```

### Regla final

```text
Una URL = una función = un copy único.
```

---

## Regla 2 — Homepage como Root Entity Anchor

### Explicación

La homepage debe establecer entidad: marca, servicio principal, ciudad, NAP, servicios core, confianza y acceso a las páginas principales.

### Estructura obligatoria

| Sección | Contenido |
|---|---|
| Hero | Marca + servicio principal + Main City + CTA |
| Servicios principales | 3–6 servicios con links |
| Cobertura | Main City + Local Coverage Areas ligeras |
| Confianza | Solo trust signals confirmados |
| NAP | Visible y rastreable |
| CTA final | Contacto o llamada |
| Internal links | Service Overview, GeoHub, Contacto |

### Ejemplo correcto

```text
H1: Cerrajeros Madrid 24h — Cerrajero urgente en Madrid
CTA: Llamar ahora
Servicios: cerrajero urgente, apertura de puertas, cambio de cerraduras...
```

### Ejemplo incorrecto

```text
H1: Los mejores cerrajeros baratos cerca de mí
```

### Regla final

```text
La homepage ancla la entidad, no compite con todas las páginas internas.
```

---

## Regla 3 — Service Overview Page sin ciudad como target principal

### Explicación

La Service Overview Page es el pilar temático del servicio. No debe transformarse en landing local.

### Estructura obligatoria

| Sección | Contenido |
|---|---|
| H1 | Servicio + marca |
| Intro | Qué es el servicio |
| Problemas | Qué resuelve |
| Proceso | Cómo se ejecuta |
| Materiales / herramientas | Entidades técnicas |
| FAQs | Preguntas generales |
| CTA | Enlace a versión local |
| Links | Homepage, LBS, servicios relacionados, GeoArticles |

### Ejemplo correcto

```text
H1: Servicio de cerrajero urgente de Cerrajeros Madrid 24h
CTA: Ver cerrajero urgente en Madrid
```

### Ejemplo incorrecto

```text
H1: Cerrajero urgente en Madrid
```

en la Service Overview no geolocalizada.

### Regla final

```text
Service Overview = servicio sin ciudad.
```

---

## Regla 4 — Location-Based Service Page como página de conversión

### Explicación

La LBS debe convertir búsquedas de servicio + ciudad. Es la página comercial local principal.

### Estructura obligatoria

| Sección | Contenido |
|---|---|
| H1 | Servicio + ciudad |
| Intro local | 100–150 palabras |
| Problemas locales | Casos reales del servicio en la ciudad |
| Proceso | Cómo se presta el servicio |
| Local Coverage Areas | Solo como señales GEO |
| FAQs locales | 3–5 preguntas |
| CTA | Urgente / presupuesto / llamada |
| Schema | LocalBusiness + FAQPage + BreadcrumbList |
| Links | Service Overview, GeoHub, servicios relacionados, GeoArticles |

### Ejemplo correcto

```text
H1: Cerrajero urgente en Madrid
```

Puede mencionar:

```text
Almagro, Chamberí y zonas próximas
```

como contexto, sin crear páginas por barrio.

### Ejemplo incorrecto

```text
Tenemos oficina en Salamanca
```

si no es verdad.

### Regla final

```text
LBS = servicio + Main City + conversión.
```

---

## Regla 5 — Additional Category Page

### Explicación

Una Additional Category Page soporta una categoría adicional del futuro GBP.

### Estructura obligatoria

| Sección | Contenido |
|---|---|
| H1 | Servicio adicional + ciudad |
| Intro | Problema local concreto |
| AUDIO | Authority, Uniqueness, Depth, Intent, Optimization |
| FAQs | Preguntas long-tail |
| CTA | Adaptado a ciudad |
| Schema | Service + BreadcrumbList |
| Links | GeoHub, LBS relacionadas, GeoArticles |

### Ejemplo correcto

```text
/cerrajero/madrid/duplicado-llaves/
H1: Duplicado de llaves en Madrid
```

### Ejemplo incorrecto

```text
Crear una página de “Proveedor de sistemas de seguridad” sin servicio real ni soporte.
```

### Regla final

```text
Cada categoría adicional efectiva necesita soporte web real.
```

---

## Regla 6 — GeoHub como contenedor local

### Explicación

El GeoHub no es una landing de venta pura. Organiza la ciudad, servicios, categorías y artículos.

### Estructura obligatoria

| Sección | Contenido |
|---|---|
| H1 | Servicios de cerrajería en Madrid |
| Intro | Contexto de ciudad |
| Servicios | Links a LBS |
| Additional Category | Links a páginas de soporte |
| GeoArticles | Links a artículos |
| Local Coverage Areas | Neighborhood coverage si aplica |
| CTA | Explorar servicios / contactar |
| Schema | CollectionPage + BreadcrumbList |

### Ejemplo correcto

```text
/madrid/
```

Lista:

```text
Cerrajero urgente en Madrid
Apertura de puertas en Madrid
Cambio de cerraduras en Madrid
```

### Ejemplo incorrecto

```text
/madrid/ solo con una lista de enlaces sin contenido contextual.
```

### Regla final

```text
GeoHub = contenedor de ciudad con contenido propio.
```

---

## Regla 7 — GeoArticles como boosters semánticos

### Explicación

Los GeoArticles no son landings. Deben responder una intención long-tail y reforzar una LBS o GeoHub.

### Estructura obligatoria

| Sección | Contenido |
|---|---|
| H1 | Pregunta o tema + ciudad |
| Intro | Contexto real |
| Desarrollo | Datos, criterios, errores, comparativas |
| FAQs | 3–5 preguntas |
| Puentes narrativos | 2–3 enlaces a LBS |
| CTA suave | Ir a la página de servicio |
| Schema | Article + FAQPage + Breadcrumb + Speakable |

### Ejemplo correcto

```text
/madrid/cuanto-cuesta-un-cerrajero-urgente/
```

Debe enlazar a:

```text
/cerrajero/madrid/cerrajero-urgente/
/madrid/
```

### Ejemplo incorrecto

```text
Artículo que repite todo el copy de la LBS y vende igual que una landing.
```

### Regla final

```text
GeoArticle = servicio + ciudad + intención long-tail.
```

---

## Regla 8 — No publicar datos sin respaldo

### Explicación

El contenido final no puede convertir placeholders en claims reales.

### Bloqueos típicos

| Dato | Acción |
|---|---|
| Reseñas no existentes | No mencionar |
| Años no confirmados | Bloquear |
| Precio no validado | Usar “pendiente” o pedir dato |
| Garantía no confirmada | Bloquear |
| Horarios no confirmados | Bloquear |
| Certificaciones no confirmadas | Bloquear |

### Ejemplo correcto

```text
Reseñas iniciales pendientes tras crear y verificar el GBP.
```

### Ejemplo incorrecto

```text
250+ reseñas en Google
```

si el GBP no existe.

### Regla final

```text
No se redacta como verdad lo que no está validado.
```

---

## Regla 9 — Output final por URL

Cada URL debe entregar:

| Campo | Obligatorio |
|---|---|
| URL | Sí |
| Page Type | Sí |
| H1 | Sí |
| Meta Title | Sí |
| Meta Description | Sí |
| Secciones H2/H3 | Sí |
| Copy final | Sí |
| FAQs | Sí |
| CTA | Sí |
| Internal Links | Sí |
| Schema recomendado | Sí |
| Datos pendientes | Sí |

---

# 6. Checklist de verificación

| Check | Pregunta | Estado |
|---|---|---|
| URL Matrix | ¿Todas las URLs tienen copy asignado? | ⬜ |
| Page Type | ¿Cada copy respeta su tipo de página? | ⬜ |
| Local | ¿Las LBS usan ciudad y LCA sin falsas ubicaciones? | ⬜ |
| GeoArticles | ¿Cada artículo enlaza a LBS y GeoHub? | ⬜ |
| Trust | ¿No hay reseñas, años o garantías inventadas? | ⬜ |
| Metadata | ¿Todas las URLs tienen title y description? | ⬜ |
| Schema | ¿Cada página tiene schema recomendado? | ⬜ |
| Links | ¿El internal linking coincide con el mapa aprobado? | ⬜ |
| No duplicados | ¿No se repite copy entre páginas? | ⬜ |
| Build-ready | ¿El contenido está listo para diseño y construcción? | ⬜ |

---

# 7. Outputs del Módulo 15

Al terminar este módulo deben existir:

```text
Content Pack por URL
Metadata Matrix
FAQ Matrix
CTA Matrix
Internal Link Copy Matrix
Schema Content Notes
Datos bloqueados / pendientes
Aprobación de contenido para pasar a diseño y construcción
```
