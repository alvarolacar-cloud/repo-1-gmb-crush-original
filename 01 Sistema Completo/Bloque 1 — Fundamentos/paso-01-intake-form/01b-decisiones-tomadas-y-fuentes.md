# Paso 1 — Intake Form

Fase 2 de trazabilidad del sistema GMB Crush.

Fuentes permitidas:

```text
GMB Crush
Input humano
Decisión de diseño
IA sin respaldo
IA heredada (paso X.YY)
```

Orígenes del dato permitidos:

```text
Doctrina GMB Crush
Input humano
Competidores
Datos de búsqueda
Decisión de diseño
Heredado del paso X.YY
IA sin respaldo
```

---

## Bloque 1 — Identidad del negocio

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 1.01 · Paso-01 §7 Business Name | Se define el nombre del negocio | Input humano | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | Cerrajeros Madrid 24h |
| 1.02 · Paso-01 §8 Website URL | Se define la URL principal de la web | Input humano | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | https://www.cerrajerosmadrid24h.com |
| 1.03 · Paso-01 §8 Website URL | Se define el dominio canónico | Input humano | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | https://www.cerrajerosmadrid24h.com |

## Bloque 2 — Estado inicial del GBP

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 1.04 · Paso-01 §4 Lo que tienes que rellenar | Se decide el estado del GBP | Input humano | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | GBP Status: Not Created |
| 1.05 · Paso-01 §4 Lo que tienes que rellenar | Se decide el momento de creación del GBP | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Web-first: GBP en Paso 14. | After website launch |
| 1.06 · Paso-01 §4 Lo que tienes que rellenar | Se decide el estado de verificación del GBP | Input humano | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | Not Started |
| 1.07 · Paso-01 §4 Lo que tienes que rellenar | Se decide que no hay GBP URL todavía | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Prohíbe inventar GBP URL antes del Paso 14. | N/A — GBP not created yet |

## Bloque 3 — NAP y contacto

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 1.08 · Paso-01 §9 Full NAP | Se define el nombre NAP | Input humano | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | Cerrajeros Madrid 24h |
| 1.09 · Paso-01 §9 Full NAP | Se define la dirección del negocio | Input humano | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí |
| 1.10 · Paso-01 §9 Full NAP | Se define la ciudad del negocio | Input humano | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | Madrid |
| 1.11 · Paso-01 §9 Full NAP | Se define la provincia o comunidad | GMB Crush | Input humano | El framework define que el NAP completo debe incluir provincia. Se aplica igual en todos los proyectos. El valor sale del NAP proporcionado por el cliente. | Comunidad de Madrid |
| 1.12 · Paso-01 §9 Full NAP | Se define el código postal | Input humano | IA sin respaldo | El cliente proporciona este dato directamente. En el ejemplo actual el código postal concreto es placeholder y requiere verificación contra la dirección real. | 28010 |
| 1.13 · Paso-01 §9 Full NAP | Se define el país | Input humano | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | España |
| 1.14 · Paso-01 §9 Full NAP | Se define el teléfono del negocio | Input humano | IA sin respaldo | El cliente proporciona este dato directamente en producción real. En el ejemplo actual es placeholder; debe sustituirse por el teléfono real antes de producción. | +34 600 000 000 |
| 1.15 · Paso-01 §9 Full NAP | Se define el email del negocio | Input humano | IA sin respaldo | El cliente proporciona este dato directamente en producción real. En el ejemplo actual es placeholder; debe sustituirse por el email real antes de producción. | info@cerrajerosmadrid24h.com |

