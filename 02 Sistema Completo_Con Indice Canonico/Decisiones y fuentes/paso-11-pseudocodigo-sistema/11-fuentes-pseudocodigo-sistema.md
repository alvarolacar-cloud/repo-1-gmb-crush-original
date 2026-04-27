# Paso 11 — Pseudocódigo del Sistema

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

## Bloque 1 — Inputs, slugs y categorías

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 11.01 · Paso-11 §7 Load inputs | Se decide cargar inputs base | GMB Crush | El sistema requiere cargar todos los inputs antes de generar la arquitectura. Sin inputs validados no se genera nada. | Business name, URL, NAP, Main City, servicios, LCA, GBP status |
| 11.02 · Paso-11 §8 Normalize slugs | Se decide normalizar slugs | GMB Crush | Las URLs limpias requieren normalización de texto: minúsculas, sin acentos, guiones en lugar de espacios. | Cerrajero urgente → cerrajero-urgente |
| 11.03 · Paso-11 §9 Validate categories | Se decide validar categorías adicionales | GMB Crush | El sistema valida si cada categoría adicional ya tiene página o necesita una nueva. Evita duplicados. | Cubierta / necesita página |

## Bloque 2 — Generación base

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 11.04 · Paso-11 §10 Generate homepage | Se decide generar Homepage | GMB Crush | La Homepage es el Root Entity Anchor. Siempre es la primera página generada. | HP-001 |
| 11.05 · Paso-11 §11 Generate Service Overview Pages | Se decide generar Service Overview Pages | GMB Crush + IA sin respaldo | El patrón de generación es GMB Crush. La lista concreta de servicios está pendiente de validación. | 5 páginas |
| 11.06 · Paso-11 §12 Generate Main City GeoHub | Se decide generar GeoHub de Madrid | GMB Crush + Input humano | El GeoHub de la Main City es obligatorio. Madrid viene del input del cliente. | /madrid/ |
| 11.07 · Paso-11 §13 Generate páginas de servicio en Main City | Se decide generar LBS de Madrid | GMB Crush + IA sin respaldo | El patrón de generación es GMB Crush. Los servicios concretos están pendientes de validación. | 5 páginas |
| 11.08 · Paso-11 §14 Generate páginas de categoría adicional | Se decide generar Additional Category Page efectiva | GMB Crush + IA sin respaldo | El tipo de página es correcto. La categoría concreta está pendiente de validación. | /cerrajero/madrid/duplicado-llaves/ |
| 11.09 · Paso-11 §15 Generate GeoArticles | Se decide generar GeoArticles | GMB Crush + IA sin respaldo | La cantidad (3 por servicio = 15) es GMB Crush. Los temas concretos están pendientes de keyword research. | 15 artículos |

## Bloque 3 — LCA y expansión

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 11.10 · Paso-11 §16 Use Local Coverage Areas | Se decide inyectar LCA en contenido y schema | GMB Crush + Geografía | Las LCA directas (Almagro, Chamberí) están validadas por el NAP. Las candidatas requieren test GEO antes de inyectarse. | LCA como señales GEO |
| 11.11 · Paso-11 §17 Generate expansion only if approved | Se decide no generar expansión si no está aprobada | GMB Crush | No se crean URLs fuera de la Main City sin aprobación explícita. La expansión es un módulo opcional posterior. | Approved Expansion Areas: None |

## Bloque 4 — Enlaces, prioridad, QA y outputs

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 11.12 · Paso-11 §18 Assign internal links | Se decide asignar enlaces internos por tipo | GMB Crush | La jerarquía de enlaces del framework se asigna automáticamente según el tipo de página. | Internal Linking Map |
| 11.13 · Paso-11 §19 Score priority | Se decide calcular prioridad por página | GMB Crush | El orden de producción requiere scoring previo. Cada página recibe su Priority Score antes de producción. | Priority Score |
| 11.14 · Paso-11 §7 Load inputs | Se decide comprobar dependencias | GMB Crush | El sistema verifica que las páginas padre existan antes de generar páginas hijas. Evita páginas huérfanas. | LBS requiere Service Overview + GeoHub |
| 11.15 · Paso-11 §6 Cuerpo operativo | Se decide ejecutar QA antes de publicar | GMB Crush | No se publica ninguna URL sin pasar el QA Gate. El pseudocódigo incluye el check de QA como paso obligatorio. | QA Matrix |
| 11.16 · Paso-11 §6 Cuerpo operativo | Se decide producir matrices finales | GMB Crush | El output operativo del sistema son matrices estructuradas, no contenido suelto. | URL Matrix, Internal Linking Matrix, Schema Map, Priority Score, Publishing Plan, QA Matrix |
