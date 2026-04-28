# Paso 3 — Matriz Base

Fase 2 de trazabilidad: se añade fuente y funcionamiento a las decisiones del ejemplo **Cerrajeros Madrid 24h**.

Fuentes usadas (jerarquía de prioridad):

```text
IA sin respaldo
IA heredada
Datos de búsqueda
Competidores
GMB Crush
Input humano
```

---

## Bloque 1 — Estructura de la matriz

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.01 · Paso-03 §7 URL Matrix | Se decide crear una matriz operativa para controlar las URLs | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. La URL Matrix es la fuente de verdad de la arquitectura. | URL Matrix |
| 3.02 · Paso-03 §7 URL Matrix | Se decide que cada página tenga un ID único | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Los IDs canónicos son HP, SO, GH, LBS, AC, GA. | HP, SO, GH, LBS, AC, GA |
| 3.03 · Paso-03 §7 URL Matrix | Se decide incluir columnas de producción | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las 20 columnas canónicas incluyen URL, H1, Meta Title, Schema, Priority, Phase, Status. | URL, H1, Meta Title, Schema, Priority, Phase, Status |

## Bloque 2 — Homepage y páginas auxiliares

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.04 · Paso-03 §7 URL Matrix | Se decide incluir la Homepage en la matriz | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. | HP-001 |
| 3.05 · Paso-03 §7 URL Matrix | Se decide que la Homepage use la raíz | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. | / |
| 3.06 · Paso-03 §7 URL Matrix | Se decide incluir página de contacto como auxiliar | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. La página de contacto es auxiliar, fuera del inventario SEO base. | /contacto/ |

## Bloque 3 — Service Overview Pages

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.07 · Paso-03 §7 URL Matrix | Se decide crear Service Overview para Cerrajero urgente | IA heredada (paso 1.34) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/cerrajero-urgente/ |
| 3.08 · Paso-03 §7 URL Matrix | Se decide crear Service Overview para Apertura de puertas | IA heredada (paso 1.35) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/apertura-puertas/ |
| 3.09 · Paso-03 §7 URL Matrix | Se decide crear Service Overview para Cambio de cerraduras | IA heredada (paso 1.36) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/cambio-cerraduras/ |
| 3.10 · Paso-03 §7 URL Matrix | Se decide crear Service Overview para Cambio de bombines | IA heredada (paso 1.37) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/cambio-bombines/ |
| 3.11 · Paso-03 §7 URL Matrix | Se decide crear Service Overview para Instalación de cerraduras de seguridad | IA heredada (paso 1.38) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/instalacion-cerraduras-seguridad/ |

## Bloque 4 — GeoHub y Location-Based Service Pages

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.12 · Paso-03 §7 URL Matrix | Se decide crear el GeoHub principal de Madrid | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. Madrid heredado del paso 1.20. El patrón /[city]/ es GMB Crush. | /madrid/ |
| 3.13 · Paso-03 §7 URL Matrix | Se decide crear LBS de Cerrajero urgente en Madrid | IA heredada (paso 1.34) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/madrid/cerrajero-urgente/ |
| 3.14 · Paso-03 §7 URL Matrix | Se decide crear LBS de Apertura de puertas en Madrid | IA heredada (paso 1.35) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/madrid/apertura-puertas/ |
| 3.15 · Paso-03 §7 URL Matrix | Se decide crear LBS de Cambio de cerraduras en Madrid | IA heredada (paso 1.36) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/madrid/cambio-cerraduras/ |
| 3.16 · Paso-03 §7 URL Matrix | Se decide crear LBS de Cambio de bombines en Madrid | IA heredada (paso 1.37) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/madrid/cambio-bombines/ |
| 3.17 · Paso-03 §7 URL Matrix | Se decide crear LBS de Instalación de cerraduras de seguridad en Madrid | IA heredada (paso 1.38) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/madrid/instalacion-cerraduras-seguridad/ |

## Bloque 5 — Additional Category Page

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.18 · Paso-03 §7 URL Matrix | Se decide crear página de duplicado de llaves en Madrid | IA heredada (paso 1.40) | El valor se hereda de una decisión IA sin respaldo en el paso indicado. Esta decisión se cura cuando se cierra la decisión origen. El patrón URL es GMB Crush. | /cerrajero/madrid/duplicado-llaves/ |

## Bloque 6 — GeoArticles

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.19 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle de coste de cerrajero urgente | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. El topic concreto requiere keyword research. | /madrid/cuanto-cuesta-un-cerrajero-urgente/ |
| 3.20 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre no poder entrar en casa | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/que-hacer-si-no-puedes-entrar-casa/ |
| 3.21 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre tiempo de llegada | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/cuanto-tarda-un-cerrajero/ |
| 3.22 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre coste de apertura de puertas | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/cuanto-cuesta-abrir-una-puerta/ |
| 3.23 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre llaves dentro | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/que-hacer-si-te-dejas-las-llaves-dentro/ |
| 3.24 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre apertura sin romper cerradura | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/apertura-de-puertas-sin-romper-cerradura/ |
| 3.25 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre cuándo cambiar cerradura | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/cuando-cambiar-la-cerradura-de-casa/ |
| 3.26 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre cambio tras perder llaves | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/cambio-de-cerradura-tras-perder-llaves/ |
| 3.27 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre cerradura nueva o reparación | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/cerradura-nueva-o-reparacion/ |
| 3.28 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre cuándo cambiar bombín | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/cuando-cambiar-el-bombin/ |
| 3.29 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre bombín antibumping | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/bombin-antibumping-madrid/ |
| 3.30 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre cambio de bombín sin cambiar cerradura | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/cambio-de-bombin-sin-cambiar-cerradura/ |
| 3.31 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre cerraduras de seguridad para viviendas | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/mejores-cerraduras-de-seguridad-para-viviendas/ |
| 3.32 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre cerraduras de seguridad para comunidades | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/cerraduras-de-seguridad-para-comunidades/ |
| 3.33 · Paso-03 §7 URL Matrix | Se decide crear GeoArticle sobre cerradura de seguridad en puerta blindada | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | /madrid/instalar-cerradura-de-seguridad-en-puerta-blindada/ |

## Bloque 7 — Tratamiento de Local Coverage Areas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 3.34 · Paso-03 §7 URL Matrix | Se decide que las Local Coverage Areas aparezcan como notas o campos de contenido | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las LCA se usan como señales GEO en contenido. | Almagro, Chamberí, Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad |
| 3.35 · Paso-03 §7 URL Matrix | Se decide que no haya filas URL para Local Coverage Areas | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las LCA no generan URLs por defecto. | No /almagro/, no /chamberi/, no /salamanca/ |
