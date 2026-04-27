# Correcciones aplicadas al sistema GMB Crush — Cerrajeros Madrid 24h

Fecha de última actualización: 27 de abril de 2026

---

## Resumen

Se han aplicado un total de **23 correcciones** al sistema completo (14 pasos + documento maestro). Todas las correcciones se aplicaron primero en el `Repo para correcciones` como sandbox, y después se propagaron a las carpetas `02 Sistema_ Ejecucion` y `03 Sistema_ Vision Completa`.

---

## Correcciones del primer lote (documento de correcciones V6)

| # | Corrección | Descripción | Archivos afectados |
|---|---|---|---|
| 0 | Definición operativa LCA | Añadida definición operativa de Local Coverage Areas al inicio del cuerpo operativo de los 14 pasos y del maestro | 14 pasos + maestro |
| 1 | Módulo interpretación dirección física | Añadido módulo completo de interpretación GMB Crush de la dirección física al final del paso 1 | Paso 1 + maestro |
| 2 | Test coherencia GEO | Incluido dentro del módulo de la corrección 1 | Paso 1 + maestro |
| 3 | /contact/ → /contacto/ | Unificada la URL de contacto al español | Transversal (14 pasos + maestro) |
| 5 | GeoArticle duplicado costes | guia-precios-cerrajero-urgente → cuanto-cuesta-un-cerrajero-urgente | Transversal |
| 6 | Trust signal móvil unificado | Unificado el trust signal de servicio móvil | Transversal |
| 7 | Duplicado de llaves como Additional Category | Verificado que Duplicado de llaves no está en core services sino como Additional Category con página propia | Paso 11 + maestro |
| 8 | Direct vs Candidate LCA | Separados los formularios en blanco y rellenados en Direct LCA, Candidate LCA y Approved Expansion Areas | Pasos 1, 14 + maestro |
| 9 | Eliminar Proveedor de sistemas de seguridad | Eliminada categoría GBP inventada | Paso 14 + maestro |
| 10 | Eliminar Reconocimiento local de servicio | Eliminado trust signal inventado | Paso 12 + maestro |
| 11 | Añadir email al intake | Añadido campo Email al NAP en formularios en blanco y rellenados | Paso 1 + todos los pasos con NAP + maestro |
| 12 | Completar 15 GeoArticles | Listados los 15 GeoArticles concretos en todos los pasos que los mencionan | 9 archivos + maestro |
| 13 | Priority Score completo 28 URLs | Añadida matriz completa de Priority Score para las 28 URLs | Paso 8 + maestro |
| 14 | QA estado para todas las URLs | Añadido estado QA para todas las URLs | Paso 9 + maestro |
| 15 | Calendario producción completo 7 fases | Añadido calendario de producción completo con 7 fases | Paso 10 + maestro |
| 16 | Menú GeoHub corregido | Eliminado duplicado de Cambio de bombines, añadida Instalación de cerraduras de seguridad | Pasos 5, 6 + maestro |
| 17 | Total páginas 28 SEO base | Corregido el conteo a 28 páginas SEO base | Transversal |

---

## Correcciones del segundo lote (auditoría post-correcciones)

| # | Corrección | Descripción | Archivos afectados |
|---|---|---|---|
| 1.2 | LBS canónico en paso 11 | apertura-puertas como LBS-001 → cerrajero-urgente en 7 lugares del pseudocódigo | Paso 11 + maestro |
| 1.5 | core_services sin Duplicado de llaves | Eliminado Duplicado de llaves de core_services, añadido Cambio de bombines, creado additional_categories_with_page | Paso 11 + maestro |
| NP1 | Error aritmético 27→28 | Corregidas todas las apariciones de 27 páginas a 28 páginas | Pasos 2, 12, 13 + maestro |
| NP2 | Redacción rota paso 1 | "licensed technicians y en el mismo día Servicio móvil en el mismo día" → redacción limpia en español | Paso 1 + maestro |
| NP3 | Direct/Candidate LCA en paso 11 | local_coverage_areas → direct_ + candidate_ en INPUT, ejemplo y bloque 10 del pseudocódigo | Paso 11 + maestro |
| NP4 | Disclosure GeoArticles | Añadido aviso de trazabilidad: 12 de los 15 GeoArticles son decisiones de la IA sin keyword research | 9 archivos + maestro |

---

## Correcciones residuales

| # | Corrección | Descripción | Archivos afectados |
|---|---|---|---|
| R1 | Doble punto | `base..` → `base.` | Paso 2 + maestro |
| R2 | Sintaxis antigua paso 13 | `28 páginas SEO base + /contacto/` → frase reformulada | Paso 13 + maestro |
| R3 | Variable antigua paso 11 | `content_uses = local_coverage_areas` → `direct_ + candidate_ (filtrado por test GEO)` | Paso 11 + maestro |

---

## Correcciones de alineación (P0.2 + P0.5)

| # | Corrección | Descripción | Archivos afectados |
|---|---|---|---|
| P0.2 | Paso 6 alineado con Direct/Candidate | Primary/Additional LCA → Direct/Candidate en formularios, ejemplos, principios, reglas operativas y checklist del paso 6 | Paso 6 + maestro |
| P0.5 | Lenguaje LCA corregido en paso 6 | "zonas atendidas", "cobertura real como criterio de selección", mezclas EN/ES → lenguaje alineado con la doctrina | Paso 6 + maestro |

---

## Correcciones de sincronización del maestro (P0.3)

| # | Corrección | Descripción |
|---|---|---|
| P0.3a | Definición operativa en maestro | Añadidas 14 definiciones operativas (una por paso) al maestro |
| P0.3b | core_services en maestro | Sincronizado con paso 11 individual (sin Duplicado de llaves, con Cambio de bombines) |
| P0.3c | Direct/Candidate LCA en maestro | Sincronizados INPUT y bloque 10 del paso 11 en el maestro |
| P0.3d | Email en maestro | Añadido campo Email en todos los formularios rellenados del maestro |
| P0.3e | Primary/Additional → Direct/Candidate en maestro | Sustituidos todos los formularios en blanco de pasos 5, 7, 8, 9, 10, 11, 12, 13 |

---

## Estado actual

Todos los archivos del `Repo para correcciones`, `02 Sistema_ Ejecucion` y `03 Sistema_ Vision Completa` están sincronizados con todas las correcciones aplicadas.

### Verificación final del maestro

| Indicador | Valor |
|---|---|
| Primary/Additional LCA | 0 apariciones |
| zonas reales atendidas (como criterio de selección) | 0 apariciones |
| Definición operativa por paso | 14 |
| Email en NAP | 10 apariciones |
| GBP Services ≠ core services (nota) | 1 |
| Direct Local Coverage | 18 apariciones |
| Candidate Local Coverage | 18 apariciones |
| 28 páginas SEO base | 7 apariciones |
| 27 páginas SEO base | 0 apariciones |
| Proveedor de sistemas de seguridad | 0 apariciones |
| Reconocimiento local de servicio | 0 apariciones |
