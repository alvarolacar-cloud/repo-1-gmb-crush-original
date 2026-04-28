# Paso 5 — Page Type Rules

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

## Bloque 1 — Homepage

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 5.01 · Paso-05 §7 Homepage | Se decide que la Homepage sea Root Entity Anchor | GMB Crush | Doctrina GMB Crush | El framework define el rol canónico de la Homepage. | / |
| 5.02 · Paso-05 §7 Homepage | Se decide que la Homepage ancle marca, servicio principal y ciudad | GMB Crush | Doctrina GMB Crush | El framework define el patrón H1: Brand + Primary Service + Main City. | Cerrajeros Madrid 24h + Cerrajero + Madrid |
| 5.03 · Paso-05 §7 Homepage | Se decide que la Homepage incluya servicios core | GMB Crush | Doctrina GMB Crush | El framework dicta mostrar los servicios principales en Homepage. | 5 servicios principales |
| 5.04 · Paso-05 §7 Homepage | Se decide que la Homepage incluya NAP y CTA | GMB Crush | Doctrina GMB Crush | El framework dicta NAP visible y CTA claro en Homepage. | NAP + Llamar ahora |

## Bloque 2 — Service Overview Pages

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 5.05 · Paso-05 §8 Service Overview | Se decide que las Service Overview Pages sean no geolocalizadas | GMB Crush | Doctrina GMB Crush | El framework define las SO como pillars temáticos sin ciudad. | /cerrajero/[service]/ |
| 5.06 · Paso-05 §8 Service Overview | Se decide que Cerrajero urgente tenga Service Overview Page | GMB Crush | Heredado del paso 1.34 | El framework dicta "1 SO por servicio core". Servicio heredado del paso 1.34. | /cerrajero/cerrajero-urgente/ |
| 5.07 · Paso-05 §8 Service Overview | Se decide que Apertura de puertas tenga Service Overview Page | GMB Crush | Heredado del paso 1.35 | El framework dicta "1 SO por servicio core". Servicio heredado del paso 1.35. | /cerrajero/apertura-puertas/ |
| 5.08 · Paso-05 §8 Service Overview | Se decide que Cambio de cerraduras tenga Service Overview Page | GMB Crush | Heredado del paso 1.36 | El framework dicta "1 SO por servicio core". Servicio heredado del paso 1.36. | /cerrajero/cambio-cerraduras/ |
| 5.09 · Paso-05 §8 Service Overview | Se decide que Cambio de bombines tenga Service Overview Page | GMB Crush | Heredado del paso 1.37 | El framework dicta "1 SO por servicio core". Servicio heredado del paso 1.37. | /cerrajero/cambio-bombines/ |
| 5.10 · Paso-05 §8 Service Overview | Se decide que Instalación de cerraduras de seguridad tenga Service Overview Page | GMB Crush | Heredado del paso 1.38 | El framework dicta "1 SO por servicio core". Servicio heredado del paso 1.38. | /cerrajero/instalacion-cerraduras-seguridad/ |

## Bloque 3 — Location-Based Service Pages

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 5.11 · Paso-05 §9 LBS | Se decide que las LBS sean convertidores locales | GMB Crush | Doctrina GMB Crush | El framework define las LBS como Main City Converter. | /cerrajero/madrid/[service]/ |
| 5.12 · Paso-05 §9 LBS | Se decide que Cerrajero urgente en Madrid sea LBS canónica | GMB Crush | Heredado del paso 1.34 | El framework define la estructura LBS canónica. Servicio heredado del paso 1.34. | /cerrajero/madrid/cerrajero-urgente/ |
| 5.13 · Paso-05 §9 LBS | Se decide que las LBS incluyan servicio + ciudad en H1 y metadata | GMB Crush | Doctrina GMB Crush | El framework define el patrón H1 LBS = [Service] + Main City. | [Service] + Madrid |

## Bloque 4 — Additional Category, GeoHub y GeoArticles

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 5.14 · Paso-05 §10 Additional Category | Se decide que Duplicado de llaves sea Additional Category Page | GMB Crush | Heredado del paso 1.18 | El framework define la regla "AC para categoría adicional efectiva". Categoría heredada del paso 1.18. | /cerrajero/madrid/duplicado-llaves/ |
| 5.15 · Paso-05 §11 GeoHub | Se decide que `/madrid/` sea GeoHub | GMB Crush | Doctrina GMB Crush | El framework define GeoHub = Main City Silo Container. | GeoHub de Madrid |
| 5.16 · Paso-05 §12 GeoArticle | Se decide que GeoArticles sean boosters semánticos, no landings | GMB Crush | Doctrina GMB Crush | El framework define GeoArticle = Semantic Booster, no convierte. | 15 GeoArticles |
| 5.17 · Paso-05 §12 GeoArticle | Se decide que GeoArticles enlacen a su LBS y GeoHub | GMB Crush | Doctrina GMB Crush | El framework dicta que cada GeoArticle apoya un LBS específico. | GeoArticle → LBS + /madrid/ |

## Bloque 5 — Schema

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 5.18 · Paso-05 §19 Schema | Se decide asignar schema por tipo de página | GMB Crush | Doctrina GMB Crush | El framework define el mapa schema canónico por page type. | Organization, WebSite, Service, LocalBusiness, CollectionPage, Article |
| 5.19 · Paso-05 §19 Schema | Se decide no usar `sameAs` de GBP hasta que exista el GBP | GMB Crush | Doctrina GMB Crush | El framework prohíbe inventar GBP URL ni sameAs antes del Paso 14. | N/A hasta Paso 14 |
