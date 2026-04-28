# Paso 18 — QA y Deploy

Fase 2 de trazabilidad del sistema GMB Crush.

Fuentes permitidas:

```text
GMB Crush
Input humano
Decisión de diseño
IA sin respaldo
IA heredada (paso X.YY)
```

Orígenes del dato permitidos:

```text
Doctrina GMB Crush
Input humano
Competidores
Datos de búsqueda
Decisión de diseño
Heredado del paso X.YY
IA sin respaldo
```

---

## Bloque 1 — Auditoría Técnica (16 criterios)

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 18.01 · Paso-18 §7 Aud. Técnica | Se decide validar URLs contra la URL Matrix | GMB Crush | Doctrina GMB Crush | El framework define esta regla. URLs en producción = URLs del Paso 3 sin desviaciones. | 28 URLs SEO + /contacto/ verificadas |
| 18.02 · Paso-18 §7 Aud. Técnica | Se decide validar canonical en cada página | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Canonical apunta a la propia URL. | 29 canonicals correctos |
| 18.03 · Paso-18 §7 Aud. Técnica | Se decide validar Header con menú del Paso 7 + teléfono Paso 1.14 | GMB Crush | Doctrina GMB Crush | El framework define esta regla. | Header con menú correcto y teléfono +34 600 000 000 |
| 18.04 · Paso-18 §7 Aud. Técnica | Se decide validar Footer con NAP del Paso 1 + enlaces del Paso 7 | GMB Crush | Doctrina GMB Crush | El framework define esta regla. | Footer con NAP completo y enlaces a silos |
| 18.05 · Paso-18 §7 Aud. Técnica | Se decide validar que no haya páginas huérfanas | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Cada URL del Paso 3 tiene al menos un enlace entrante en el Internal Linking Map. | 0 páginas huérfanas |
| 18.06 · Paso-18 §7 Aud. Técnica | Se decide validar Meta Tags únicos por página | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Title y description únicos. | 29 títulos únicos, 29 descriptions únicos |
| 18.07 · Paso-18 §7 Aud. Técnica | Se decide validar un H1 único por página con keyword principal | GMB Crush | Doctrina GMB Crush | El framework define esta regla. | 29 H1s únicos con keyword |
| 18.08 · Paso-18 §7 Aud. Técnica | Se decide validar Schema Organization + WebSite en Homepage | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Schema canónico de Homepage. | Organization + WebSite presentes en / |
| 18.09 · Paso-18 §7 Aud. Técnica | Se decide validar Schema LocalBusiness en Homepage + LBS + GeoHub con NAP del Paso 1 | GMB Crush | Doctrina GMB Crush | El framework define esta regla. NAP heredado del Paso 1.08–1.15. | LocalBusiness en 7 páginas con NAP correcto |
| 18.10 · Paso-18 §7 Aud. Técnica | Se decide validar Schema Service en SO + AC | GMB Crush | Doctrina GMB Crush | El framework define esta regla. | Service en 6 páginas |
| 18.11 · Paso-18 §7 Aud. Técnica | Se decide validar Schema CollectionPage en GeoHub | GMB Crush | Doctrina GMB Crush | El framework define esta regla. | CollectionPage en /madrid/ |
| 18.12 · Paso-18 §7 Aud. Técnica | Se decide validar Schema Article + FAQPage en GeoArticles | GMB Crush | Doctrina GMB Crush | El framework define esta regla. | Article + FAQPage en 15 GeoArticles |
| 18.13 · Paso-18 §7 Aud. Técnica | Se decide validar Schema BreadcrumbList en todas las páginas | GMB Crush | Doctrina GMB Crush | El framework define esta regla. | BreadcrumbList en 29 páginas |
| 18.14 · Paso-18 §7 Aud. Técnica | Se decide validar sitemap.xml con todas las URLs del Paso 3 | GMB Crush | Doctrina GMB Crush | El framework define esta regla. | sitemap-index.xml con 29 URLs |
| 18.15 · Paso-18 §7 Aud. Técnica | Se decide validar robots.txt | GMB Crush | Doctrina GMB Crush | El framework define esta regla. No bloquea URLs SEO, apunta al sitemap. | robots.txt correcto |
| 18.16 · Paso-18 §7 Aud. Técnica | Se decide validar responsive en 375 / 768 / 1280 | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Mobile-first del Paso 16 §10. | Sin desbordamientos en 3 breakpoints |

