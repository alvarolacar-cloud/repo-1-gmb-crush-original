# Paso 5 — Page Type Rules

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

## Bloque 1 — Homepage

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 5.01 | Se decide que la Homepage sea Root Entity Anchor | / | GMB Crush | El framework define la homepage como señal primaria de entidad. | Validada |
| 5.02 | Se decide que la Homepage ancle marca, servicio principal y ciudad | Cerrajeros Madrid 24h + Cerrajero + Madrid | GMB Crush + Input humano | La estructura es GMB; marca/ciudad vienen del input. | Validada |
| 5.03 | Se decide que la Homepage incluya servicios core | 5 servicios principales | GMB Crush + IA sin respaldo | GMB pide core services; lista concreta pendiente de validación. | Parcialmente validada |
| 5.04 | Se decide que la Homepage incluya NAP y CTA | NAP + Llamar ahora | GMB Crush + IA sin respaldo | NAP es necesario; CTA concreto pendiente. | Parcialmente validada |

## Bloque 2 — Service Overview Pages

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 5.05 | Se decide que las Service Overview Pages sean no geolocalizadas | /cerrajero/[service]/ | GMB Crush | Service Overview no debe confundirse con Service in City. | Validada |
| 5.06-5.10 | Se deciden 5 Service Overview Pages concretas | 5 URLs de servicio | GMB Crush + IA sin respaldo | Tipo y patrón validado; servicios concretos pendientes. | Parcialmente validada |

## Bloque 3 — Location-Based Service Pages

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 5.11 | Se decide que las LBS sean convertidores locales | /cerrajero/madrid/[service]/ | GMB Crush | LBS rankea consultas service in city. | Validada |
| 5.12 | Se decide que Cerrajero urgente en Madrid sea LBS canónica | /cerrajero/madrid/cerrajero-urgente/ | GMB Crush + IA sin respaldo | URL pattern validado; servicio canónico pendiente de validación de mercado. | Parcialmente validada |
| 5.13 | Se decide que las LBS incluyan servicio + ciudad en H1 y metadata | [Service] + Madrid | GMB Crush | Requisito de Location-Based Service Pages. | Validada |

## Bloque 4 — Additional Category, GeoHub y GeoArticles

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 5.14 | Se decide que Duplicado de llaves sea Additional Category Page | /cerrajero/madrid/duplicado-llaves/ | GMB Crush + IA sin respaldo | GMB exige soporte para categorías; categoría concreta pendiente. | Parcialmente validada |
| 5.15 | Se decide que /madrid/ sea GeoHub | GeoHub de Madrid | GMB Crush | GeoHub es city-level silo container. | Validada |
| 5.16 | Se decide que GeoArticles sean boosters semánticos, no landings | 15 GeoArticles | GMB Crush | El framework define GeoArticles como semantic amplifiers. | Validada |
| 5.17 | Se decide que GeoArticles enlacen a su LBS y GeoHub | GeoArticle → LBS + /madrid/ | GMB Crush | Interlinking obligatorio de GeoArticles. | Validada |

## Bloque 5 — Schema

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 5.18 | Se decide asignar schema por tipo de página | Organization, WebSite, Service, LocalBusiness, CollectionPage, Article | GMB Crush | Schema por tipo está en la estructura GMB. | Validada |
| 5.19 | Se decide no usar sameAs de GBP hasta que exista el GBP | N/A hasta Paso 14 | GMB Crush | No se inventa GBP URL ni sameAs. | Validada |

