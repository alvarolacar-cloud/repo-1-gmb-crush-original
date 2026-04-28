# Módulo 19 — Escalado post-lanzamiento

Versión añadida · Capa de Salida al Mercado · Sistema GMB Crush  
Este módulo define cómo medir, optimizar y escalar después de publicar.

---

## Índice del módulo

1. Objetivo del Módulo 19  
2. Cuándo se ejecuta  
3. Lo que tienes que rellenar  
4. Ejemplo rellenado — Cerrajeros Madrid 24h  
5. Cuerpo operativo  
6. Checklist de verificación  
7. Outputs del módulo  

---

# 1. Objetivo del Módulo 19

El objetivo del Módulo 19 es evitar que el sistema se quede parado después del lanzamiento.

Este módulo define:

```text
qué medir
cuándo optimizar
cuándo refrescar contenido
cuándo crear nuevas páginas
cuándo NO escalar
qué datos faltan
qué acciones dependen del futuro módulo de competidores
```

Este módulo no crea páginas nuevas automáticamente.

---

# 2. Cuándo se ejecuta

Ejecutar después de:

```text
Módulo 18 — QA de lanzamiento
Publicación
Indexación inicial
Configuración de tracking
```

No ejecutar si falta:

```text
GSC
GA4
tracking de conversiones
Geo-grid si aplica
sitemap enviado
URLs indexables
```

---

# 3. Lo que tienes que rellenar

## 3.1 — Datos de seguimiento

| Campo | Valor |
|---|---|
| Dominio | [DOMAIN] |
| Fecha publicación | [DATE] |
| GSC configurado | [SÍ / NO] |
| GA4 configurado | [SÍ / NO] |
| Conversiones configuradas | [SÍ / NO] |
| Geo-grid inicial | [SÍ / NO] |
| GBP creado | [SÍ / NO] |
| GBP verificado | [SÍ / NO] |

---

## 3.2 — Métricas a vigilar

| Métrica | Fuente | Frecuencia |
|---|---|---|
| Indexación | GSC | Semanal |
| Impresiones por URL | GSC | Semanal |
| Clicks por URL | GSC | Semanal |
| CTR | GSC | Semanal |
| Posición media | GSC | Semanal |
| Leads | GA4 / CRM | Semanal |
| Clics tel | GA4 | Semanal |
| Formularios | GA4 / CRM | Semanal |
| Geo-grid | GMB Crush | Quincenal / mensual |

---

# 4. Ejemplo rellenado — Cerrajeros Madrid 24h

| Campo | Valor |
|---|---|
| Dominio | `https://www.cerrajerosmadrid24h.com` |
| Fecha publicación | Pendiente |
| GSC configurado | Pendiente |
| GA4 configurado | Pendiente |
| Conversiones configuradas | Pendiente |
| Geo-grid inicial | Pendiente |
| GBP creado | No |
| GBP verificado | No |

---

# 5. Cuerpo operativo

## Regla 1 — No escalar antes de medir

### Explicación

No se crean nuevas páginas por intuición. Primero se mide si la base responde.

### Señales mínimas

```text
URLs indexadas
impresiones iniciales
clicks o leads
GeoArticles enviando tráfico
Location-Based Service Pages recibiendo consultas
```

### Ejemplo incorrecto

```text
Publicar la web y crear al día siguiente 20 páginas de barrio.
```

### Regla final

```text
Escalar sin datos rompe el sistema.
```

---

## Regla 2 — Medir el flujo GeoArticle → LBS → Contacto

### Explicación

El sistema funciona si los artículos alimentan páginas comerciales y estas llevan a contacto.

### Métricas

| Flujo | Qué medir |
|---|---|
| GeoArticle → LBS | clics internos |
| LBS → Contacto | clics CTA |
| Contacto → Lead | formulario / llamada |
| GeoHub → LBS | navegación local |
| Homepage → LBS | distribución de autoridad |

### Regla final

```text
El flujo importa más que una URL aislada.
```

---

## Regla 3 — Optimización de contenido

### Cuándo optimizar

```text
URL indexada sin impresiones
URL con impresiones y bajo CTR
URL con clics y sin conversión
GeoArticle sin puente narrativo efectivo
LBS sin CTA visible
GeoHub sin navegación útil
```

