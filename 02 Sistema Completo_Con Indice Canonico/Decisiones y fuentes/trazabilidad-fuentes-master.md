# Trazabilidad de fuentes — 14 pasos

# Paso 1 — Intake Form

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

## Bloque 1 — Identidad del negocio

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 1.01 | Se define el nombre del negocio | Cerrajeros Madrid 24h | Input humano | El nombre del negocio fue proporcionado en el ejemplo. | Validada |
| 1.02 | Se define la URL principal de la web | https://www.cerrajerosmadrid24h.com | IA sin respaldo | El dominio fue creado para el ejemplo; no consta como dato real aportado. | Pendiente de validación |
| 1.03 | Se define el dominio canónico | https://www.cerrajerosmadrid24h.com | IA sin respaldo | Deriva del dominio de ejemplo; debe confirmarse antes de producción. | Pendiente de validación |

## Bloque 2 — Estado inicial del GBP

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 1.04 | Se decide que el GBP no existe todavía | GBP Status: Not Created | Input humano | La situación inicial acordada fue que no hay GBP. | Validada |
| 1.05 | Se decide que el GBP se creará después de publicar la web | After website launch | Input humano + GMB Crush | El usuario definió el flujo web-first; GMB Crush exige alinear web y GBP, pero no obliga a crear GBP antes. | Validada |
| 1.06 | Se decide que la verificación del GBP no ha empezado | GBP Verification Status: Not Started | Input humano | Si el GBP no existe, la verificación no ha empezado. | Validada |
| 1.07 | Se decide que no hay GBP URL todavía | N/A — GBP not created yet | GMB Crush | No se debe inventar sameAs ni URL de GBP si el perfil no existe. | Validada |

## Bloque 3 — NAP y contacto

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 1.08 | Se define el nombre NAP | Cerrajeros Madrid 24h | Input humano | Coincide con el nombre proporcionado. | Validada |
| 1.09 | Se define la dirección del negocio | Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí | Input humano | Dirección proporcionada en el ejemplo. | Validada |
| 1.10 | Se define la ciudad del negocio | Madrid | Input humano | La dirección proporcionada está en Madrid. | Validada |
| 1.11 | Se define la provincia o comunidad | Comunidad de Madrid | Geografía | Se infiere territorialmente desde Madrid; conviene confirmar formato administrativo final. | Parcialmente validada |
| 1.12 | Se define el código postal | 28010 | Geografía | El CP se infiere para la zona de Almagro/Chamberí; debe verificarse contra la dirección exacta. | Pendiente de validación |
| 1.13 | Se define el país | España | Input humano | El contexto y la dirección son de Madrid, España. | Validada |
| 1.14 | Se define el teléfono del negocio | +34 600 000 000 | IA sin respaldo | Teléfono placeholder creado para el ejemplo. | IA sin respaldo |
| 1.15 | Se define el email del negocio | info@cerrajerosmadrid24h.com | IA sin respaldo | Email derivado del dominio de ejemplo; no consta como dato real. | Pendiente de validación |

## Bloque 4 — Categorías GBP planificadas

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 1.16 | Se define la categoría principal planificada para el futuro GBP | Cerrajero | Input humano + GMB Crush | El nombre del negocio indica cerrajería; GMB Crush requiere categoría principal para alinear web y GBP. | Parcialmente validada |
| 1.17 | Se define una categoría adicional planificada | Servicio de cerrajería de urgencia | IA sin respaldo | Es coherente con “24h”, pero no fue confirmada ni validada como categoría disponible. | Pendiente de validación |
| 1.18 | Se define otra categoría adicional planificada | Servicio de duplicado de llaves | IA sin respaldo | Servicio/categoría típica de cerrajería, pero no confirmada por input ni datos. | Pendiente de validación |

## Bloque 5 — Dirección física, Main City y zonas

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 1.19 | Se define la dirección física como ancla del sistema | Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí, Madrid | Input humano | La dirección fue proporcionada y se usa como ancla NAP. | Validada |
| 1.20 | Se define la ciudad que crea la arquitectura base | Madrid | Input humano | Madrid sale directamente del dato de dirección. | Validada |
| 1.21 | Se define la ciudad de ubicación física | Madrid | Input humano | La ubicación física está en Madrid según el dato aportado. | Validada |
| 1.22 | Se define una Direct Local Coverage Area | Almagro | Input humano + Geografía | Almagro aparece en la dirección como barrio. | Validada |
| 1.23 | Se define una Direct Local Coverage Area | Chamberí | Input humano + Geografía | Chamberí aparece en la dirección como distrito. | Validada |
| 1.24 | Se define una Candidate Local Coverage Area | Salamanca | Geografía | Zona candidata por proximidad/contexto urbano; requiere test GEO/datos antes de uso fuerte. | Pendiente de validación |
| 1.25 | Se define una Candidate Local Coverage Area | Retiro | Geografía | Zona candidata por contexto Madrid; requiere validación de coherencia GEO. | Pendiente de validación |
| 1.26 | Se define una Candidate Local Coverage Area | Centro | Geografía | Zona candidata; requiere validación de proximidad/demanda/competencia. | Pendiente de validación |
| 1.27 | Se define una Candidate Local Coverage Area | Tetuán | Geografía | Zona candidata; requiere validación de proximidad/demanda/competencia. | Pendiente de validación |
| 1.28 | Se define una Candidate Local Coverage Area | Chamartín | Geografía | Zona candidata; requiere validación de proximidad/demanda/competencia. | Pendiente de validación |
| 1.29 | Se define una Candidate Local Coverage Area | Arganzuela | Geografía | Zona candidata; requiere validación de proximidad/demanda/competencia. | Pendiente de validación |
| 1.30 | Se define una Candidate Local Coverage Area | Moncloa | Geografía | Zona candidata; requiere validación de proximidad/demanda/competencia. | Pendiente de validación |
| 1.31 | Se define una Candidate Local Coverage Area | Prosperidad | Geografía | Zona candidata; requiere validación de proximidad/demanda/competencia. | Pendiente de validación |

