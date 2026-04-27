# Paso 2 — Fórmula Maestra de Arquitectura

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

## Bloque 1 — Alcance de la fórmula base

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 2.01 · Paso-02 §21 Main City como único multiplicador base | Se decide que la fórmula base se construye sobre una sola Main City | GMB Crush + Input humano | GMB Crush establece que la arquitectura base usa una sola ciudad como multiplicador. Madrid viene de la dirección aportada por el cliente. | Madrid |
| 2.02 · Paso-02 §8 Regla 1 | Se decide que las Local Coverage Areas no multiplican páginas por defecto | GMB Crush | GMB Crush establece que barrios y zonas se usan como señales GEO, no como URLs. Las páginas de zona requieren expansión aprobada explícitamente. | LCA no generan URLs base |
| 2.03 · Paso-02 §17 Optional Expansion Formula | Se decide que las Approved Expansion Areas no entran en la fórmula inicial | GMB Crush | La expansión geográfica es opcional y posterior a la base. Se activa solo cuando hay Approved Expansion Areas validadas. | None in Phase 1 |

## Bloque 2 — Servicios incluidos en el cálculo

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 2.04 · Paso-02 §19 Conteo de servicios core | Se define el número de servicios principales usados en la fórmula | IA sin respaldo | El número depende de la lista de servicios del Paso 1, aún pendiente de validación con input/datos/competidores. | S = 5 |
| 2.05 · Paso-02 §9 Regla 2 Variable S | Se incluye Cerrajero urgente en el cálculo | IA sin respaldo | Servicio plausible pero no confirmado con input del cliente, datos de búsqueda ni análisis de competencia. | Cerrajero urgente |
| 2.06 · Paso-02 §9 Regla 2 Variable S | Se incluye Apertura de puertas en el cálculo | IA sin respaldo | Servicio típico de cerrajería pero no confirmado con input, datos ni competencia. | Apertura de puertas |
| 2.07 · Paso-02 §9 Regla 2 Variable S | Se incluye Cambio de cerraduras en el cálculo | IA sin respaldo | Servicio típico de cerrajería pero no confirmado con input, datos ni competencia. | Cambio de cerraduras |
| 2.08 · Paso-02 §9 Regla 2 Variable S | Se incluye Cambio de bombines en el cálculo | IA sin respaldo | Servicio típico de cerrajería pero no confirmado con input, datos ni competencia. | Cambio de bombines |
| 2.09 · Paso-02 §9 Regla 2 Variable S | Se incluye Instalación de cerraduras de seguridad en el cálculo | IA sin respaldo | Servicio típico de cerrajería pero no confirmado con input, datos ni competencia. | Instalación de cerraduras de seguridad |

## Bloque 3 — Páginas generadas por la fórmula

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 2.10 · Paso-02 §8 Regla 1 | Se decide crear una Homepage | GMB Crush | La Homepage es el Root Entity Anchor obligatorio de toda arquitectura GMB Crush. Es parte fija de la fórmula. | 1 Homepage |
| 2.11 · Paso-02 §9 Regla 2 Variable S | Se decide crear una Service Overview Page por cada servicio principal | GMB Crush + IA sin respaldo | GMB Crush establece una SOP por servicio. El número concreto depende de los servicios pendientes de validación. | 5 Service Overview Pages |
| 2.12 · Paso-02 §8 Regla 1 | Se decide crear un GeoHub para la Main City | GMB Crush | El GeoHub de ciudad es el contenedor local obligatorio en la arquitectura GMB Crush. | 1 GeoHub para Madrid |
| 2.13 · Paso-02 §8 Regla 1 | Se decide crear una LBS por cada servicio principal en Madrid | GMB Crush + IA sin respaldo | GMB Crush establece una LBS por combinación servicio × ciudad. El número depende de servicios pendientes. | 5 LBS |
| 2.14 · Paso-02 §20 Conteo de categorías adicionales efectivas | Se decide crear una Additional Category Page para la categoría adicional efectiva | GMB Crush + IA sin respaldo | GMB Crush exige soporte web para cada categoría adicional efectiva. La categoría concreta está pendiente de validación. | 1 Additional Category Page |