## Bloque 4 — Categorías GBP planificadas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 1.16 · Paso-01 §10 Planned Primary GBP Category | Se define la categoría principal planificada para el futuro GBP | GMB Crush | Competidores | El framework define que la categoría principal del GBP rige toda la arquitectura. La metodología exige análisis del Local Pack para identificar la categoría correcta; pendiente de validación. | Cerrajero |
| 1.17 · Paso-01 §11 Planned Additional GBP Categories | Se define una categoría adicional planificada | GMB Crush | Competidores | El framework exige analizar categorías adicionales del GBP que ofrecen los competidores. Pendiente de validación con análisis del Local Pack. | Servicio de cerrajería de urgencia |
| 1.18 · Paso-01 §11 Planned Additional GBP Categories | Se define otra categoría adicional planificada | GMB Crush | Competidores | El framework exige analizar categorías adicionales del GBP que ofrecen los competidores. Pendiente de validación con análisis del Local Pack. | Servicio de duplicado de llaves |

## Bloque 5 — Dirección física, Main City y zonas

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 1.19 · Paso-01 §9 Full NAP | Se define la dirección física como ancla del sistema | GMB Crush | Input humano | El framework define que la dirección física es ancla NAP del ecosistema. El valor sale del cliente. | Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí, Madrid |
| 1.20 · Paso-01 §12 Main City | Se define la ciudad que crea la arquitectura base | GMB Crush | Input humano | El framework exige una sola Main City que crea la arquitectura base. El valor sale del NAP del cliente. | Madrid |
| 1.21 · Paso-01 §13 Physical Location City | Se define la ciudad de ubicación física | Input humano | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | Madrid |
| 1.22 · Paso-01 §15 Local Coverage Areas | Se define una Direct Local Coverage Area | GMB Crush | Input humano | El framework define que las Direct LCAs salen del ancla física del NAP (§35.1). Almagro aparece en la dirección como barrio. | Almagro |
| 1.23 · Paso-01 §15 Local Coverage Areas | Se define una Direct Local Coverage Area | GMB Crush | Input humano | El framework define que las Direct LCAs salen del ancla física del NAP (§35.1). Chamberí aparece en la dirección como distrito. | Chamberí |
| 1.24 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | Competidores | El framework define el test de coherencia GEO 3/6 (§34) para Candidate LCAs. La validación combina proximidad geográfica + competidores que cubren la zona; pendiente de ejecutar. | Salamanca |
| 1.25 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | Competidores | El framework define el test de coherencia GEO 3/6 (§34). Pendiente de ejecutar. | Retiro |
| 1.26 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | Competidores | El framework define el test de coherencia GEO 3/6 (§34). Pendiente de ejecutar. | Centro |
| 1.27 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | Competidores | El framework define el test de coherencia GEO 3/6 (§34). Pendiente de ejecutar. | Tetuán |
| 1.28 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | Competidores | El framework define el test de coherencia GEO 3/6 (§34). Pendiente de ejecutar. | Chamartín |
| 1.29 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | Competidores | El framework define el test de coherencia GEO 3/6 (§34). Pendiente de ejecutar. | Arganzuela |
| 1.30 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | Competidores | El framework define el test de coherencia GEO 3/6 (§34). Pendiente de ejecutar. | Moncloa |
| 1.31 · Paso-01 §15 Local Coverage Areas | Se define una Candidate Local Coverage Area | GMB Crush | Competidores | El framework define el test de coherencia GEO 3/6 (§34). Pendiente de ejecutar. | Prosperidad |

## Bloque 6 — Expansión geográfica

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 1.32 · Paso-01 §16 Approved Expansion Areas | Se decide que las Local Coverage Areas no generarán páginas en la base | GMB Crush | Doctrina GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. | No, not in the base build |
| 1.33 · Paso-01 §16 Approved Expansion Areas | Se decide que no hay Approved Expansion Areas en la fase inicial | GMB Crush | Doctrina GMB Crush | El framework define esta regla. La expansión requiere aprobación explícita. | None in Phase 1 |