## Bloque 6 — Expansión geográfica

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 1.32 | Se decide que las Local Coverage Areas no generarán páginas en la base | No, not in the base build | GMB Crush | La estructura base es ciudad + servicio; zonas/barrios se usan como señales GEO salvo expansión aprobada. | Validada |
| 1.33 | Se decide que no hay Approved Expansion Areas en la fase inicial | None in Phase 1 | GMB Crush | La expansión requiere aprobación/validación; la base se centra en Main City. | Validada |

## Bloque 7 — Servicios principales

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 1.34 | Se define el servicio principal 1 | Cerrajero urgente | IA sin respaldo | Servicio plausible por “24h”, pero no confirmado por input, datos ni competencia. | Pendiente de validación |
| 1.35 | Se define el servicio principal 2 | Apertura de puertas | IA sin respaldo | Servicio típico de cerrajería, pero no confirmado por input, datos ni competencia. | Pendiente de validación |
| 1.36 | Se define el servicio principal 3 | Cambio de cerraduras | IA sin respaldo | Servicio típico de cerrajería, pero no confirmado por input, datos ni competencia. | Pendiente de validación |
| 1.37 | Se define el servicio principal 4 | Cambio de bombines | IA sin respaldo | Servicio típico de cerrajería, pero no confirmado por input, datos ni competencia. | Pendiente de validación |
| 1.38 | Se define el servicio principal 5 | Instalación de cerraduras de seguridad | IA sin respaldo | Servicio típico de cerrajería, pero no confirmado por input, datos ni competencia. | Pendiente de validación |

## Bloque 8 — Consolidación de categorías adicionales

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 1.39 | Se decide que una categoría adicional ya está cubierta por un servicio principal | Servicio de cerrajería de urgencia queda cubierta por Cerrajero urgente | GMB Crush | Evita duplicar páginas cuando una categoría adicional ya está cubierta por un servicio core. | Validada |
| 1.40 | Se decide que una categoría adicional necesita página propia | Servicio de duplicado de llaves | GMB Crush + IA sin respaldo | GMB Crush exige soporte para categorías adicionales; la categoría concreta está pendiente de validación. | Parcialmente validada |

## Bloque 9 — Contenido, conversión y confianza

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 1.41 | Se define el número de GeoArticles por servicio | 3 | GMB Crush | El framework de GeoArticles pide generar 3 ideas por Service × City pair. | Validada |
| 1.42 | Se define el CTA principal | Llamar ahora | IA sin respaldo | CTA plausible para cerrajería, pero no confirmado por el negocio. | Pendiente de validación |
| 1.43 | Se define una señal de confianza | 10+ años de experiencia | IA sin respaldo | No consta input o prueba que confirme los años. | IA sin respaldo |
| 1.44 | Se define una señal de confianza pendiente del futuro GBP | Reseñas iniciales pendientes de recopilar tras crear y verificar el GBP | GMB Crush | Evita inventar reseñas antes de tener GBP real. | Validada |
| 1.45 | Se define una señal de confianza | Técnicos cerrajeros cualificados | IA sin respaldo | No consta confirmación del negocio. | Pendiente de validación |
| 1.46 | Se define una señal de confianza | Servicio móvil en el mismo día | IA sin respaldo | No consta confirmación operativa del negocio. | Pendiente de validación |
| 1.47 | Se define una señal de confianza | Garantía de trabajo | IA sin respaldo | No consta confirmación del negocio. | Pendiente de validación |



---

# Paso 2 — Fórmula Maestra de Arquitectura

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

## Bloque 1 — Alcance de la fórmula base

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.01 | Se decide que la fórmula base se construye sobre una sola Main City | Madrid | GMB Crush + Input humano | GMB Crush estructura la base por ciudad; Madrid viene de la dirección. | Validada |
| 2.02 | Se decide que las Local Coverage Areas no multiplican páginas por defecto | LCA no generan URLs base | GMB Crush | Barrios/zonas se usan como señales GEO; URLs de zona requieren expansión aprobada. | Validada |
| 2.03 | Se decide que las Approved Expansion Areas no entran en la fórmula inicial | None in Phase 1 | GMB Crush | La expansión es opcional y posterior a la base. | Validada |

## Bloque 2 — Servicios incluidos en el cálculo

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.04 | Se define el número de servicios principales usados en la fórmula | S = 5 | IA sin respaldo | El número depende de la lista de servicios, aún pendiente de validación. | Pendiente de validación |
| 2.05 | Se incluye Cerrajero urgente en el cálculo | Cerrajero urgente | IA sin respaldo | Servicio no validado con input/datos/competidores. | Pendiente de validación |
| 2.06 | Se incluye Apertura de puertas en el cálculo | Apertura de puertas | IA sin respaldo | Servicio no validado con input/datos/competidores. | Pendiente de validación |
| 2.07 | Se incluye Cambio de cerraduras en el cálculo | Cambio de cerraduras | IA sin respaldo | Servicio no validado con input/datos/competidores. | Pendiente de validación |
| 2.08 | Se incluye Cambio de bombines en el cálculo | Cambio de bombines | IA sin respaldo | Servicio no validado con input/datos/competidores. | Pendiente de validación |
| 2.09 | Se incluye Instalación de cerraduras de seguridad en el cálculo | Instalación de cerraduras de seguridad | IA sin respaldo | Servicio no validado con input/datos/competidores. | Pendiente de validación |