## Bloque 2 — Auditoría de Contenido (8 criterios)

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 18.17 · Paso-18 §8 Aud. Contenido | Se decide validar copy de Homepage contra Paso 15.06–15.09 | GMB Crush | Heredado del paso 15.06–15.09 | El framework dicta validar el copy. Valores heredados del copy del Paso 15 (IA sin respaldo). | Copy Homepage idéntico al aprobado en Paso 15 |
| 18.18 · Paso-18 §8 Aud. Contenido | Se decide validar copy de las 5 Service Overview Pages contra Paso 15.11–15.14 | GMB Crush | Heredado del paso 15.11–15.14 | El framework dicta validar el copy. Valores heredados del copy del Paso 15 (IA sin respaldo). | 5 SOs con copy idéntico |
| 18.19 · Paso-18 §8 Aud. Contenido | Se decide validar copy de las 5 LBS contra Paso 15.16–15.19 | GMB Crush | Heredado del paso 15.16–15.19 | El framework dicta validar el copy. Valores heredados del copy del Paso 15 (IA sin respaldo). | 5 LBS con copy idéntico |
| 18.20 · Paso-18 §8 Aud. Contenido | Se decide validar copy de la Additional Category contra Paso 15.21–15.24 | GMB Crush | Heredado del paso 15.21–15.24 | El framework dicta validar el copy. Valores heredados del copy del Paso 15 (IA sin respaldo). | AC con copy idéntico |
| 18.21 · Paso-18 §8 Aud. Contenido | Se decide validar copy del GeoHub contra Paso 15.26–15.29 | GMB Crush | Heredado del paso 15.26–15.29 | El framework dicta validar el copy. Valores heredados del copy del Paso 15 (IA sin respaldo). | GeoHub con copy idéntico |
| 18.22 · Paso-18 §8 Aud. Contenido | Se decide validar copy de los 15 GeoArticles contra Paso 15.31–15.34 | GMB Crush | Heredado del paso 15.31–15.34 | El framework dicta validar el copy. Valores heredados del copy del Paso 15 (IA sin respaldo). | 15 GeoArticles con copy idéntico |
| 18.23 · Paso-18 §8 Aud. Contenido | Se decide validar puentes narrativos en GeoArticles (3 puntos por artículo) | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Regla del Paso 15.35. | 15 GeoArticles con 3 puentes cada uno |
| 18.24 · Paso-18 §8 Aud. Contenido | Se decide validar NAP consistente en Header, Footer, Contact, schema | GMB Crush | Doctrina GMB Crush | El framework define esta regla. NAP del Paso 1.08–1.15 idéntico en todos los puntos. | NAP único: Cerrajeros Madrid 24h, Calle Rafael Calvo 12, Madrid, +34 600 000 000 |

