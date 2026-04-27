# Paso 1 — Intake Form

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

## Bloque 1 — Identidad del negocio

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.01 · Paso-01 §7 Business Name | Se define el nombre del negocio | Input humano | El cliente proporciona el nombre del negocio directamente. El sistema lo recoge sin transformación. | Cerrajeros Madrid 24h |
| 1.02 · Paso-01 §8 Website URL | Se define la URL principal de la web | IA sin respaldo | No hay dato real aportado por el cliente. El dominio fue generado para el ejemplo y debe confirmarse antes de producción. | https://www.cerrajerosmadrid24h.com |
| 1.03 · Paso-01 §8 Website URL | Se define el dominio canónico | IA sin respaldo | Deriva del dominio de ejemplo. El sistema exige elegir entre opción A (con www) y opción B (sin www); la elección concreta no fue confirmada por input real. | https://www.cerrajerosmadrid24h.com |

## Bloque 2 — Estado inicial del GBP

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.04 · Paso-01 §4 Lo que tienes que rellenar | Se decide el estado del GBP | Input humano | El cliente indica si el GBP existe o no. El sistema no asume ningún estado por defecto. | GBP Status: Not Created |
| 1.05 · Paso-01 §4 Lo que tienes que rellenar | Se decide el momento de creación del GBP | Input humano + GMB Crush | El cliente define el flujo; GMB Crush establece que la web debe estar publicada antes de crear el GBP en el flujo web-first. | After website launch |
| 1.06 · Paso-01 §4 Lo que tienes que rellenar | Se decide el estado de verificación del GBP | Input humano | Si el GBP no existe, la verificación no ha empezado. El sistema lo registra como dato de partida. | GBP Verification Status: Not Started |
| 1.07 · Paso-01 §4 Lo que tienes que rellenar | Se decide que no hay GBP URL todavía | GMB Crush | GMB Crush prohíbe inventar sameAs ni URL de GBP si el perfil no existe. El campo se deja en blanco hasta el Paso 14. | N/A — GBP not created yet |

## Bloque 3 — NAP y contacto

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.08 · Paso-01 §9 Full NAP | Se define el nombre NAP | Input humano | El nombre NAP debe coincidir exactamente con el nombre del negocio proporcionado por el cliente. | Cerrajeros Madrid 24h |
| 1.09 · Paso-01 §9 Full NAP | Se define la dirección del negocio | Input humano | El cliente proporciona la dirección física. El sistema la usa como ancla NAP y señal de ubicación. | Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí |
| 1.10 · Paso-01 §9 Full NAP | Se define la ciudad del negocio | Input humano | Se extrae directamente de la dirección proporcionada. | Madrid |
| 1.11 · Paso-01 §9 Full NAP | Se define la provincia o comunidad | Geografía | Se infiere territorialmente desde la ciudad. Conviene confirmar el formato administrativo final. | Comunidad de Madrid |
| 1.12 · Paso-01 §9 Full NAP | Se define el código postal | Geografía | Se infiere para la zona de Almagro/Chamberí. Debe verificarse contra la dirección exacta. | 28010 |
| 1.13 · Paso-01 §9 Full NAP | Se define el país | Input humano | El contexto y la dirección son de Madrid, España. | España |
| 1.14 · Paso-01 §9 Full NAP | Se define el teléfono del negocio | IA sin respaldo | Teléfono placeholder generado para el ejemplo. No consta dato real aportado por el cliente. | +34 600 000 000 |
| 1.15 · Paso-01 §9 Full NAP | Se define el email del negocio | IA sin respaldo | Email derivado del dominio de ejemplo. No consta como dato real aportado por el cliente. | info@cerrajerosmadrid24h.com |

## Bloque 4 — Categorías GBP planificadas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.16 · Paso-01 §10 Planned Primary GBP Category | Se define la categoría principal planificada para el futuro GBP | Input humano + GMB Crush | El nombre del negocio indica cerrajería; GMB Crush requiere categoría principal para alinear web y GBP. Debe confirmarse como categoría disponible en Google. | Cerrajero |
| 1.17 · Paso-01 §11 Planned Additional GBP Categories | Se define una categoría adicional planificada | IA sin respaldo | Coherente con "24h" pero no confirmada como categoría GBP disponible ni validada con datos de búsqueda. | Servicio de cerrajería de urgencia |
| 1.18 · Paso-01 §11 Planned Additional GBP Categories | Se define otra categoría adicional planificada | IA sin respaldo | Servicio típico de cerrajería pero no confirmado por input ni datos. Pendiente de validación con datos reales. | Servicio de duplicado de llaves |

