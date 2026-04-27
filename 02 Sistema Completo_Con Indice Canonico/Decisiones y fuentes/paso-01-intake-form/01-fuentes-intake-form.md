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

| ID · Ref. canónica | Decisión tomada | Valor decidido en el ejemplo | Fuente | Funcionamiento de la fuente |
|---|---|---|---|---|
| 1.01 · Paso-01 §7 Business Name | Se define el nombre del negocio | Cerrajeros Madrid 24h | Input humano | El cliente proporciona el nombre del negocio directamente. El sistema lo recoge sin transformación. |
| 1.02 · Paso-01 §8 Website URL | Se define la URL principal de la web | https://www.cerrajerosmadrid24h.com | IA sin respaldo | No hay dato real aportado por el cliente. El dominio fue generado para el ejemplo y debe confirmarse antes de producción. |
| 1.03 · Paso-01 §8 Website URL | Se define el dominio canónico | https://www.cerrajerosmadrid24h.com | IA sin respaldo | Deriva del dominio de ejemplo. El sistema exige elegir entre opción A (con www) y opción B (sin www); la elección concreta no fue confirmada por input real. |

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

