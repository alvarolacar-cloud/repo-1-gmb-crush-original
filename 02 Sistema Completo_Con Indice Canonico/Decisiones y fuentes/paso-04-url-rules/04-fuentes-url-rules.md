# Paso 4 — URL Rules

Fase 2 de trazabilidad: se añade fuente, justificación y estado a las decisiones del ejemplo **Cerrajeros Madrid 24h**.

Fuentes usadas:

```text
GMB Crush
Input humano
Geografía
Datos de búsqueda
Competidores
IA sin respaldo
```

Estados usados:

```text
Validada
Parcialmente validada
Pendiente de validación
IA sin respaldo
```

---

## Bloque 1 — Dominio y formato general

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 4.01 | Se decide usar HTTPS | https:// | GMB Crush | Estándar web/canónico para URLs de producción. | Validada |
| 4.02 | Se decide usar dominio canónico con www | https://www.cerrajerosmadrid24h.com | IA sin respaldo | El dominio es de ejemplo y debe confirmarse. | Pendiente de validación |
| 4.03 | Se decide usar trailing slash | Sí | GMB Crush | Regla operativa de consistencia URL. | Validada |

## Bloque 2 — Patrones URL principales

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 4.04 | Se decide que la Homepage use raíz | / | GMB Crush | Homepage root domain. | Validada |
| 4.05 | Se decide que Service Overview use categoría + servicio | /cerrajero/[service-slug]/ | GMB Crush | Service Overview usa /category/service/. | Validada |
| 4.06 | Se decide que LBS use categoría + ciudad + servicio | /cerrajero/madrid/[service-slug]/ | GMB Crush | Location-Based Service usa /category/city/service/. | Validada |
| 4.07 | Se decide que Additional Category use categoría + ciudad + servicio | /cerrajero/madrid/duplicado-llaves/ | GMB Crush | Additional Category Page usa estructura local por ciudad. | Validada |
| 4.08 | Se decide que GeoHub use ciudad | /madrid/ | GMB Crush | GeoHub es contenedor de ciudad. | Validada |
| 4.09 | Se decide que GeoArticles usen ciudad + topic | /madrid/[article-topic-slug]/ | GMB Crush | GeoArticle usa ciudad + long-tail topic. | Validada |

## Bloque 3 — URLs concretas de servicio

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 4.10-4.14 | Se deciden URLs locales para los 5 servicios | 5 URLs /cerrajero/madrid/[service]/ | GMB Crush + IA sin respaldo | Patrón validado; servicios pendientes de validación. | Parcialmente validada |

## Bloque 4 — Reglas anti-URL débil

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 4.15 | Se decide no usar near-me en URLs principales | No near-me | GMB Crush | Evita URLs artificiales o débiles. | Validada |
| 4.16 | Se decide no usar adjetivos SEO vacíos en URLs | No best, cheap, top-rated | GMB Crush | Evita slugs manipulativos y no semánticos. | Validada |
| 4.17 | Se decide no crear URLs para Local Coverage Areas en la base | No /almagro/, no /chamberi/, no /salamanca/ | GMB Crush | Las LCA no generan URL por defecto. | Validada |
| 4.18 | Se decide que Approved Expansion Areas podrían generar URLs solo en expansión | None in Phase 1 | GMB Crush | La expansión requiere aprobación. | Validada |