## Bloque 7 — Servicios principales

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 1.34 · Paso-01 §14 Servicios principales | Se define el servicio principal 1 | GMB Crush | Competidores | El framework dicta identificar los servicios core mediante análisis del Local Pack. Pendiente de validación con los 3 negocios competidores en Madrid. | Cerrajero urgente |
| 1.35 · Paso-01 §14 Servicios principales | Se define el servicio principal 2 | GMB Crush | Competidores | El framework dicta identificar los servicios core mediante análisis del Local Pack. Pendiente de validación. | Apertura de puertas |
| 1.36 · Paso-01 §14 Servicios principales | Se define el servicio principal 3 | GMB Crush | Competidores | El framework dicta identificar los servicios core mediante análisis del Local Pack. Pendiente de validación. | Cambio de cerraduras |
| 1.37 · Paso-01 §14 Servicios principales | Se define el servicio principal 4 | GMB Crush | Competidores | El framework dicta identificar los servicios core mediante análisis del Local Pack. Pendiente de validación. | Cambio de bombines |
| 1.38 · Paso-01 §14 Servicios principales | Se define el servicio principal 5 | GMB Crush | Competidores | El framework dicta identificar los servicios core mediante análisis del Local Pack. Pendiente de validación. | Instalación de cerraduras de seguridad |

## Bloque 8 — Consolidación de categorías adicionales

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 1.39 · Paso-01 §21 Categorías adicionales clasificadas | Se decide que una categoría adicional ya está cubierta por un servicio principal | GMB Crush | Doctrina GMB Crush | El framework define la regla de consolidación: si una categoría adicional ya está cubierta por un servicio core, no genera página propia. | Servicio de cerrajería de urgencia queda cubierta por Cerrajero urgente |
| 1.40 · Paso-01 §21 Categorías adicionales clasificadas | Se decide que una categoría adicional necesita página propia | GMB Crush | Heredado del paso 1.18 | El framework dicta la clasificación. El valor concreto (Servicio de duplicado de llaves) viene heredado del paso 1.18. | Servicio de duplicado de llaves |

## Bloque 9 — Contenido, conversión y confianza

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 1.41 · Paso-01 §15 Local Coverage Areas | Se define el número de GeoArticles por servicio | GMB Crush | Doctrina GMB Crush | El framework establece el default operativo G=3 ideas por Service × City pair. | 3 |
| 1.42 · Paso-01 §17 Preferred CTA | Se define el CTA principal | Decisión de diseño | Decisión de diseño | El operador o agencia toma esta decisión basándose en criterios de UX, conversión y mejores prácticas del sector. Para Cerrajeros Madrid 24h se elige "Llamar ahora" por la naturaleza urgente del servicio. | Llamar ahora |
| 1.43 · Paso-01 §18 Trust Signals | Se define una señal de confianza | GMB Crush | Competidores | El framework exige trust signals reales y reutilizables (§18). El valor concreto ("10+ años") requiere benchmark sectorial vs competidores; pendiente de validación. | 10+ años de experiencia |
| 1.44 · Paso-01 §18 Trust Signals | Se define una señal de confianza pendiente del futuro GBP | GMB Crush | Doctrina GMB Crush | El framework prohíbe inventar reseñas antes de tener GBP real (regla web-first). | Reseñas iniciales pendientes de recopilar tras crear y verificar el GBP |
| 1.45 · Paso-01 §18 Trust Signals | Se define una señal de confianza | GMB Crush | Competidores | El framework exige trust signals reales y reutilizables (§18). Pendiente de validación con benchmark sectorial. | Técnicos cerrajeros cualificados |
| 1.46 · Paso-01 §18 Trust Signals | Se define una señal de confianza | GMB Crush | Competidores | El framework exige trust signals reales y reutilizables (§18). Pendiente de validación con benchmark sectorial. | Servicio móvil en el mismo día |
| 1.47 · Paso-01 §18 Trust Signals | Se define una señal de confianza | GMB Crush | Competidores | El framework exige trust signals reales y reutilizables (§18). Pendiente de validación con benchmark sectorial. | Garantía de trabajo |