## Bloque 3 — Páginas generadas por la fórmula

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.10 | Se decide crear una Homepage | 1 Homepage | GMB Crush | Homepage es Root Entity Anchor obligatorio. | Validada |
| 2.11 | Se decide crear una Service Overview Page por cada servicio principal | 5 Service Overview Pages | GMB Crush + IA sin respaldo | La regla es GMB Crush; el número depende de servicios aún pendientes. | Parcialmente validada |
| 2.12 | Se decide crear un GeoHub para la Main City | 1 GeoHub para Madrid | GMB Crush | GeoHub de ciudad como contenedor local. | Validada |
| 2.13 | Se decide crear una LBS por cada servicio principal en Madrid | 5 LBS | GMB Crush + IA sin respaldo | El patrón es GMB Crush; el número depende de servicios pendientes. | Parcialmente validada |
| 2.14 | Se decide crear una Additional Category Page para la categoría adicional efectiva | 1 Additional Category Page | GMB Crush + IA sin respaldo | GMB exige soporte de categorías; categoría concreta pendiente. | Parcialmente validada |

## Bloque 4 — Categorías adicionales efectivas

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.15 | Se decide que Servicio de cerrajería de urgencia no suma como categoría adicional separada | Cubierta por Cerrajero urgente | GMB Crush | Evita duplicar una intención ya cubierta por core service. | Validada |
| 2.16 | Se decide que Servicio de duplicado de llaves cuenta como categoría adicional efectiva | A = 1 | GMB Crush + IA sin respaldo | La lógica es GMB; la categoría concreta no está validada. | Parcialmente validada |

## Bloque 5 — GeoArticles

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.17 | Se decide usar 3 GeoArticles por servicio principal | G = 3 | GMB Crush | GeoArticle framework pide 3 ideas por Service × City pair. | Validada |
| 2.18 | Se decide calcular GeoArticles como G × S | 3 × 5 | GMB Crush + IA sin respaldo | La fórmula es GMB; S depende de servicios no validados. | Parcialmente validada |
| 2.19 | Se calcula el número total de GeoArticles | 15 GeoArticles | GMB Crush + IA sin respaldo | Deriva de G=3 y S=5; S pendiente. | Parcialmente validada |
| 2.20 | Se decide que los GeoArticles se generan para Madrid, no para cada LCA | 15 GeoArticles para Madrid | GMB Crush | GeoArticles son servicio + ciudad + long-tail; LCA no multiplican URLs. | Validada |

## Bloque 6 — Total de páginas SEO base

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 2.21 | Se calcula el bloque de Homepage | 1 página | GMB Crush | Parte fija de la arquitectura. | Validada |
| 2.22 | Se calcula el bloque de Service Overview Pages | 5 páginas | GMB Crush + IA sin respaldo | Depende de los servicios elegidos. | Parcialmente validada |
| 2.23 | Se calcula el bloque de GeoHub | 1 página | GMB Crush | Un GeoHub para la Main City. | Validada |
| 2.24 | Se calcula el bloque de LBS | 5 páginas | GMB Crush + IA sin respaldo | Depende de los servicios elegidos. | Parcialmente validada |
| 2.25 | Se calcula el bloque de Additional Category Pages | 1 página | GMB Crush + IA sin respaldo | Depende de categoría adicional efectiva pendiente. | Parcialmente validada |
| 2.26 | Se calcula el bloque de GeoArticles | 15 páginas | GMB Crush + IA sin respaldo | Depende de servicios y temas pendientes de keyword research. | Parcialmente validada |
| 2.27 | Se calcula el total de páginas SEO base | 28 páginas SEO base | GMB Crush + IA sin respaldo | La suma es correcta si se aceptan S=5, A=1 y G=3. | Parcialmente validada |
| 2.28 | Se decide que /contacto/ queda fuera del inventario SEO base | Página auxiliar | GMB Crush | Contacto es página operativa, no uno de los 6 tipos SEO principales. | Validada |



---

# Paso 3 — Matriz Base

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

## Bloque 1 — Estructura de la matriz

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.01 | Se decide crear una matriz operativa para controlar las URLs | URL Matrix | GMB Crush | La metodología requiere controlar páginas, URLs, schema, links y fases. | Validada |
| 3.02 | Se decide que cada página tenga un ID único | HP, SO, GH, LBS, AC, GA | GMB Crush | IDs permiten controlar tipos de página y evitar duplicados. | Validada |
| 3.03 | Se decide incluir columnas de producción | URL, H1, Meta Title, Schema, Priority, Phase, Status | GMB Crush | Cada página debe tener función, metadata, schema, prioridad y fase. | Validada |

## Bloque 2 — Homepage y páginas auxiliares

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.04 | Se decide incluir la Homepage en la matriz | HP-001 | GMB Crush | Homepage es Root Entity Anchor. | Validada |
| 3.05 | Se decide que la Homepage use la raíz | / | GMB Crush | El framework define la homepage en root domain. | Validada |
| 3.06 | Se decide incluir página de contacto como auxiliar | /contacto/ | GMB Crush | La homepage y otras páginas deben enlazar a contacto; no es URL SEO base. | Validada |

## Bloque 3 — Service Overview Pages

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.07 | Se decide crear Service Overview para Cerrajero urgente | /cerrajero/cerrajero-urgente/ | GMB Crush + IA sin respaldo | Patrón GMB; servicio pendiente de validación. | Parcialmente validada |
| 3.08 | Se decide crear Service Overview para Apertura de puertas | /cerrajero/apertura-puertas/ | GMB Crush + IA sin respaldo | Patrón GMB; servicio pendiente de validación. | Parcialmente validada |
| 3.09 | Se decide crear Service Overview para Cambio de cerraduras | /cerrajero/cambio-cerraduras/ | GMB Crush + IA sin respaldo | Patrón GMB; servicio pendiente de validación. | Parcialmente validada |
| 3.10 | Se decide crear Service Overview para Cambio de bombines | /cerrajero/cambio-bombines/ | GMB Crush + IA sin respaldo | Patrón GMB; servicio pendiente de validación. | Parcialmente validada |
| 3.11 | Se decide crear Service Overview para Instalación de cerraduras de seguridad | /cerrajero/instalacion-cerraduras-seguridad/ | GMB Crush + IA sin respaldo | Patrón GMB; servicio pendiente de validación. | Parcialmente validada |

