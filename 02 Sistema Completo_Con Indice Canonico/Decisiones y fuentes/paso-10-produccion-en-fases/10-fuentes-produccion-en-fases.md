# Paso 10 — Producción en Fases

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

## Bloque 1 — Capacidad y herramientas

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 10.01 | Se define capacidad de publicación | 5 páginas por semana | IA sin respaldo | No consta capacidad real del equipo. | Pendiente de validación |
| 10.02 | Se define equipo de producción | SEO + Writer + Developer | IA sin respaldo | Equipo operativo genérico, no confirmado. | Pendiente de validación |
| 10.03 | Se define CMS | WordPress | IA sin respaldo | No confirmado por el usuario. | Pendiente de validación |
| 10.04 | Se decide que se puede añadir schema | Yes | IA sin respaldo | Capacidad técnica no confirmada. | Pendiente de validación |
| 10.05 | Se decide que se pueden editar enlaces internos | Yes | IA sin respaldo | Capacidad técnica no confirmada. | Pendiente de validación |
| 10.06 | Se define tracking | GMB Crush Geo Grid, Google Search Console, GA4 | GMB Crush + IA sin respaldo | GMB Crush recomienda tracking; disponibilidad de herramientas no confirmada. | Parcialmente validada |

## Bloque 2 — Fases de producción

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 10.07 | Se define Fase 1 | Entity Foundation | GMB Crush | Construcción inicial de entidad y servicios base. | Validada |
| 10.08 | Se decide publicar Homepage, contacto, Service Overview y GeoHub en Fase 1 | Semana 1 | GMB Crush + IA sin respaldo | Orden estructural correcto; semana concreta depende de capacidad no validada. | Parcialmente validada |
| 10.09 | Se define Fase 2 | Main City Conversion Layer | GMB Crush | LBS y categorías locales tras foundation. | Validada |
| 10.10 | Se decide publicar LBS y Additional Category en Fase 2 | Páginas servicio + Madrid | GMB Crush | Páginas comerciales locales después de bases. | Validada |
| 10.11 | Se define Fase 3 | Semantic Expansion | GMB Crush | GeoArticles después de landings padre. | Validada |
| 10.12 | Se decide publicar 15 GeoArticles en Fase 3 | 3 por servicio | GMB Crush + IA sin respaldo | Cantidad GMB; temas pendientes de keyword research. | Parcialmente validada |
| 10.13 | Se define Fase 4 | Optimization Loop | GMB Crush | Optimización post-publicación. | Validada |
| 10.14 | Se define Fase 5 | Optional Expansion Module | GMB Crush | Expansión después de validar zonas. | Validada |
| 10.15 | Se decide no activar expansión inicial | None in Phase 1 | GMB Crush | No hay Approved Expansion Areas. | Validada |

## Bloque 3 — GBP después de la web

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 10.16 | Se decide crear el GBP después de publicar web base | Paso 14 | Input humano + GMB Crush | Flujo web-first acordado y alineado con GBP después. | Validada |
| 10.17 | Se decide que GBP no se cree antes de páginas core | Web-first | Input humano + GMB Crush | Evita conectar GBP a una web vacía o incompleta. | Validada |

