# Paso 1 — Intake Form

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

## Bloque 1 — Identidad del negocio

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.01 · Paso-01 §7 Business Name | Se define el nombre del negocio | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | Cerrajeros Madrid 24h |
| 1.02 · Paso-01 §8 Website URL | Se define la URL principal de la web | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | https://www.cerrajerosmadrid24h.com |
| 1.03 · Paso-01 §8 Website URL | Se define el dominio canónico | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. La elección entre opción A (con www) y opción B (sin www) está pendiente de confirmar. | https://www.cerrajerosmadrid24h.com |

## Bloque 2 — Estado inicial del GBP

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.04 · Paso-01 §4 Lo que tienes que rellenar | Se decide el estado del GBP | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | GBP Status: Not Created |
| 1.05 · Paso-01 §4 Lo que tienes que rellenar | Se decide el momento de creación del GBP | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. El flujo web-first exige publicar la web antes de crear el GBP. | After website launch |
| 1.06 · Paso-01 §4 Lo que tienes que rellenar | Se decide el estado de verificación del GBP | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | GBP Verification Status: Not Started |
| 1.07 · Paso-01 §4 Lo que tienes que rellenar | Se decide que no hay GBP URL todavía | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Prohíbe inventar sameAs ni URL de GBP si el perfil no existe; el campo se deja en blanco hasta el Paso 14. | N/A — GBP not created yet |

## Bloque 3 — NAP y contacto

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.08 · Paso-01 §9 Full NAP | Se define el nombre NAP | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | Cerrajeros Madrid 24h |
| 1.09 · Paso-01 §9 Full NAP | Se define la dirección del negocio | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí |
| 1.10 · Paso-01 §9 Full NAP | Se define la ciudad del negocio | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. Se extrae directamente de la dirección. | Madrid |
| 1.11 · Paso-01 §9 Full NAP | Se define la provincia o comunidad | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. La provincia se incluye en el NAP completo proporcionado. | Comunidad de Madrid |
| 1.12 · Paso-01 §9 Full NAP | Se define el código postal | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. El código postal se incluye en el NAP completo proporcionado. | 28010 |
| 1.13 · Paso-01 §9 Full NAP | Se define el país | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | España |
| 1.14 · Paso-01 §9 Full NAP | Se define el teléfono del negocio | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | +34 600 000 000 |
| 1.15 · Paso-01 §9 Full NAP | Se define el email del negocio | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | info@cerrajerosmadrid24h.com |

## Bloque 4 — Categorías GBP planificadas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.16 · Paso-01 §10 Planned Primary GBP Category | Se define la categoría principal planificada para el futuro GBP | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Exige declarar categoría principal alineada con el negocio. La categoría concreta debe confirmarse como disponible en Google. | Cerrajero |
| 1.17 · Paso-01 §11 Planned Additional GBP Categories | Se define una categoría adicional planificada | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. Coherente con "24h" pero no confirmada como categoría GBP disponible. | Servicio de cerrajería de urgencia |
| 1.18 · Paso-01 §11 Planned Additional GBP Categories | Se define otra categoría adicional planificada | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | Servicio de duplicado de llaves |

## Bloque 5 — Dirección física, Main City y zonas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.19 · Paso-01 §9 Full NAP | Se define la dirección física como ancla del sistema | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. Se usa como ancla NAP para todo el ecosistema. | Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí, Madrid |
| 1.20 · Paso-01 §12 Main City | Se define la ciudad que crea la arquitectura base | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. Madrid sale directamente del dato de dirección. | Madrid |
| 1.21 · Paso-01 §13 Physical Location City | Se define la ciudad de ubicación física | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. Coincide con la Main City en este ejemplo. | Madrid |
| 1.22 · Paso-01 §15 Local Coverage Areas | Se define una Direct Local Coverage Area | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Direct Local Coverage Areas se extraen del ancla física del NAP según §35.1. Almagro aparece en la dirección como barrio. | Almagro |
| 1.23 · Paso-01 §15 Local Coverage Areas | Se define una Direct Local Coverage Area | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Direct Local Coverage Areas se extraen del ancla física del NAP según §35.1. Chamberí aparece en la dirección como distrito. | Chamberí |
| 1.24 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Candidate Local Coverage Areas se proponen siguiendo el test de coherencia GEO 3/6 (§34); requieren validación con datos de búsqueda o competidores antes de uso fuerte. | Salamanca |
| 1.25 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Candidate Local Coverage Areas se proponen siguiendo el test de coherencia GEO 3/6 (§34); requieren validación con datos de búsqueda o competidores antes de uso fuerte. | Retiro |
| 1.26 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Candidate Local Coverage Areas se proponen siguiendo el test de coherencia GEO 3/6 (§34); requieren validación con datos de búsqueda o competidores antes de uso fuerte. | Centro |
| 1.27 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Candidate Local Coverage Areas se proponen siguiendo el test de coherencia GEO 3/6 (§34); requieren validación con datos de búsqueda o competidores antes de uso fuerte. | Tetuán |
| 1.28 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Candidate Local Coverage Areas se proponen siguiendo el test de coherencia GEO 3/6 (§34); requieren validación con datos de búsqueda o competidores antes de uso fuerte. | Chamartín |
| 1.29 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Candidate Local Coverage Areas se proponen siguiendo el test de coherencia GEO 3/6 (§34); requieren validación con datos de búsqueda o competidores antes de uso fuerte. | Arganzuela |
| 1.30 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Candidate Local Coverage Areas se proponen siguiendo el test de coherencia GEO 3/6 (§34); requieren validación con datos de búsqueda o competidores antes de uso fuerte. | Moncloa |
| 1.31 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las Candidate Local Coverage Areas se proponen siguiendo el test de coherencia GEO 3/6 (§34); requieren validación con datos de búsqueda o competidores antes de uso fuerte. | Prosperidad |