## Bloque 4 — GeoHub y Location-Based Service Pages

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.12 | Se decide crear el GeoHub principal de Madrid | /madrid/ | GMB Crush + Input humano | GeoHub por Main City; Madrid viene del input. | Validada |
| 3.13 | Se decide crear LBS de Cerrajero urgente en Madrid | /cerrajero/madrid/cerrajero-urgente/ | GMB Crush + IA sin respaldo | Patrón /category/city/service/ validado; servicio pendiente. | Parcialmente validada |
| 3.14 | Se decide crear LBS de Apertura de puertas en Madrid | /cerrajero/madrid/apertura-puertas/ | GMB Crush + IA sin respaldo | Patrón validado; servicio pendiente. | Parcialmente validada |
| 3.15 | Se decide crear LBS de Cambio de cerraduras en Madrid | /cerrajero/madrid/cambio-cerraduras/ | GMB Crush + IA sin respaldo | Patrón validado; servicio pendiente. | Parcialmente validada |
| 3.16 | Se decide crear LBS de Cambio de bombines en Madrid | /cerrajero/madrid/cambio-bombines/ | GMB Crush + IA sin respaldo | Patrón validado; servicio pendiente. | Parcialmente validada |
| 3.17 | Se decide crear LBS de Instalación de cerraduras de seguridad en Madrid | /cerrajero/madrid/instalacion-cerraduras-seguridad/ | GMB Crush + IA sin respaldo | Patrón validado; servicio pendiente. | Parcialmente validada |

## Bloque 5 — Additional Category Page

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.18 | Se decide crear página de duplicado de llaves en Madrid | /cerrajero/madrid/duplicado-llaves/ | GMB Crush + IA sin respaldo | Additional Category Page está respaldada; categoría concreta pendiente. | Parcialmente validada |

## Bloque 6 — GeoArticles

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.19-3.33 | Se deciden 15 GeoArticles con URLs concretas | 15 URLs /madrid/[topic]/ | GMB Crush + IA sin respaldo | GMB exige 3 ideas por servicio; temas y slugs no están validados con keyword research. | Pendiente de validación |

## Bloque 7 — Tratamiento de Local Coverage Areas

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 3.34 | Se decide que las LCA aparezcan como notas o campos de contenido | Almagro, Chamberí, Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad | GMB Crush + Geografía | GMB permite señales GEO; directas validadas, candidatas pendientes. | Parcialmente validada |
| 3.35 | Se decide que no haya filas URL para Local Coverage Areas | No /almagro/, no /chamberi/, no /salamanca/ | GMB Crush | LCA no generan URLs salvo Approved Expansion Areas. | Validada |



---

# Paso 4 — URL Rules

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

## Bloque 1 — Dominio y formato general

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 4.01 | Se decide usar HTTPS | https:// | GMB Crush | Estándar web/canónico para URLs de producción. | Validada |
| 4.02 | Se decide usar dominio canónico con www | https://www.cerrajerosmadrid24h.com | IA sin respaldo | El dominio es de ejemplo y debe confirmarse. | Pendiente de validación |
| 4.03 | Se decide usar trailing slash | Sí | GMB Crush | Regla operativa de consistencia URL. | Validada |

## Bloque 2 — Patrones URL principales

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 4.04 | Se decide que la Homepage use raíz | / | GMB Crush | Homepage root domain. | Validada |
| 4.05 | Se decide que Service Overview use categoría + servicio | /cerrajero/[service-slug]/ | GMB Crush | Service Overview usa /category/service/. | Validada |
| 4.06 | Se decide que LBS use categoría + ciudad + servicio | /cerrajero/madrid/[service-slug]/ | GMB Crush | Location-Based Service usa /category/city/service/. | Validada |
| 4.07 | Se decide que Additional Category use categoría + ciudad + servicio | /cerrajero/madrid/duplicado-llaves/ | GMB Crush | Additional Category Page usa estructura local por ciudad. | Validada |
| 4.08 | Se decide que GeoHub use ciudad | /madrid/ | GMB Crush | GeoHub es contenedor de ciudad. | Validada |
| 4.09 | Se decide que GeoArticles usen ciudad + topic | /madrid/[article-topic-slug]/ | GMB Crush | GeoArticle usa ciudad + long-tail topic. | Validada |

## Bloque 3 — URLs concretas de servicio

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 4.10-4.14 | Se deciden URLs locales para los 5 servicios | 5 URLs /cerrajero/madrid/[service]/ | GMB Crush + IA sin respaldo | Patrón validado; servicios pendientes de validación. | Parcialmente validada |

## Bloque 4 — Reglas anti-URL débil

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 4.15 | Se decide no usar near-me en URLs principales | No near-me | GMB Crush | Evita URLs artificiales o débiles. | Validada |
| 4.16 | Se decide no usar adjetivos SEO vacíos en URLs | No best, cheap, top-rated | GMB Crush | Evita slugs manipulativos y no semánticos. | Validada |
| 4.17 | Se decide no crear URLs para Local Coverage Areas en la base | No /almagro/, no /chamberi/, no /salamanca/ | GMB Crush | Las LCA no generan URL por defecto. | Validada |
| 4.18 | Se decide que Approved Expansion Areas podrían generar URLs solo en expansión | None in Phase 1 | GMB Crush | La expansión requiere aprobación. | Validada |



---

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



---

# Paso 6 — Estructura de Contenido + Local Coverage Areas

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

