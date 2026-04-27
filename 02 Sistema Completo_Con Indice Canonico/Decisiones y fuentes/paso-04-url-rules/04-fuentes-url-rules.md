# Paso 4 — URL Rules

Fase 2 de trazabilidad: se añade fuente y funcionamiento a las decisiones del ejemplo **Cerrajeros Madrid 24h**.

Fuentes usadas:

```text
GMB Crush
Input humano
Geografía
Datos de búsqueda
Competidores
IA sin respaldo
```

---

## Bloque 1 — Dominio y formato general

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 4.01 · Paso-04 §7 Regla 1 Dominio canónico | Se decide usar HTTPS | GMB Crush | HTTPS es el estándar web canónico. GMB Crush lo exige para todas las URLs de producción. | https:// |
| 4.02 · Paso-04 §7 Regla 1 Dominio canónico | Se decide usar dominio canónico con www | IA sin respaldo | El dominio es de ejemplo y debe confirmarse con el cliente antes de producción. | https://www.cerrajerosmadrid24h.com |
| 4.03 · Paso-04 §8 Regla 2 Trailing slash | Se decide usar trailing slash | GMB Crush | Regla operativa de consistencia URL. Todas las URLs del sistema terminan en /. | Sí |

## Bloque 2 — Patrones URL principales

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 4.04 · Paso-04 §9 Regla 3 Homepage | Se decide que la Homepage use raíz | GMB Crush | La Homepage es el Root Entity Anchor. Su URL es siempre el root domain sin slug. | / |
| 4.05 · Paso-04 §10 Regla 4 Service Overview | Se decide que Service Overview use categoría + servicio | GMB Crush | El patrón /category/service/ es la regla fija de GMB Crush para Service Overview Pages. | /cerrajero/[service-slug]/ |
| 4.06 · Paso-04 §12 Regla 6 Main City LBS | Se decide que LBS use categoría + ciudad + servicio | GMB Crush | El patrón /category/city/service/ es la regla fija de GMB Crush para Location-Based Service Pages. | /cerrajero/madrid/[service-slug]/ |
| 4.07 · Paso-04 §13 Regla 7 Additional Category Page | Se decide que Additional Category use categoría + ciudad + servicio | GMB Crush | La Additional Category Page usa la misma estructura local que la LBS. | /cerrajero/madrid/duplicado-llaves/ |
| 4.08 · Paso-04 §11 Regla 5 Main City GeoHub | Se decide que GeoHub use ciudad | GMB Crush | El GeoHub es el contenedor de ciudad. Su URL es solo el slug de la ciudad. | /madrid/ |
| 4.09 · Paso-04 §14 Regla 8 GeoArticle | Se decide que GeoArticles usen ciudad + topic | GMB Crush | El GeoArticle usa ciudad + long-tail topic. No incluye el slug de servicio en la URL. | /madrid/[article-topic-slug]/ |

## Bloque 3 — URLs concretas de servicio

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 4.10–4.14 · Paso-04 §29 LBS con patrón fijo | Se deciden URLs locales para los 5 servicios | GMB Crush + IA sin respaldo | El patrón de URL es GMB Crush. Los servicios concretos están pendientes de validación con datos reales. | 5 URLs /cerrajero/madrid/[service]/ |

## Bloque 4 — Reglas anti-URL débil

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 4.15 · Paso-04 §17 Regla 11 No near-me | Se decide no usar near-me en URLs principales | GMB Crush | GMB Crush prohíbe URLs artificiales o débiles que no corresponden a intenciones reales de búsqueda. | No near-me |
| 4.16 · Paso-04 §18 Regla 12 No adjetivos vacíos | Se decide no usar adjetivos SEO vacíos en URLs | GMB Crush | GMB Crush prohíbe slugs manipulativos y no semánticos como best, cheap, top-rated. | No best, cheap, top-rated |
| 4.17 · Paso-04 §15 Regla 9 LCA no generan URLs | Se decide no crear URLs para Local Coverage Areas en la base | GMB Crush | Las LCA no generan URL por defecto. Solo generan URL si son Approved Expansion Areas. | No /almagro/, no /chamberi/, no /salamanca/ |
| 4.18 · Paso-04 §16 Regla 10 Approved Expansion URLs | Se decide que Approved Expansion Areas podrían generar URLs solo en expansión | GMB Crush | La expansión geográfica requiere aprobación explícita. No se activa en la fase base. | None in Phase 1 |