## Bloque 6 — Expansión geográfica

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.32 · Paso-01 §16 Approved Expansion Areas | Se decide que las Local Coverage Areas no generarán páginas en la base | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. La estructura base es ciudad + servicio; las zonas se usan como señales GEO, no como URLs. | No, not in the base build |
| 1.33 · Paso-01 §16 Approved Expansion Areas | Se decide que no hay Approved Expansion Areas en la fase inicial | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. La expansión requiere aprobación y validación; las Approved Expansion Areas se dejan en blanco por defecto. | None in Phase 1 |

## Bloque 7 — Servicios principales

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.34 · Paso-01 §14 Servicios principales | Se define el servicio principal 1 | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. Servicio plausible por "24h" pero no confirmado por input, datos ni competencia. | Cerrajero urgente |
| 1.35 · Paso-01 §14 Servicios principales | Se define el servicio principal 2 | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | Apertura de puertas |
| 1.36 · Paso-01 §14 Servicios principales | Se define el servicio principal 3 | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | Cambio de cerraduras |
| 1.37 · Paso-01 §14 Servicios principales | Se define el servicio principal 4 | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | Cambio de bombines |
| 1.38 · Paso-01 §14 Servicios principales | Se define el servicio principal 5 | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | Instalación de cerraduras de seguridad |

## Bloque 8 — Consolidación de categorías adicionales

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.39 · Paso-01 §21 Categorías adicionales clasificadas | Se decide que una categoría adicional ya está cubierta por un servicio principal | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Si una categoría adicional ya está cubierta por un servicio core, no genera página propia. | Servicio de cerrajería de urgencia queda cubierta por Cerrajero urgente |
| 1.40 · Paso-01 §21 Categorías adicionales clasificadas | Se decide que una categoría adicional necesita página propia | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. La regla de clasificación es GMB Crush, pero la categoría concreta "duplicado de llaves" está pendiente de validación. | Servicio de duplicado de llaves |

## Bloque 9 — Contenido, conversión y confianza

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.41 · Paso-01 §15 Local Coverage Areas | Se define el número de GeoArticles por servicio | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. El default operativo del framework es 3 ideas por Service × City pair. | 3 |
| 1.42 · Paso-01 §17 Preferred CTA | Se define el CTA principal | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | Llamar ahora |
| 1.43 · Paso-01 §18 Trust Signals | Se define una señal de confianza | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | 10+ años de experiencia |
| 1.44 · Paso-01 §18 Trust Signals | Se define una señal de confianza pendiente del futuro GBP | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Prohíbe inventar reseñas antes de tener GBP real; se recopilan tras crear y verificar el perfil en el Paso 14. | Reseñas iniciales pendientes de recopilar tras crear y verificar el GBP |
| 1.45 · Paso-01 §18 Trust Signals | Se define una señal de confianza | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | Técnicos cerrajeros cualificados |
| 1.46 · Paso-01 §18 Trust Signals | Se define una señal de confianza | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | Servicio móvil en el mismo día |
| 1.47 · Paso-01 §18 Trust Signals | Se define una señal de confianza | IA sin respaldo | Valor generado para el ejemplo sin dato real ni regla aplicable. Debe sustituirse con dato real antes de producción. | Garantía de trabajo |