### Acciones

```text
revisar H1
revisar meta title
revisar intro
añadir FAQs
mejorar CTA
añadir enlaces internos
mejorar trust signals confirmados
```

### Regla final

```text
Primero optimizar, después escalar.
```

---

## Regla 4 — Refresh de GeoArticles

### Frecuencia

```text
cada 3–6 meses
```

### Qué revisar

```text
datos desactualizados
precios
FAQs
enlaces internos
secciones débiles
nuevas preguntas de usuarios
schema
```

### Regla final

```text
GeoArticles se mantienen vivos.
```

---

## Regla 5 — Escalado a nuevas zonas

### Explicación

Las Local Coverage Areas no generan URLs por defecto. Pueden evolucionar a Approved Expansion Areas solo si hay datos.

### Triggers internos

| Trigger | Condición |
|---|---|
| LBS responde | La página principal recibe impresiones/clics |
| GeoArticles responden | 1–2 artículos reciben tráfico |
| Leads aparecen | Contacto o llamadas desde la zona/servicio |
| Zona validada | La zona tiene coherencia con el sistema |
| Contenido único posible | Se puede crear contenido no duplicado |

### Regla final

```text
Candidate LCA no es URL. Approved Expansion Area sí puede ser URL.
```

---

## Regla 6 — Competidores quedan para módulo futuro

### Explicación

La validación SERP/competidores no se ejecuta en este módulo todavía.

### Estado

```text
Pendiente de módulo de competidores
```

### Qué queda bloqueado hasta ese módulo

```text
crear páginas de barrio por SERP
crear nuevas ciudades
cambiar servicios por gap competitivo
priorizar por competition gap
```

### Regla final

```text
Si una acción depende de competidores, queda pendiente.
```

---

## Regla 7 — Cuándo crear una página nueva

### Puede crearse si

```text
la página madre existe
la página madre responde
hay intención diferenciada
no canibaliza
hay contenido único
hay datos que lo justifican
pasa QA
```

### No puede crearse si

```text
solo se quiere cubrir más mapa
solo se añade barrio al H1
no hay contenido único
no hay datos
rompe interlinking
finge ubicación física
```

### Regla final

```text
Una página nueva debe fortalecer el cluster, no diluirlo.
```

---

## Regla 8 — Plan post-lanzamiento por ciclos

### Ciclo 1 — Semana 1–2

```text
verificar indexación
revisar errores técnicos
enviar sitemap
configurar GSC/GA4
revisar formulario
```

### Ciclo 2 — Semana 3–6

```text
analizar impresiones
ajustar metadata
revisar CTR
mejorar CTAs
revisar enlaces internos
```

### Ciclo 3 — Mes 2–3

```text
optimizar páginas con datos
refrescar GeoArticles débiles
preparar GBP si no está creado
iniciar primera lectura geo-grid
```

### Ciclo 4 — Mes 3+

```text
evaluar expansión
priorizar nuevas páginas
activar módulo de competidores
crear roadmap trimestral
```

---

# 6. Checklist de verificación

| Check | Pregunta | Estado |
|---|---|---|
| Indexación | ¿Todas las URLs SEO están indexables? | ⬜ |
| GSC | ¿Search Console está configurado? | ⬜ |
| GA4 | ¿GA4 mide eventos clave? | ⬜ |
| Leads | ¿Se miden formularios y llamadas? | ⬜ |
| GeoArticles | ¿Envían tráfico a LBS? | ⬜ |
| LBS | ¿Reciben impresiones/clicks? | ⬜ |
| Contacto | ¿Convierte o hay fricción? | ⬜ |
| GBP | ¿Está creado o planificado? | ⬜ |
| Escalado | ¿Hay datos suficientes para ampliar? | ⬜ |
| Competidores | ¿La acción requiere módulo futuro? | ⬜ |

---

# 7. Outputs del Módulo 19

Al terminar este módulo deben existir:

```text
Post-launch Monitoring Matrix
Optimization Log
Indexation Report
Conversion Tracking Report
GeoArticle Performance Report
LBS Performance Report
Expansion Candidate List
Blocked-by-Competitors List
Quarterly Roadmap
```
