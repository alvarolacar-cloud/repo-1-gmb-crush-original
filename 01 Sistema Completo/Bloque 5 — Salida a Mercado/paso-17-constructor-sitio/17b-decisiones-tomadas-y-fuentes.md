# Paso 17 — Constructor del Sitio

Fase 2 de trazabilidad del sistema GMB Crush.

Fuentes permitidas:

```text
GMB Crush
Input humano
Input humano + GMB Crush
Datos de búsqueda
Competidores
IA sin respaldo
GMB Crush + IA sin respaldo
Input humano + IA sin respaldo
IA heredada (paso X.YY)
Decisión de diseño
```

---

## Bloque 1 — Fase 0: Acta de Lectura y Autocontraste

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 17.01 · Paso-17 §7.1 Acta de Lectura | Se decide leer literalmente los outputs de Pasos 1, 2, 3, 4, 5, 6, 7, 15 y 16 | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Sin Acta de Lectura no se inicia construcción. | Acta con valores literales: nombre, NAP, Main City, LCAs, servicios, URL Matrix, Internal Linking, Design Tokens |
| 17.02 · Paso-17 §7.2 Autocontraste | Se decide ejecutar autocontraste entre bloques antes de construir | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Si hay contradicción entre bloques, parar y reportar. | 8 cruces verificados: URLs, servicios, Main City, NAP, Internal Linking, Layout-Map vs secciones |
| 17.03 · Paso-17 §7.3 Materialización del Diseño | Se decide materializar Design Tokens y Layout-Map en archivos consumibles | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Tokens y Layout-Map listos para Fase 1. | design-tokens.md, layout-map.md, contraste-check.md |

## Bloque 2 — Fase 1: Setup técnico

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 17.04 · Paso-17 §8 Setup | Se decide inicializar el proyecto Astro 5 | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Stack canónico cerrado. | `pnpm create astro@latest` |
| 17.05 · Paso-17 §8 Setup | Se decide instalar Tailwind CSS v3 | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Tailwind v3 (no v4) por compatibilidad con `@astrojs/tailwind`. | `pnpm astro add tailwind` |
| 17.06 · Paso-17 §8 Setup | Se decide configurar `tailwind.config.mjs` con tokens del Paso 16 | IA heredada (paso 16.18–16.20) | El valor se hereda de decisiones de Decisión de diseño en el paso indicado. Esta decisión se cura cuando se cierran las decisiones origen. | tailwind.config.mjs con font-heading, primary, btn-radius, etc. |
| 17.07 · Paso-17 §8 Setup | Se decide inyectar variables CSS heredadas del Paso 16 en `global.css` | IA heredada (paso 16.18–16.20) | El valor se hereda de decisiones de Decisión de diseño en el paso indicado. Esta decisión se cura cuando se cierran las decisiones origen. | src/styles/global.css con variables CSS root |

## Bloque 3 — Fase 2: Componentes UI

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 17.08 · Paso-17 §9 Componentes | Se decide construir Button.astro parametrizable | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Componente canónico del stack con variantes primary/secondary/outline. | src/components/Button.astro con tokens del Paso 16 |
| 17.09 · Paso-17 §9 Componentes | Se decide construir Card.astro parametrizable | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Variantes: servicio, zona, testimonio, geoarticle teaser. | src/components/Card.astro |
| 17.10 · Paso-17 §9 Componentes | Se decide construir Badge.astro | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Etiquetas para trust signals y categorías. | src/components/Badge.astro |
| 17.11 · Paso-17 §9 Componentes | Se decide construir Hero.astro parametrizable según page type | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. El Hero varía por page type (Paso 16 §11). | src/components/Hero.astro |
| 17.12 · Paso-17 §9 Componentes | Se decide construir Testimonial.astro estático | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Sin reseñas inventadas si el GBP no existe (Paso 1.44, Paso 14.46). | src/components/Testimonial.astro |
| 17.13 · Paso-17 §9 Componentes | Se decide construir FAQ.astro como acordeón accesible | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. ARIA correcto, navegación por teclado. | src/components/FAQ.astro |
| 17.14 · Paso-17 §9 Componentes | Se decide construir ContactForm.astro con campos del NAP | IA heredada (paso 1.08–1.15) | El valor se hereda del NAP del Paso 1. Esta decisión se cura cuando se cierra la decisión origen. | src/components/ContactForm.astro con campos basados en NAP |

## Bloque 4 — Fase 3: Layout Global

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 17.15 · Paso-17 §10 Layout | Se decide construir Header.astro con menú del Paso 7 y teléfono del Paso 1 | IA heredada (paso 1.14, paso 7.01–7.04) | El valor se hereda de decisiones del Paso 1 (teléfono IA) y Paso 7 (estructura de enlaces GMB Crush). | Header con menú a SO + GeoHub + Contacto + teléfono |
| 17.16 · Paso-17 §10 Layout | Se decide construir Footer.astro con NAP completo del Paso 1 | IA heredada (paso 1.08–1.15) | El valor se hereda del NAP del Paso 1 (mezcla Input humano e IA). | Footer con NAP completo + enlaces a silos del Paso 7 |
| 17.17 · Paso-17 §10 Layout | Se decide construir Layout.astro como wrapper global | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Layout único que envuelve todas las páginas con Header + slot + Footer. | src/layouts/Layout.astro |

