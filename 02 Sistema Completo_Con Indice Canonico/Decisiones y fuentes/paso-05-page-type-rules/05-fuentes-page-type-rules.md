# Paso 5 — Page Type Rules

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

## Bloque 1 — Homepage

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 5.01 · Paso-05 §7 Homepage Root Entity Anchor | Se decide que la Homepage sea Root Entity Anchor | GMB Crush | El framework define la homepage como señal primaria de entidad. Es el punto de anclaje de toda la arquitectura. | / |
| 5.02 · Paso-05 §13 Homepage como Root Entity Anchor | Se decide que la Homepage ancle marca, servicio principal y ciudad | GMB Crush + Input humano | La estructura de anclaje es GMB Crush. La marca y la ciudad vienen del input del cliente. | Cerrajeros Madrid 24h + Cerrajero + Madrid |
| 5.03 · Paso-05 §7 Homepage Root Entity Anchor | Se decide que la Homepage incluya servicios core | GMB Crush + IA sin respaldo | GMB Crush requiere listar core services en la homepage. La lista concreta está pendiente de validación. | 5 servicios principales |
| 5.04 · Paso-05 §7 Homepage Root Entity Anchor | Se decide que la Homepage incluya NAP y CTA | GMB Crush + IA sin respaldo | NAP es obligatorio en la homepage para consistencia de entidad. El CTA concreto está pendiente de definir. | NAP + Llamar ahora |

## Bloque 2 — Service Overview Pages

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 5.05 · Paso-05 §8 Service Overview Page | Se decide que las Service Overview Pages sean no geolocalizadas | GMB Crush | GMB Crush establece que la Service Overview no debe incluir ciudad en la URL. Se diferencia así de la LBS. | /cerrajero/[service]/ |
| 5.06–5.10 · Paso-05 §14 Service Overview como pilar no local | Se deciden 5 Service Overview Pages concretas | GMB Crush + IA sin respaldo | El tipo y patrón de URL son GMB Crush. Los servicios concretos están pendientes de validación. | 5 URLs de servicio |

## Bloque 3 — Location-Based Service Pages

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 5.11 · Paso-05 §9 LBS Main City Converter | Se decide que las LBS sean convertidores locales | GMB Crush | GMB Crush establece que las LBS rankean consultas service in city. Son las páginas de conversión principal. | /cerrajero/madrid/[service]/ |
| 5.12 · Paso-05 §15 LBS como convertidor local | Se decide que Cerrajero urgente en Madrid sea LBS canónica | GMB Crush + IA sin respaldo | El patrón de URL es GMB Crush. El servicio canónico está pendiente de validación de mercado. | /cerrajero/madrid/cerrajero-urgente/ |
| 5.13 · Paso-05 §9 LBS Main City Converter | Se decide que las LBS incluyan servicio + ciudad en H1 y metadata | GMB Crush | Requisito de Location-Based Service Pages. El H1 y meta title deben incluir el par servicio + ciudad. | [Service] + Madrid |

## Bloque 4 — Additional Category, GeoHub y GeoArticles

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 5.14 · Paso-05 §10 Additional Category Page | Se decide que Duplicado de llaves sea Additional Category Page | GMB Crush + IA sin respaldo | GMB Crush exige soporte web para cada categoría adicional efectiva. La categoría concreta está pendiente de validación. | /cerrajero/madrid/duplicado-llaves/ |
| 5.15 · Paso-05 §11 GeoHub Main City Silo Container | Se decide que /madrid/ sea GeoHub | GMB Crush | El GeoHub es el city-level silo container. Agrupa todo el contenido local de la ciudad. | GeoHub de Madrid |
| 5.16 · Paso-05 §12 GeoArticle Semantic Booster | Se decide que GeoArticles sean boosters semánticos, no landings | GMB Crush | El framework define GeoArticles como semantic amplifiers. No son páginas de conversión directa. | 15 GeoArticles |
| 5.17 · Paso-05 §18 GeoArticle como booster semántico | Se decide que GeoArticles enlacen a su LBS y GeoHub | GMB Crush | El interlinking de GeoArticles hacia LBS y GeoHub es obligatorio en el framework. | GeoArticle → LBS + /madrid/ |

## Bloque 5 — Schema

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 5.18 · Paso-05 §7–§12 (por tipo de página) | Se decide asignar schema por tipo de página | GMB Crush | GMB Crush asigna un schema específico a cada tipo de página. La asignación se hace desde la matriz base. | Organization, WebSite, Service, LocalBusiness, CollectionPage, Article |
| 5.19 · Paso-05 §7 Homepage Root Entity Anchor | Se decide no usar sameAs de GBP hasta que exista el GBP | GMB Crush | No se inventa la URL del GBP ni se añade sameAs hasta que el GBP esté creado y verificado en el Paso 14. | N/A hasta Paso 14 |