## Bloque 1 — Main City y Local Coverage Areas

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 6.01 | Se decide que Madrid crea la estructura principal | Madrid | Input humano + GMB Crush | Madrid viene de dirección; GMB estructura por ciudad. | Validada |
| 6.02 | Se decide que Direct LCA refuercen el contenido | Almagro, Chamberí | Input humano + Geografía | Ambas salen del NAP/dirección. | Validada |
| 6.03 | Se decide que Candidate LCA puedan usarse si pasan test GEO | Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad | Geografía | Son candidatas; requieren validación de proximidad/datos/competencia. | Pendiente de validación |
| 6.04 | Se decide que las LCA no sustituyan a Madrid | La página sigue siendo Madrid | GMB Crush | Las páginas son city/service; zonas son señales GEO. | Validada |

## Bloque 2 — Uso por tipo de página

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 6.05 | Se decide que la Homepage pueda mencionar LCA de forma ligera | Almagro, Chamberí, etc. | GMB Crush | Homepage establece dónde opera; menciones deben ser secundarias. | Validada |
| 6.06 | Se decide que Service Overview no use LCA | Sin zonas locales | GMB Crush | Service Overview es no geolocalizada. | Validada |
| 6.07 | Se decide que LBS use LCA en intro, H2s y FAQs | Páginas servicio + Madrid | GMB Crush | Location pages permiten geo-specific paragraph, neighborhoods/local issues. | Validada |
| 6.08 | Se decide que GeoHub use sección de cobertura local | /madrid/ | GMB Crush | GeoHub puede incluir neighborhood coverage. | Validada |
| 6.09 | Se decide que Additional Category use cobertura local como contexto | /cerrajero/madrid/duplicado-llaves/ | GMB Crush | Additional Category Page debe ser local y GEO-optimizada. | Validada |
| 6.10 | Se decide que GeoArticles usen zonas como ejemplos locales | Madrid + zonas GEO | GMB Crush | GeoArticles incluyen local references/landmarks/neighborhoods. | Validada |

## Bloque 3 — Restricciones

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 6.11 | Se decide que una mención de zona no equivale a crear URL | Mencionar Almagro ≠ crear /almagro/ | GMB Crush | La arquitectura base no crea URLs por zona. | Validada |
| 6.12 | Se decide no afirmar oficina física en cada LCA | No oficina en Salamanca/Retiro salvo verdad | GMB Crush | GeoArticles y páginas locales no deben fingir ubicación física. | Validada |
| 6.13 | Se decide que areaServed pueda incluir cobertura real validada | Madrid + zonas validadas | GMB Crush + Geografía | Schema debe reflejar cobertura real/validada, no aspiracional. | Parcialmente validada |



---

# Paso 7 — Internal Linking Rules

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

## Bloque 1 — Enlaces desde Homepage

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 7.01 | Homepage enlaza a Service Overview Pages | 5 Service Overview Pages | GMB Crush | Homepage debe enlazar a Service Overviews. | Validada |
| 7.02 | Homepage enlaza al GeoHub de Madrid | /madrid/ | GMB Crush | Homepage debe enlazar al Main GeoHub. | Validada |
| 7.03 | Homepage enlaza a Additional Category Page | /cerrajero/madrid/duplicado-llaves/ | GMB Crush | Additional Category Pages deben estar enlazadas. | Validada |
| 7.04 | Homepage enlaza a contacto | /contacto/ | GMB Crush | Contacto es destino operacional obligatorio. | Validada |

## Bloque 2 — Enlaces desde Service Overview y LBS

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 7.05 | Service Overview enlaza a versión local en Madrid | /cerrajero/[service]/ → /cerrajero/madrid/[service]/ | GMB Crush | Service Overview enlaza a versiones city/service. | Validada |
| 7.06 | Service Overview enlaza a servicios relacionados | Cross-links entre servicios | GMB Crush | Cross-linking refuerza silo semántico. | Validada |
| 7.07 | LBS enlaza a página padre | LBS → Service Overview | GMB Crush | LBS debe enlazar a parent service. | Validada |
| 7.08 | LBS enlaza al GeoHub | LBS → /madrid/ | GMB Crush | LBS debe enlazar al GeoHub. | Validada |
| 7.09 | LBS enlaza a servicios relacionados en Madrid | LBS → otras LBS | GMB Crush | Mismo city silo. | Validada |
| 7.10 | LBS enlaza a GeoArticles relacionados | LBS → GeoArticles | GMB Crush | GeoArticles refuerzan LBS. | Validada |

## Bloque 3 — GeoHub y GeoArticles

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 7.11 | GeoHub enlaza a todas las LBS de Madrid | 5 LBS | GMB Crush | GeoHub agrupa servicios de ciudad. | Validada |
| 7.12 | GeoHub enlaza a Additional Category Page | /cerrajero/madrid/duplicado-llaves/ | GMB Crush | GeoHub agrupa categorías locales. | Validada |
| 7.13 | GeoHub enlaza a GeoArticles | 15 GeoArticles | GMB Crush | GeoHub agrupa artículos ciudad/servicio. | Validada |
| 7.14 | GeoArticles enlazan a LBS correspondiente | GeoArticle → LBS | GMB Crush | Interlink obligatorio. | Validada |
| 7.15 | GeoArticles enlazan al GeoHub | GeoArticle → /madrid/ | GMB Crush | Interlink obligatorio. | Validada |

## Bloque 4 — Restricciones de enlaces

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 7.16 | No enlazar LCA sin URL aprobada | No enlazar /almagro/ | GMB Crush | No se enlaza a URLs inexistentes/no aprobadas. | Validada |
| 7.17 | Usar anchors contextuales | Anchors naturales | GMB Crush | Anchors contextuales evitan exact-match forzado. | Validada |
| 7.18 | Usar breadcrumbs | Home > Madrid > Servicio | GMB Crush | BreadcrumbList y navegación jerárquica. | Validada |



---

# Paso 8 — Priority Score

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