## Bloque 5 — Fase 4: Construcción de Páginas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 17.18 · Paso-17 §11 Páginas | Se decide construir la Homepage según copy del Paso 15 y layout del Paso 16 | IA heredada (paso 15.06, paso 16.27) | El valor se hereda del copy del Paso 15 (GMB Crush + IA sin respaldo) y del Layout-Map del Paso 16 (Decisión de diseño). | src/pages/index.astro |
| 17.19 · Paso-17 §11 Páginas | Se decide construir las 5 Service Overview Pages | IA heredada (paso 15.11, paso 16.28) | El valor se hereda del copy del Paso 15 y del Layout-Map del Paso 16. Servicios heredados del Paso 1.34–1.38. | 5 src/pages/cerrajero/[service].astro |
| 17.20 · Paso-17 §11 Páginas | Se decide construir las 5 Location-Based Service Pages | IA heredada (paso 15.16, paso 16.29) | El valor se hereda del copy del Paso 15 y del Layout-Map del Paso 16. Servicios heredados del Paso 1.34–1.38. | 5 src/pages/cerrajero/madrid/[service].astro |
| 17.21 · Paso-17 §11 Páginas | Se decide construir la Additional Category Page | IA heredada (paso 15.21, paso 16.30) | El valor se hereda del copy del Paso 15 y del Layout-Map del Paso 16. Categoría heredada del Paso 1.18. | src/pages/cerrajero/madrid/duplicado-llaves.astro |
| 17.22 · Paso-17 §11 Páginas | Se decide construir el GeoHub /madrid/ | IA heredada (paso 15.26, paso 16.31) | El valor se hereda del copy del Paso 15 y del Layout-Map del Paso 16. Main City heredada del Paso 1.20. | src/pages/madrid/index.astro |
| 17.23 · Paso-17 §11 Páginas | Se decide construir los 15 GeoArticles | IA heredada (paso 15.31, paso 16.32) | El valor se hereda del copy del Paso 15 y del Layout-Map del Paso 16. Topics heredados del Paso 3.19–3.33. | 15 src/pages/madrid/[topic].astro |
| 17.24 · Paso-17 §11 Páginas | Se decide construir /contacto/ como página auxiliar | IA heredada (paso 1.08–1.15) | El valor se hereda del NAP del Paso 1. La estructura es GMB Crush (página auxiliar simple). | src/pages/contacto.astro |

## Bloque 6 — Fase 5: SEO y Schema

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 17.25 · Paso-17 §12 SEO | Se decide implementar SEO.astro con title, meta description y canonical | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Heredado del mapa schema del Paso 5.18. | src/components/SEO.astro |
| 17.26 · Paso-17 §12 Schema | Se decide implementar Schema LocalBusiness en Homepage, LBS y GeoHub | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. NAP del Paso 1.08–1.15 heredado. | LocalBusiness JSON-LD en 7 páginas |
| 17.27 · Paso-17 §12 Schema | Se decide implementar Schema Service en Service Overview Pages y Additional Category | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Heredado del mapa schema del Paso 5.18. | Service JSON-LD en 6 páginas |
| 17.28 · Paso-17 §12 Schema | Se decide implementar Schema FAQPage en páginas con FAQ (LBS + GeoArticles + Homepage) | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. | FAQPage JSON-LD donde aplique |
| 17.29 · Paso-17 §12 SEO | Se decide implementar sitemap.xml con todas las URLs del Paso 3 | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. `@astrojs/sitemap` con las 28 SEO + /contacto/. | public/sitemap-index.xml |
| 17.30 · Paso-17 §12 SEO | Se decide implementar robots.txt apuntando al sitemap | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. No bloquear URLs SEO. | public/robots.txt |

## Bloque 7 — Fase 6: Limpieza de Rastros de IA

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 17.31 · Paso-17 §13 Limpieza IA | Se decide sustituir o eliminar el README.md del starter kit | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Sin README starter kit visible. | README.md propio o eliminado |
| 17.32 · Paso-17 §13 Limpieza IA | Se decide eliminar comentarios de instrucción del scaffold en archivos `.astro/.ts/.js` | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Sin "este componente hace X" del template. | Archivos limpios sin comentarios scaffold |
| 17.33 · Paso-17 §13 Limpieza IA | Se decide verificar ausencia de `meta generator` en HTML de producción | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Sin `<meta name="generator">` visible. | HTML final sin meta generator |
| 17.34 · Paso-17 §13 Limpieza IA | Se decide ejecutar grep limpio de referencias a IA | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. `grep -ri "claude\|chatgpt\|gpt-\|openai\|anthropic"` debe salir limpio. | grep sin matches |
| 17.35 · Paso-17 §13 Limpieza IA | Se decide renombrar `package.json` con el nombre real del proyecto | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Sin `astro-starter` ni similares. | "name": "cerrajeros-madrid-24h" |
| 17.36 · Paso-17 §13 Limpieza IA | Se decide revisar commits para eliminar referencias a IA | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Sin "via Claude" ni similares. | git log limpio |
