# Paso 10 — Producción en Fases

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

## Bloque 1 — Capacidad y herramientas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 10.01 · Paso-10 §21 Capacidad de publicación realista | Se define capacidad de publicación | IA sin respaldo | No consta capacidad real del equipo. El valor es una estimación genérica para el ejemplo. | 5 páginas por semana |
| 10.02 · Paso-10 §21 Capacidad de publicación realista | Se define equipo de producción | IA sin respaldo | Equipo operativo genérico. No confirmado para el cliente del ejemplo. | SEO + Writer + Developer |
| 10.03 · Paso-10 §21 Capacidad de publicación realista | Se define CMS | IA sin respaldo | No confirmado por el usuario. Debe validarse en ejecución real. | WordPress |
| 10.04 · Paso-10 §21 Capacidad de publicación realista | Se decide que se puede añadir schema | IA sin respaldo | Capacidad técnica no confirmada. Depende del CMS y del acceso del equipo. | Yes |
| 10.05 · Paso-10 §21 Capacidad de publicación realista | Se decide que se pueden editar enlaces internos | IA sin respaldo | Capacidad técnica no confirmada. Depende del CMS y del acceso del equipo. | Yes |
| 10.06 · Paso-10 §17 Phase 4 Optimization Loop | Se define tracking | GMB Crush + IA sin respaldo | GMB Crush recomienda las herramientas de tracking. La disponibilidad real de cada herramienta no está confirmada. | GMB Crush Geo Grid, Google Search Console, GA4 |

## Bloque 2 — Fases de producción

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 10.07 · Paso-10 §7 Fase 1 Entity Foundation | Se define Fase 1 | GMB Crush | GMB Crush define la Fase 1 como Entity Foundation: construcción inicial de entidad y servicios base. | Entity Foundation |
| 10.08 · Paso-10 §12 Calendario ejemplo | Se decide publicar Homepage, contacto, Service Overview y GeoHub en Fase 1 | GMB Crush + IA sin respaldo | El orden estructural es GMB Crush. La semana concreta depende de la capacidad del equipo, no validada. | Semana 1 |
| 10.09 · Paso-10 §8 Fase 2 Main City Conversion Layer | Se define Fase 2 | GMB Crush | GMB Crush define la Fase 2 como Main City Conversion Layer: LBS y categorías locales tras la foundation. | Main City Conversion Layer |
| 10.10 · Paso-10 §15 Phase 2 Main City Conversion | Se decide publicar LBS y Additional Category en Fase 2 | GMB Crush | Las páginas comerciales locales se publican después de las bases. Es la secuencia estándar del framework. | Páginas servicio + Madrid |
| 10.11 · Paso-10 §9 Fase 3 Main City Semantic Expansion | Se define Fase 3 | GMB Crush | GMB Crush define la Fase 3 como Semantic Expansion: GeoArticles después de las landings padre. | Semantic Expansion |
| 10.12 · Paso-10 §16 Phase 3 Semantic Expansion | Se decide publicar 15 GeoArticles en Fase 3 | GMB Crush + IA sin respaldo | La cantidad de GeoArticles (3 por servicio) es GMB Crush. Los temas concretos están pendientes de keyword research. | 3 por servicio |
| 10.13 · Paso-10 §10 Fase 4 Optimization Loop | Se define Fase 4 | GMB Crush | GMB Crush define la Fase 4 como Optimization Loop: revisión y optimización post-publicación. | Optimization Loop |
| 10.14 · Paso-10 §11 Fase 5 Optional Expansion Module | Se define Fase 5 | GMB Crush | GMB Crush define la Fase 5 como Optional Expansion Module: expansión geográfica después de validar zonas. | Optional Expansion Module |
| 10.15 · Paso-10 §23 No expansión prematura | Se decide no activar expansión inicial | GMB Crush | No hay Approved Expansion Areas en la fase base. La expansión solo se activa cuando las zonas candidatas pasan el test GEO. | None in Phase 1 |

## Bloque 3 — GBP después de la web

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 10.16 · Paso-10 §26 Fase 5 GBP Creation | Se decide crear el GBP después de publicar web base | Input humano + GMB Crush | El flujo web-first está acordado con el cliente y alineado con el framework GMB Crush. El GBP se crea en el Paso 14. | Paso 14 |
| 10.17 · Paso-10 §26 Fase 5 GBP Creation | Se decide que GBP no se cree antes de páginas core | Input humano + GMB Crush | Crear el GBP antes de la web conectaría el perfil a una web vacía o incompleta, lo que perjudica la señal de entidad. | Web-first |