## Bloque 3 — Auditoría Visual (5 criterios)

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 18.25 · Paso-18 §9 Aud. Visual | Se decide validar colores contra Design Tokens del Paso 16.18–16.20 | GMB Crush | Heredado del paso 16.18–16.20 | El framework dicta validar los colores. Valores heredados de Decisión de diseño en el Paso 16. | Todos los colores de producción coinciden con tokens |
| 18.26 · Paso-18 §9 Aud. Visual | Se decide validar tipografías contra Design Tokens del Paso 16.18 | GMB Crush | Heredado del paso 16.18 | El framework dicta validar la tipografía. Valor heredado de Decisión de diseño en el Paso 16. | font-heading y font-body correctos |
| 18.27 · Paso-18 §9 Aud. Visual | Se decide validar Layout-Map de cada page type contra Paso 16.27–16.32 | GMB Crush | Heredado del paso 16.27–16.32 | El framework dicta validar el Layout-Map. Valores heredados de Decisión de diseño en el Paso 16. | 6 page types con layout correcto |
| 18.28 · Paso-18 §9 Aud. Visual | Se decide validar jerarquía Homepage (Servicios Core > AC) | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Heredado del Paso 15.05. | Servicios Core destacados, AC en posición secundaria |
| 18.29 · Paso-18 §9 Aud. Visual | Se decide validar GeoHub con contenido propio (no solo índice) | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Heredado del Paso 15.26. | GeoHub con introducción + contenido contextual + enlaces |

## Bloque 4 — Auditoría de Rastros de IA (6 criterios)

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 18.30 · Paso-18 §10 Aud. Rastros IA | Se decide validar README.md sin texto del starter kit | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Heredado del Paso 17.31. | README propio o eliminado |
| 18.31 · Paso-18 §10 Aud. Rastros IA | Se decide validar comentarios internos sin instrucciones de IA | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Heredado del Paso 17.32. | Sin comentarios "este componente hace X" |
| 18.32 · Paso-18 §10 Aud. Rastros IA | Se decide validar ausencia de meta generator en HTML | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Heredado del Paso 17.33. | HTML sin `<meta name="generator">` |
| 18.33 · Paso-18 §10 Aud. Rastros IA | Se decide ejecutar grep limpio de referencias a IA en todo el repo | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Heredado del Paso 17.34. | grep -ri "claude\|chatgpt\|openai\|anthropic" sin matches |
| 18.34 · Paso-18 §10 Aud. Rastros IA | Se decide validar package.json con nombre real del proyecto | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Heredado del Paso 17.35. | "name": "cerrajeros-madrid-24h" |
| 18.35 · Paso-18 §10 Aud. Rastros IA | Se decide validar commits sin referencias a IA | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Heredado del Paso 17.36. | git log limpio |

## Bloque 5 — Deploy a Cloudflare Pages

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 18.36 · Paso-18 §12.1 Setup | Se decide conectar el repositorio a Cloudflare Pages | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Stack canónico: hosting Cloudflare Pages. | github.com/cliente/cerrajeros-madrid-24h conectado a Cloudflare |
| 18.37 · Paso-18 §12.1 Setup | Se decide configurar build command `pnpm run build` | GMB Crush | Doctrina GMB Crush | El framework define esta regla. pnpm canónico (no npm). | Build command: `pnpm run build`, output dir: `dist` |
| 18.38 · Paso-18 §12.2 Dominio | Se decide conectar el dominio del Paso 1.02 a Cloudflare con SSL | GMB Crush | Heredado del paso 1.02 | El framework dicta conectar el dominio con SSL. Valor heredado del Paso 1.02 (Input humano). | https://www.cerrajerosmadrid24h.com con SSL activo |
| 18.39 · Paso-18 §12.2 Dominio | Se decide configurar redirección entre apex y www según versión canónica del Paso 1.03 | GMB Crush | Heredado del paso 1.03 | El framework dicta aplicar la redirección canónica. Valor heredado del Paso 1.03 (Input humano). | apex cerrajerosmadrid24h.com → www.cerrajerosmadrid24h.com |
| 18.40 · Paso-18 §12.3 Verificación | Se decide validar sitemap, robots.txt y URLs en producción | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Verificación post-deploy obligatoria. | sitemap-index.xml accesible, 200 OK en 29 URLs |
| 18.41 · Paso-18 §12.3 Verificación | Se decide registrar sitemap en Google Search Console tras deploy | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Sin GSC registrado, indexación lenta. | sitemap registrado en GSC con status Success |
