# Paso 16 — Extracción de Diseño y Layout

Fase 2 de trazabilidad del sistema GMB Crush.

Fuentes permitidas:

```text
GMB Crush
Input humano
Input humano + GMB Crush
Datos de búsqueda
Competidores
IA sin respaldo
GMB Crush + IA sin respaldo
Input humano + IA sin respaldo
IA heredada (paso X.YY)
Decisión de diseño
```

---

## Bloque 1 — CSS Base de la web de referencia

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 16.01 · Paso-16 §7.1 CSS Base | Se decide la web de referencia para extracción visual | Input humano | El cliente aporta este dato directamente. El sistema lo recoge sin transformación. La elección debe estar aprobada antes de Fase 1. | Web de referencia aprobada por Cerrajeros Madrid 24h (pendiente de definir cuál) |
| 16.02 · Paso-16 §7.1 CSS Base | Se decide el color primario | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Está cerrada salvo que el cliente solicite cambio. Extraído de la web de referencia. | primary: [HEX extraído de referencia] |
| 16.03 · Paso-16 §7.1 CSS Base | Se decide el color secundario | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Extraído de la web de referencia. | secondary: [HEX extraído de referencia] |
| 16.04 · Paso-16 §7.1 CSS Base | Se decide el color acento | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Extraído de la web de referencia. | accent: [HEX extraído de referencia] |
| 16.05 · Paso-16 §7.1 CSS Base | Se decide la paleta de fondo y texto | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Extraída de la web de referencia. Validada con contraste WCAG AA. | bg-light, bg-dark, text-primary, text-light, text-secondary [HEX extraídos] |
| 16.06 · Paso-16 §7.1 CSS Base | Se decide la tipografía heading | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Extraída de la web de referencia. | font-heading: [FONT_FAMILY identificada] |
| 16.07 · Paso-16 §7.1 CSS Base | Se decide la tipografía body | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Extraída de la web de referencia. | font-body: [FONT_FAMILY identificada] |
| 16.08 · Paso-16 §7.1 CSS Base | Se decide la jerarquía de tamaños tipográficos | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. H1, H2, H3, body extraídos de la web de referencia. | H1 [PX], H2 [PX], H3 [PX], body [PX] |
| 16.09 · Paso-16 §7.1 CSS Base | Se decide los radius de botones, cards e inputs | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Extraídos de la web de referencia. | btn-radius, card-radius, input-radius [PX] |
| 16.10 · Paso-16 §7.1 CSS Base | Se decide el box-shadow base de cards | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Extraído de la web de referencia. | card-shadow: [CSS_VALUE] |

## Bloque 2 — Layout y Estructura por Sección

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 16.11 · Paso-16 §7.2 Layout Homepage | Se decide el layout de cada sección de la Homepage | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Cruzado con las 6 secciones del Paso 15 §9.1. | 6 layouts uno por sección Homepage |
| 16.12 · Paso-16 §7.2 Layout SO | Se decide el layout de cada sección de las Service Overview Pages | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Cruzado con las 7 secciones del Paso 15 §10.1. | 7 layouts uno por sección SO |
| 16.13 · Paso-16 §7.2 Layout LBS | Se decide el layout de cada sección de las Location-Based Service Pages | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Cruzado con las 8 secciones del Paso 15 §11.1. | 8 layouts uno por sección LBS |
| 16.14 · Paso-16 §7.2 Layout AC | Se decide el layout de cada sección de la Additional Category Page | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Cruzado con las 6 secciones del Paso 15 §12.1. | 6 layouts uno por sección AC |
| 16.15 · Paso-16 §7.2 Layout GeoHub | Se decide el layout de cada sección del GeoHub | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Cruzado con las 8 secciones del Paso 15 §13.1. | 8 layouts uno por sección GeoHub |
| 16.16 · Paso-16 §7.2 Layout GeoArticle | Se decide el layout de cada sección del GeoArticle | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Cruzado con las 6 secciones del Paso 15 §14.1. | 6 layouts uno por sección GeoArticle |