## Bloque 1 — Fórmula de prioridad

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 8.01 | Se decide usar fórmula de seis factores | Revenue + Intent + GBP Relevance + Local Relevance + Gap + Urgency | GMB Crush | Prioriza por valor, intención y relevancia local. | Validada |
| 8.02 | Se decide no usar City Priority en la base | Se usa Local Relevance | GMB Crush | La base tiene una Main City; no hay comparación multi-ciudad. | Validada |

## Bloque 2 — Ejemplo canónico

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 8.03 | Se decide evaluar LBS de Cerrajero urgente | /cerrajero/madrid/cerrajero-urgente/ | GMB Crush + IA sin respaldo | LBS canónica estructural; servicio concreto pendiente. | Parcialmente validada |
| 8.04 | Se asigna Revenue Value | 5 | IA sin respaldo | No hay datos económicos o de conversión. | IA sin respaldo |
| 8.05 | Se asigna Search Intent | 5 | IA sin respaldo | No hay keyword research documentado. | IA sin respaldo |
| 8.06 | Se asigna GBP Category Relevance | 5 | GMB Crush + IA sin respaldo | Parece alineado con cerrajero, pero categoría/servicio no confirmados. | Parcialmente validada |
| 8.07 | Se asigna Local Relevance | 5 | Input humano + GMB Crush | Madrid es Main City; LBS de Madrid es estructuralmente relevante. | Validada |
| 8.08 | Se asigna Competition Gap | 4 | IA sin respaldo | No hay análisis competitivo documentado. | IA sin respaldo |
| 8.09 | Se asigna Conversion Urgency | 5 | IA sin respaldo | Plausible para urgencias, pero no validado con datos. | Pendiente de validación |
| 8.10 | Se calcula el score total | 29 | IA sin respaldo | Suma de factores no validados. | Pendiente de validación |
| 8.11 | Se asigna prioridad | P1 | IA sin respaldo | Deriva del score pendiente de validación. | Pendiente de validación |

## Bloque 3 — Inventario completo

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 8.12 | Se decide asignar Priority Score a las 28 URLs SEO base | 28 URLs | GMB Crush | Cada URL debe tener prioridad para producción. | Validada |
| 8.13 | Se decide que /contacto/ tenga prioridad operativa, no SEO | Página auxiliar | GMB Crush | Contacto no forma parte del inventario SEO base. | Validada |
| 8.14 | Se decide que GeoArticles se prioricen después de páginas padre | GeoArticle después de LBS | GMB Crush | GeoArticles apoyan LBS/GeoHub, no sustituyen páginas padre. | Validada |



---

# Paso 9 — QA Checklist

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

## Bloque 1 — Ejemplo desarrollado

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 9.01 | Se decide auditar como ejemplo una LBS concreta | /cerrajero/madrid/cerrajero-urgente/ | GMB Crush | LBS es página crítica para QA. | Validada |
| 9.02 | Se asigna ID de QA | LBS-001 | GMB Crush | ID permite control de QA por URL. | Validada |
| 9.03 | Se define el tipo de página auditada | Location-Based Service | GMB Crush | Tipo de página del framework. | Validada |
| 9.04 | Se define el servicio objetivo | Cerrajero urgente | IA sin respaldo | Servicio pendiente de validación. | Pendiente de validación |
| 9.05 | Se define la Main City | Madrid | Input humano | Madrid sale de dirección. | Validada |
| 9.06 | Se define estado de QA | Ready for QA | IA sin respaldo | Estado operativo asignado en el ejemplo, no validación real. | Pendiente de validación |
| 9.07 | Se define reviewer | SEO Manager | IA sin respaldo | Rol genérico no asociado a persona real. | Pendiente de validación |
| 9.08 | Se define fecha de QA | 2026-04-24 | IA sin respaldo | Fecha generada en ejemplo, no calendario real confirmado. | Pendiente de validación |

## Bloque 2 — Checks obligatorios

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 9.09-9.20 | Se deciden checks obligatorios de QA | parent page, GeoHub, related services, GeoArticle, schema, NAP, CTA, no falsa ubicación, no canibalización | GMB Crush | QA refleja requisitos de estructura, schema, links, NAP y no falsa ubicación. | Validada |

## Bloque 3 — Inventario QA

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 9.21 | Se decide que inventario SEO base tenga QA Status | 28 URLs | GMB Crush | Ninguna URL debe publicarse sin QA. | Validada |
| 9.22 | Se decide que /contacto/ también pase QA operativo | Página auxiliar | GMB Crush | Contacto debe ser funcional y consistente con NAP. | Validada |
| 9.23 | Se decide que resto de URLs queden Pending hasta ejecución real | QA Pending | GMB Crush | Estado pendiente evita asumir aprobación no realizada. | Validada |



---

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



---

# Paso 11 — Pseudocódigo del Sistema

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

## Bloque 1 — Inputs, slugs y categorías

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 11.01 | Se decide cargar inputs base | Business name, URL, NAP, Main City, servicios, LCA, GBP status | GMB Crush | El sistema necesita inputs antes de generar arquitectura. | Validada |
| 11.02 | Se decide normalizar slugs | Cerrajero urgente → cerrajero-urgente | GMB Crush | URLs limpias requieren normalización. | Validada |
| 11.03 | Se decide validar categorías adicionales | Cubierta / necesita página | GMB Crush | Evita duplicados y asegura soporte a categorías. | Validada |

## Bloque 2 — Generación base

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 11.04 | Se decide generar Homepage | HP-001 | GMB Crush | Root Entity Anchor. | Validada |
| 11.05 | Se decide generar Service Overview Pages | 5 páginas | GMB Crush + IA sin respaldo | Patrón válido; lista de servicios pendiente. | Parcialmente validada |
| 11.06 | Se decide generar GeoHub de Madrid | /madrid/ | GMB Crush + Input humano | GeoHub de Main City. | Validada |
| 11.07 | Se decide generar LBS de Madrid | 5 páginas | GMB Crush + IA sin respaldo | Patrón válido; servicios pendientes. | Parcialmente validada |
| 11.08 | Se decide generar Additional Category Page efectiva | /cerrajero/madrid/duplicado-llaves/ | GMB Crush + IA sin respaldo | Tipo válido; categoría pendiente. | Parcialmente validada |
| 11.09 | Se decide generar GeoArticles | 15 artículos | GMB Crush + IA sin respaldo | Cantidad válida; temas pendientes de datos. | Parcialmente validada |