## Bloque 4 — Categorías adicionales efectivas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 2.15 · Paso-02 §20 Conteo de categorías adicionales efectivas | Se decide que Servicio de cerrajería de urgencia no suma como categoría adicional separada | GMB Crush | GMB Crush establece que si una categoría adicional ya está cubierta por un servicio core, no genera página propia. Evita duplicar intenciones. | Cubierta por Cerrajero urgente |
| 2.16 · Paso-02 §20 Conteo de categorías adicionales efectivas | Se decide que Servicio de duplicado de llaves cuenta como categoría adicional efectiva | GMB Crush + IA sin respaldo | La lógica de clasificación es GMB Crush. La categoría concreta no está validada con datos reales. | A = 1 |

## Bloque 5 — GeoArticles

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 2.17 · Paso-02 §22 GeoArticles por servicio | Se decide usar 3 GeoArticles por servicio principal | GMB Crush | El GeoArticle framework establece 3 ideas por Service × City pair. Es una regla fija del sistema. | G = 3 |
| 2.18 · Paso-02 §22 GeoArticles por servicio | Se decide calcular GeoArticles como G × S | GMB Crush + IA sin respaldo | La fórmula es GMB Crush. S depende de los servicios pendientes de validación. | 3 × 5 |
| 2.19 · Paso-02 §23 Fórmula base completa | Se calcula el número total de GeoArticles | GMB Crush + IA sin respaldo | Deriva de G=3 y S=5. El resultado es correcto si S=5 se valida. | 15 GeoArticles |
| 2.20 · Paso-02 §22 GeoArticles por servicio | Se decide que los GeoArticles se generan para Madrid, no para cada LCA | GMB Crush | GeoArticles son servicio + ciudad + long-tail. Las LCA no multiplican URLs de GeoArticles. | 15 GeoArticles para Madrid |

## Bloque 6 — Total de páginas SEO base

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 2.21 · Paso-02 §23 Fórmula base completa | Se calcula el bloque de Homepage | GMB Crush | Parte fija de la arquitectura. Siempre es 1. | 1 página |
| 2.22 · Paso-02 §23 Fórmula base completa | Se calcula el bloque de Service Overview Pages | GMB Crush + IA sin respaldo | Depende del número de servicios validados. | 5 páginas |
| 2.23 · Paso-02 §23 Fórmula base completa | Se calcula el bloque de GeoHub | GMB Crush | Un GeoHub por Main City. Siempre es 1 en la base. | 1 página |
| 2.24 · Paso-02 §23 Fórmula base completa | Se calcula el bloque de LBS | GMB Crush + IA sin respaldo | Depende del número de servicios validados. | 5 páginas |
| 2.25 · Paso-02 §23 Fórmula base completa | Se calcula el bloque de Additional Category Pages | GMB Crush + IA sin respaldo | Depende de la categoría adicional efectiva pendiente de validación. | 1 página |
| 2.26 · Paso-02 §23 Fórmula base completa | Se calcula el bloque de GeoArticles | GMB Crush + IA sin respaldo | Depende de servicios y temas pendientes de keyword research. | 15 páginas |
| 2.27 · Paso-02 §28 Resultado final verificable | Se calcula el total de páginas SEO base | GMB Crush + IA sin respaldo | La suma es correcta si se aceptan S=5, A=1 y G=3. Todos los componentes variables están pendientes de validación. | 28 páginas SEO base |
| 2.28 · Paso-02 §8 Regla 1 | Se decide que /contacto/ queda fuera del inventario SEO base | GMB Crush | Contacto es página operativa, no uno de los 6 tipos SEO principales de la arquitectura GMB Crush. | Página auxiliar |
