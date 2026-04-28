# Paso 4 — URL Rules

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

## Bloque 1 — Dominio y formato general

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 4.01 · Paso-04 §7 Dominio canónico | Se decide usar HTTPS | GMB Crush | Doctrina GMB Crush | El framework define HTTPS como estándar para producción. | https:// |
| 4.02 · Paso-04 §7 Dominio canónico | Se decide usar dominio canónico con www | GMB Crush | Heredado del paso 1.03 | El framework exige una sola versión canónica. El dominio sale del paso 1.03. | https://www.cerrajerosmadrid24h.com |
| 4.03 · Paso-04 §8 Trailing slash | Se decide usar trailing slash | GMB Crush | Doctrina GMB Crush | El framework define decisión binaria uniforme en toda la web. | Sí |

## Bloque 2 — Patrones URL principales

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 4.04 · Paso-04 §9 Homepage | Se decide que la Homepage use raíz | GMB Crush | Doctrina GMB Crush | El framework define la regla. | / |
| 4.05 · Paso-04 §10 Service Overview | Se decide que Service Overview use categoría + servicio | GMB Crush | Doctrina GMB Crush | El framework define la regla. | /cerrajero/[service-slug]/ |
| 4.06 · Paso-04 §12 LBS | Se decide que LBS use categoría + ciudad + servicio | GMB Crush | Doctrina GMB Crush | El framework define la regla. | /cerrajero/madrid/[service-slug]/ |
| 4.07 · Paso-04 §13 Additional Category | Se decide que Additional Category use categoría + ciudad + servicio | GMB Crush | Doctrina GMB Crush | El framework define la regla. | /cerrajero/madrid/duplicado-llaves/ |
| 4.08 · Paso-04 §11 GeoHub | Se decide que GeoHub use ciudad | GMB Crush | Doctrina GMB Crush | El framework define la regla. | /madrid/ |
| 4.09 · Paso-04 §14 GeoArticle | Se decide que GeoArticles usen ciudad + topic | GMB Crush | Doctrina GMB Crush | El framework define la regla. | /madrid/[article-topic-slug]/ |

## Bloque 3 — URLs concretas de servicio

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 4.10 · Paso-04 §12 LBS | Se decide crear URL local de Cerrajero urgente | GMB Crush | Heredado del paso 1.34 | El framework define el patrón URL. El slug del servicio sale del paso 1.34. | /cerrajero/madrid/cerrajero-urgente/ |
| 4.11 · Paso-04 §12 LBS | Se decide crear URL local de Apertura de puertas | GMB Crush | Heredado del paso 1.35 | El framework define el patrón URL. El slug del servicio sale del paso 1.35. | /cerrajero/madrid/apertura-puertas/ |
| 4.12 · Paso-04 §12 LBS | Se decide crear URL local de Cambio de cerraduras | GMB Crush | Heredado del paso 1.36 | El framework define el patrón URL. El slug del servicio sale del paso 1.36. | /cerrajero/madrid/cambio-cerraduras/ |
| 4.13 · Paso-04 §12 LBS | Se decide crear URL local de Cambio de bombines | GMB Crush | Heredado del paso 1.37 | El framework define el patrón URL. El slug del servicio sale del paso 1.37. | /cerrajero/madrid/cambio-bombines/ |
| 4.14 · Paso-04 §12 LBS | Se decide crear URL local de Instalación de cerraduras de seguridad | GMB Crush | Heredado del paso 1.38 | El framework define el patrón URL. El slug del servicio sale del paso 1.38. | /cerrajero/madrid/instalacion-cerraduras-seguridad/ |

## Bloque 4 — Reglas anti-URL débil

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 4.15 · Paso-04 §19 Slugs | Se decide no usar `near-me` en URLs principales | GMB Crush | Doctrina GMB Crush | El framework define la regla anti-URL artificial. | No se usa near-me |
| 4.16 · Paso-04 §19 Slugs | Se decide no usar adjetivos SEO vacíos en URLs | GMB Crush | Doctrina GMB Crush | El framework define la regla anti-slug manipulativo. | No usar best, cheap, top-rated |
| 4.17 · Paso-04 §15 Local Coverage URLs | Se decide no crear URLs para Local Coverage Areas en la base | GMB Crush | Doctrina GMB Crush | El framework define la regla — las LCA no generan URLs por defecto. | No /almagro/, no /chamberi/, no /salamanca/ |
| 4.18 · Paso-04 §16 Approved Expansion | Se decide que Approved Expansion Areas podrían generar URLs solo en expansión | GMB Crush | Doctrina GMB Crush | El framework define la regla — la expansión requiere aprobación explícita. | None in Phase 1 |