## Bloque 3 — LCA y expansión

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 11.10 | Se decide inyectar LCA en contenido y schema | LCA como señales GEO | GMB Crush + Geografía | LCA directas validadas; candidatas pendientes de test GEO. | Parcialmente validada |
| 11.11 | Se decide no generar expansión si no está aprobada | Approved Expansion Areas: None | GMB Crush | No crear URLs fuera de Main City sin aprobación. | Validada |

## Bloque 4 — Enlaces, prioridad, QA y outputs

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 11.12 | Se decide asignar enlaces internos por tipo | Internal Linking Map | GMB Crush | Jerarquía de enlaces del framework. | Validada |
| 11.13 | Se decide calcular prioridad por página | Priority Score | GMB Crush | Orden de producción requiere scoring. | Validada |
| 11.14 | Se decide comprobar dependencias | LBS requiere Service Overview + GeoHub | GMB Crush | Evita páginas huérfanas o sin padre. | Validada |
| 11.15 | Se decide ejecutar QA antes de publicar | QA Matrix | GMB Crush | No publicar sin QA. | Validada |
| 11.16 | Se decide producir matrices finales | URL Matrix, Internal Linking Matrix, Schema Map, Priority Score, Publishing Plan, QA Matrix | GMB Crush | El output operativo son matrices, no contenido suelto. | Validada |



---

# Paso 12 — Master Prompt Reutilizable

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

## Bloque 1 — Creación del prompt maestro

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 12.01 | Se decide crear un prompt maestro reutilizable | Master Prompt GMB Crush | GMB Crush | El sistema debe ser reutilizable y automatizable. | Validada |
| 12.02 | Se decide que el prompt genere el sistema completo | 14 pasos | GMB Crush | El prompt debe reproducir todo el SOP. | Validada |

## Bloque 2 — Inputs del prompt

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 12.03 | El prompt pide Main City | Madrid | Input humano + GMB Crush | Madrid es input; GMB usa ciudad como base. | Validada |
| 12.04 | El prompt pide Direct Local Coverage Areas | Almagro, Chamberí | Input humano + Geografía | Salen del NAP/dirección. | Validada |
| 12.05 | El prompt pide Candidate Local Coverage Areas | Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad | Geografía | Candidatas; requieren validación. | Pendiente de validación |
| 12.06 | El prompt pide Approved Expansion Areas | None in Phase 1 | GMB Crush | No hay expansión inicial. | Validada |
| 12.07 | El prompt pide GBP Status | Not Created | Input humano | Situación inicial acordada. | Validada |
| 12.08 | El prompt pide Planned Primary GBP Category | Cerrajero | Input humano + GMB Crush | Deriva del nombre/categoría principal planificada. | Parcialmente validada |
| 12.09 | El prompt pide Planned Additional GBP Categories | Servicio de cerrajería de urgencia, Servicio de duplicado de llaves | IA sin respaldo | Categorías concretas pendientes de validación. | Pendiente de validación |

## Bloque 3 — Outputs del prompt

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 12.10-12.17 | El prompt genera matrices, reglas, content architecture, links, score, plan, QA y GBP alignment | Sí | GMB Crush | El sistema requiere outputs operativos para cada capa. | Validada |

## Bloque 4 — Restricciones del prompt

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 12.18 | No inventar GBP URL | GBP URL N/A hasta creación | GMB Crush | No sameAs/GBP URL inexistente. | Validada |
| 12.19 | No crear URLs para LCA por defecto | No URLs LCA | GMB Crush | LCA son señales GEO salvo expansión. | Validada |
| 12.20 | Mantener web-first | Web primero, GBP después | Input humano + GMB Crush | Flujo acordado y alineado con sistema. | Validada |



---

# Paso 13 — Sistema Final Operativo

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

## Bloque 1 — Consolidación del sistema

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 13.01 | Se consolida el sistema en SOP final | Sistema GMB Crush de 14 pasos | GMB Crush | El sistema debe quedar operativo y secuencial. | Validada |
| 13.02 | El sistema empieza con Intake | Paso 1 | GMB Crush | Primero inputs, luego arquitectura. | Validada |
| 13.03 | El sistema cierra con GBP después de la web | Paso 14 | Input humano + GMB Crush | Web-first acordado. | Validada |

## Bloque 2 — Secuencia operativa

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 13.04-13.14 | Se decide la secuencia de pasos 2 a 12 | Arquitectura → matriz → URL rules → page types → contenido → links → score → QA → producción → pseudocódigo → prompt | GMB Crush | Secuencia lógica para evitar duplicados, huérfanas y outputs incompletos. | Validada |

## Bloque 3 — Outputs finales

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 13.15 | El sistema produce matrices | URL Matrix, Schema Map, Linking Map, QA, Publishing Plan | GMB Crush | Outputs operativos del sistema. | Validada |
| 13.16 | El sistema se optimiza con tracking | GMB Crush Geo Grid, GSC, GA4 | GMB Crush + IA sin respaldo | Tracking recomendado; herramientas específicas deben confirmarse. | Parcialmente validada |
| 13.17 | Local Coverage Areas refuerzan contenido, no URLs | LCA como señales GEO | GMB Crush | Zonas se usan como señales, no URLs por defecto. | Validada |
| 13.18 | Approved Expansion Areas son opcionales | None in Phase 1 | GMB Crush | No expansión sin aprobación. | Validada |



---

# Paso 14 — GBP Creation & Website Alignment

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