## Bloque 5 — Dirección física, Main City y zonas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.19 · Paso-01 §9 Full NAP | Se define la dirección física como ancla del sistema | Input humano | La dirección fue proporcionada por el cliente y el sistema la usa como ancla NAP para todo el ecosistema. | Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí, Madrid |
| 1.20 · Paso-01 §12 Main City | Se define la ciudad que crea la arquitectura base | Input humano | Madrid sale directamente del dato de dirección. Es la Main City sobre la que se construye toda la arquitectura URL. | Madrid |
| 1.21 · Paso-01 §13 Physical Location City | Se define la ciudad de ubicación física | Input humano | La ubicación física está en Madrid según el dato aportado. Coincide con la Main City en este ejemplo. | Madrid |
| 1.22 · Paso-01 §15 Local Coverage Areas | Se define una Direct Local Coverage Area | Input humano + Geografía | Almagro aparece en la dirección como barrio. Las Direct LCA salen de la dirección física sin necesidad de validación adicional. | Almagro |
| 1.23 · Paso-01 §15 Local Coverage Areas | Se define una Direct Local Coverage Area | Input humano + Geografía | Chamberí aparece en la dirección como distrito. Las Direct LCA salen de la dirección física sin necesidad de validación adicional. | Chamberí |
| 1.24 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | Geografía | Zona candidata por proximidad urbana. Requiere test GEO o datos de búsqueda antes de usarla como señal fuerte. | Salamanca |
| 1.25 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | Geografía | Zona candidata por contexto Madrid. Requiere validación de coherencia GEO. | Retiro |
| 1.26 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | Geografía | Zona candidata. Requiere validación de proximidad, demanda y competencia. | Centro |
| 1.27 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | Geografía | Zona candidata. Requiere validación de proximidad, demanda y competencia. | Tetuán |
| 1.28 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | Geografía | Zona candidata. Requiere validación de proximidad, demanda y competencia. | Chamartín |
| 1.29 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | Geografía | Zona candidata. Requiere validación de proximidad, demanda y competencia. | Arganzuela |
| 1.30 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | Geografía | Zona candidata. Requiere validación de proximidad, demanda y competencia. | Moncloa |
| 1.31 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | Geografía | Zona candidata. Requiere validación de proximidad, demanda y competencia. | Prosperidad |

## Bloque 6 — Expansión geográfica

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.32 · Paso-01 §16 Approved Expansion Areas | Se decide que las Local Coverage Areas no generarán páginas en la base | GMB Crush | GMB Crush establece que la estructura base es ciudad + servicio. Las zonas y barrios se usan como señales GEO, no como URLs, salvo expansión aprobada explícitamente. | No, not in the base build |
| 1.33 · Paso-01 §16 Approved Expansion Areas | Se decide que no hay Approved Expansion Areas en la fase inicial | GMB Crush | La expansión requiere aprobación y validación. La base se centra en Main City. Las Approved Expansion Areas se dejan en blanco por defecto. | None in Phase 1 |

## Bloque 7 — Servicios principales

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.34 · Paso-01 §14 Servicios principales | Se define el servicio principal 1 | IA sin respaldo | Servicio plausible por "24h" pero no confirmado por input del cliente, datos de búsqueda ni análisis de competencia. | Cerrajero urgente |
| 1.35 · Paso-01 §14 Servicios principales | Se define el servicio principal 2 | IA sin respaldo | Servicio típico de cerrajería pero no confirmado por input, datos ni competencia. | Apertura de puertas |
| 1.36 · Paso-01 §14 Servicios principales | Se define el servicio principal 3 | IA sin respaldo | Servicio típico de cerrajería pero no confirmado por input, datos ni competencia. | Cambio de cerraduras |
| 1.37 · Paso-01 §14 Servicios principales | Se define el servicio principal 4 | IA sin respaldo | Servicio típico de cerrajería pero no confirmado por input, datos ni competencia. | Cambio de bombines |
| 1.38 · Paso-01 §14 Servicios principales | Se define el servicio principal 5 | IA sin respaldo | Servicio típico de cerrajería pero no confirmado por input, datos ni competencia. | Instalación de cerraduras de seguridad |

## Bloque 8 — Consolidación de categorías adicionales

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.39 · Paso-01 §21 Categorías adicionales clasificadas | Se decide que una categoría adicional ya está cubierta por un servicio principal | GMB Crush | GMB Crush establece que si una categoría adicional ya está cubierta por un servicio core, no genera página propia. Evita duplicar intenciones. | Servicio de cerrajería de urgencia queda cubierta por Cerrajero urgente |
| 1.40 · Paso-01 §21 Categorías adicionales clasificadas | Se decide que una categoría adicional necesita página propia | GMB Crush + IA sin respaldo | GMB Crush exige soporte web para cada categoría adicional efectiva. La categoría concreta está pendiente de validación. | Servicio de duplicado de llaves |

## Bloque 9 — Contenido, conversión y confianza

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.41 · Paso-01 §18 Trust Signals | Se define el número de GeoArticles por servicio | GMB Crush | El framework de GeoArticles establece 3 ideas por Service × City pair. Es una regla fija del sistema. | 3 |
| 1.42 · Paso-01 §17 Preferred CTA | Se define el CTA principal | IA sin respaldo | CTA plausible para cerrajería pero no confirmado por el negocio. Debe validarse con el cliente antes de producción. | Llamar ahora |
| 1.43 · Paso-01 §18 Trust Signals | Se define una señal de confianza | IA sin respaldo | No consta input ni prueba que confirme los años de experiencia. Dato generado para el ejemplo. | 10+ años de experiencia |
| 1.44 · Paso-01 §18 Trust Signals | Se define una señal de confianza pendiente del futuro GBP | GMB Crush | GMB Crush prohíbe inventar reseñas antes de tener GBP real. Las reseñas se recopilan después de crear y verificar el perfil en el Paso 14. | Reseñas iniciales pendientes de recopilar tras crear y verificar el GBP |
| 1.45 · Paso-01 §18 Trust Signals | Se define una señal de confianza | IA sin respaldo | No consta confirmación del negocio. Pendiente de validación con el cliente. | Técnicos cerrajeros cualificados |
| 1.46 · Paso-01 §18 Trust Signals | Se define una señal de confianza | IA sin respaldo | No consta confirmación operativa del negocio. Pendiente de validación con el cliente. | Servicio móvil en el mismo día |
| 1.47 · Paso-01 §18 Trust Signals | Se define una señal de confianza | IA sin respaldo | No consta confirmación del negocio. Pendiente de validación con el cliente. | Garantía de trabajo |