## Bloque 3 — Design Tokens en Tailwind

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 16.17 · Paso-16 §8.2 Design Tokens | Se decide convertir los CSS extraídos a tokens Tailwind | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Tailwind como sistema de tokens canónico del stack (Paso 17). | tailwind.config.mjs con tokens completos |
| 16.18 · Paso-16 §8.2.1 Tipografía | Se decide los tokens de tipografía Tailwind | Decisión de diseño | El operador o agencia toma esta decisión basándose en los CSS extraídos en §7.1 y la nomenclatura Tailwind. | font-heading, font-body con valores definitivos |
| 16.19 · Paso-16 §8.2.2 Colores | Se decide los tokens de colores Tailwind | Decisión de diseño | El operador o agencia toma esta decisión basándose en los CSS extraídos en §7.1 y la nomenclatura Tailwind. Validada con contraste WCAG AA. | primary, secondary, accent, bg-light, bg-dark, text-primary, text-light, text-secondary |
| 16.20 · Paso-16 §8.2.3 Componentes | Se decide los tokens de componentes Tailwind | Decisión de diseño | El operador o agencia toma esta decisión basándose en los CSS extraídos en §7.1 y la nomenclatura Tailwind. | btn-radius, card-radius, card-shadow, input-radius, section-padding-y |

## Bloque 4 — Reglas críticas de aplicación CSS

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 16.21 · Paso-16 §8.2.4 Regla Hero | Se decide la regla crítica para Hero (fondo, texto, CTA) | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX y conversión. Las reglas las aplica el constructor del Paso 17 sin reinterpretar. | Hero con fondo bg-light, H1 text-primary, CTA primario |
| 16.22 · Paso-16 §8.2.4 Regla Botones | Se decide la regla crítica para botones primarios y secundarios | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX y conversión. | Primario: bg-primary text-light radius btn-radius. Secundario: bg-transparent border-primary text-primary |
| 16.23 · Paso-16 §8.2.4 Regla Sección Oscura | Se decide la regla crítica para secciones de fondo oscuro | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX y conversión. | bg-dark con text-light. CTA usa accent en vez de primary. |
| 16.24 · Paso-16 §8.2.4 Regla Cards | Se decide la regla crítica para cards (padding, radius, shadow, hover) | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX y conversión. | Padding 24px, radius card-radius, card-shadow base, hover lift 4px |
| 16.25 · Paso-16 §8.2.4 Regla Tipografía | Se decide la regla crítica para uso de fuentes (cuándo heading vs body) | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX y conversión. | H1-H3 con font-heading. Body, captions, FAQs con font-body. |
| 16.26 · Paso-16 §8.2.4 Regla Forms | Se decide la regla crítica para formularios y inputs | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX y conversión. | Input radius input-radius, border 1px text-secondary, focus border primary |

## Bloque 5 — Layout-Map definitivo por page type

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 16.27 · Paso-16 §8.3 Layout-Map Homepage | Se decide el Layout-Map definitivo de la Homepage cruzado con Paso 15 §9.1 | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. El framework GMB Crush exige cruzar el layout con las secciones del Paso 15. El detalle de columnas, breakpoints e imágenes es Decisión de diseño. | Homepage: 6 secciones con layout completo y comportamiento mobile/tablet/desktop |
| 16.28 · Paso-16 §8.3 Layout-Map SO | Se decide el Layout-Map definitivo de las Service Overview Pages cruzado con Paso 15 §10.1 | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. El framework GMB Crush exige cruzar el layout con las secciones del Paso 15. El detalle es Decisión de diseño. | SO: 7 secciones con layout completo |
| 16.29 · Paso-16 §8.3 Layout-Map LBS | Se decide el Layout-Map definitivo de las LBS cruzado con Paso 15 §11.1 | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. El framework GMB Crush exige cruzar el layout con las secciones del Paso 15. El detalle es Decisión de diseño. | LBS: 8 secciones con layout completo |
| 16.30 · Paso-16 §8.3 Layout-Map AC | Se decide el Layout-Map definitivo de la AC cruzado con Paso 15 §12.1 | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. El framework GMB Crush exige cruzar el layout con las secciones del Paso 15. El detalle es Decisión de diseño. | AC: 6 secciones con layout completo |
| 16.31 · Paso-16 §8.3 Layout-Map GeoHub | Se decide el Layout-Map definitivo del GeoHub cruzado con Paso 15 §13.1 | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. El framework GMB Crush exige cruzar el layout con las secciones del Paso 15. El detalle es Decisión de diseño. | GeoHub: 8 secciones con layout completo |
| 16.32 · Paso-16 §8.3 Layout-Map GeoArticle | Se decide el Layout-Map definitivo de los GeoArticles cruzado con Paso 15 §14.1 | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. El framework GMB Crush exige cruzar el layout con las secciones del Paso 15. El detalle es Decisión de diseño. | GeoArticle: 6 secciones con layout completo |