## Bloque 1 — Momento de creación y estado inicial

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 14.01 | Crear GBP después de publicar web base | After website launch | Input humano + GMB Crush | Flujo web-first acordado; web soporta GBP antes de crearlo. | Validada |
| 14.02 | Estado inicial del GBP | Not Created | Input humano | Situación inicial confirmada. | Validada |
| 14.03 | Sincronizar GBP, web, schema y tracking al final | Paso 14 como cierre | GMB Crush | GBP debe alinearse con web y schema. | Validada |

## Bloque 2 — NAP, modelo y dirección

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 14.04 | NAP final para el GBP | Cerrajeros Madrid 24h + Calle Rafael Calvo 12 + Madrid + teléfono | Input humano + IA sin respaldo | Nombre/dirección validos; teléfono placeholder no validado. | Parcialmente validada |
| 14.05 | Modelo de negocio | Service Area Business | IA sin respaldo | Modelo no confirmado; plausible para cerrajero. | Pendiente de validación |
| 14.06 | Dirección física | Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí, Madrid | Input humano | Dirección aportada. | Validada |
| 14.07 | Mostrar dirección públicamente depende del modelo y elegibilidad | Depends on business model and eligibility | GMB Crush | Evita afirmaciones no elegibles sobre ubicación. | Validada |

## Bloque 3 — Main City y LCA

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 14.08 | Main City para GBP | Madrid | Input humano | Dirección en Madrid. | Validada |
| 14.09 | Direct LCA para GBP | Almagro, Chamberí | Input humano + Geografía | Salen de dirección. | Validada |
| 14.10 | Candidate LCA para GBP | Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad | Geografía | Candidatas; no todas están validadas para GBP service areas. | Pendiente de validación |
| 14.11 | No hay Approved Expansion Areas iniciales | None in Phase 1 | GMB Crush | No URLs/expansión sin aprobación. | Validada |

## Bloque 4 — Categorías GBP

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 14.12 | Categoría principal prevista | Cerrajero | Input humano + GMB Crush | Deriva del nombre; debe confirmarse como categoría GBP disponible. | Parcialmente validada |
| 14.13 | Primera categoría adicional prevista | Servicio de cerrajería de urgencia | IA sin respaldo | Pendiente de confirmar disponibilidad/encaje. | Pendiente de validación |
| 14.14 | Segunda categoría adicional prevista | Servicio de duplicado de llaves | IA sin respaldo | Pendiente de confirmar disponibilidad/encaje. | Pendiente de validación |
| 14.15 | No añadir categoría de seguridad sin soporte web real | No añadir Proveedor de sistemas de seguridad | GMB Crush | Cada categoría adicional debe tener soporte web real. | Validada |

## Bloque 5 — Servicios del GBP

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 14.16-14.21 | Se definen servicios del GBP | Apertura, urgente, cerraduras, bombines, duplicado, seguridad | IA sin respaldo | Servicios plausibles pero no confirmados con input/datos/competencia. | Pendiente de validación |

## Bloque 6 — URLs conectadas al GBP

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 14.22 | URL web conectada al GBP | https://www.cerrajerosmadrid24h.com/ | IA sin respaldo | Dominio de ejemplo pendiente de confirmación. | Pendiente de validación |
| 14.23 | URL de contacto/cita | https://www.cerrajerosmadrid24h.com/contacto/ | GMB Crush + IA sin respaldo | /contacto/ es canónica; dominio pendiente. | Parcialmente validada |

## Bloque 7 — Horarios y recursos visuales

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 14.24 | Horarios de apertura | 24 horas, todos los días | IA sin respaldo | Inferido por nombre 24h, pendiente de confirmación. | Pendiente de validación |
| 14.25-14.30 | Preparar fotos y recursos visuales | Logo, cover, equipo, vehículo, herramientas, trabajos | GMB Crush | GBP y homepage requieren pruebas visuales/trust; recursos concretos pendientes. | Parcialmente validada |

## Bloque 8 — Q&A, posts, reseñas y tracking

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 14.31 | Preparar Q&A del GBP | Q&A Plan | GMB Crush | GBP debe cubrir preguntas reales del usuario. | Validada |
| 14.32 | Preparar Google Posts | Google Posts Plan | GMB Crush | GBP se optimiza después de creación. | Validada |
| 14.33 | Crear estrategia de reseñas reales | Review Strategy | GMB Crush | No se inventan reseñas; se recogen después. | Validada |
| 14.34 | Crear UTM para el enlace GBP | GBP UTM URL | GMB Crush | Tracking de interacciones GBP. | Validada |

## Bloque 9 — Ajustes post-GBP en la web

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 14.35 | Actualizar schema después de crear GBP | Añadir sameAs cuando exista GBP URL | GMB Crush | sameAs solo con URL real. | Validada |
| 14.36 | Actualizar Homepage tras crear GBP | Añadir GBP URL, reseñas reales si existen, trust blocks | GMB Crush | Alineación web-GBP. | Validada |
| 14.37 | Actualizar contacto tras crear GBP | Datos confirmados y mapa si procede | GMB Crush | Contacto debe alinear NAP/GBP. | Validada |
| 14.38 | Actualizar LBS tras crear GBP | Ajustar schema, sameAs, reseñas y NAP | GMB Crush | LBS soportan GBP y Local Pack. | Validada |
| 14.39 | Actualizar GeoHub tras crear GBP | Alinear cobertura, reviews y enlaces | GMB Crush | GeoHub agrupa señales ciudad/GBP. | Validada |

## Bloque 10 — No invención

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 14.40 | No inventar reseñas antes de que existan | Reseñas iniciales pendientes | GMB Crush | No usar social proof inexistente. | Validada |
| 14.41 | No inventar GBP URL antes de crear perfil | GBP URL N/A hasta creación | GMB Crush | No sameAs ni URL falsa. | Validada |



---

