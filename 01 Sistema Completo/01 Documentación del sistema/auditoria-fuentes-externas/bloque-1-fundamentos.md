# Auditoría de fuentes externas — Bloque 1 Fundamentos

Audit de las decisiones cuya Fuente contiene `Competidores` o `Datos de búsqueda` en el Bloque 1. Se cruza cada fila con su `§X` canónica del ejecutable para validar si la doctrina realmente define el método de extracción del valor desde la fuente externa.

---

## Alcance

```text
Bloque 1 — Fundamentos:
  paso-01-intake-form         → 14 filas (4 grupos)
  paso-02-formula-maestra     → 0 filas
  paso-03-matriz-base         → 15 filas (1 grupo)

Total Bloque 1: 29 filas en 5 grupos.
```

---

## Estados

```text
✅ DEFINIDO  — la §X canónica describe el método de extracción de la fuente externa.
⚠️ VAGO     — la §X menciona la fuente pero no detalla cómo aplicarla.
❌ AUSENTE  — la §X no menciona la fuente ni el método de extracción.
```

---

## Auditoría por grupo

### Grupo A — Categoría principal del GBP planificada

| Filas | Decisión | Fuente | §X canónica |
|---|---|---|---|
| 1.16 | Categoría principal del GBP planificada | GMB Crush + Competidores | paso-01 §10 Planned Primary GBP Category |

**Qué dice §10 hoy:**

> "La categoría principal del GBP manda sobre la arquitectura. Los servicios y páginas deben apoyar esa categoría. Patrón: `Planned Primary GBP Category → Primary Category Slug → Service Pages`. Regla final: la categoría principal debe verse reflejada en homepage, servicios y páginas locales."

**Veredicto:** ❌ **AUSENTE.** §10 dice qué hace la categoría principal, pero no dice cómo escogerla. No menciona competidores, Local Pack ni método de extracción.

**Propuesta de mejora — añadir a §10 una subsección "Método":**

```text
§10.6 Método (extraer de competidores)

1. Buscar en Google Maps "[servicio principal] [main city]" sin login.
2. Anotar las categorías primarias declaradas por los 5 negocios mejor
   posicionados en el Local Pack.
3. Seleccionar la categoría que más se repite (>3 de 5) como Primary
   Category Planned. Si hay empate, priorizar la más amplia (categoría
   madre del catálogo GBP).
4. Validar contra el catálogo oficial de GBP. Si la categoría no existe
   exactamente, escoger la más próxima del catálogo.
```

---

### Grupo B — Categorías adicionales del GBP planificadas

| Filas | Decisión | Fuente | §X canónica |
|---|---|---|---|
| 1.17 | Categoría adicional planificada | GMB Crush + Competidores | paso-01 §11 Planned Additional GBP Categories |
| 1.18 | Categoría adicional planificada | GMB Crush + Competidores | paso-01 §11 Planned Additional GBP Categories |

**Qué dice §11 hoy:**

> "Las categorías adicionales refuerzan la profundidad de entidad, pero no siempre generan páginas nuevas si ya están cubiertas por un core service. Patrón: `Additional Category → covered or separate page`. Regla final: cada categoría adicional se consolida o se convierte en página, pero nunca se duplica."

**Veredicto:** ❌ **AUSENTE.** §11 explica qué hacer con las categorías adicionales (consolidar vs página propia), pero no dice cómo encontrarlas. No menciona competidores.

**Propuesta de mejora — añadir a §11 una subsección "Método":**

```text
§11.6 Método (extraer de competidores)

1. Tras escoger la Primary Category (§10), revisar las "categorías
   adicionales" declaradas por los mismos 5 competidores top.
2. Listar todas las categorías secundarias que aparecen en al menos 2 de
   los 5 competidores.
3. Filtrar las que el cliente realmente ofrece (cruce con servicios
   reales). Las que no ofrece se descartan.
4. Aplicar la regla de consolidación (§11.5): si una categoría adicional
   coincide con un core service, se marca cubierta. Si no, se marca como
   "necesita página".
```

---

### Grupo C — Candidate Local Coverage Areas

| Filas | Decisión | Fuente | §X canónica |
|---|---|---|---|
| 1.24–1.31 | Candidate Local Coverage Area (8 zonas) | GMB Crush + Competidores | paso-01 §15 Local Coverage Areas |

**Qué dice §15 hoy:**

> "Son zonas seleccionadas por proximidad al NAP, coherencia GEO y lógica GMB Crush. Incluyen barrios, distritos, municipios cercanos o áreas de servicio. Se clasifican en Direct (salen del ancla física) y Candidate (requieren validación GEO). No generan URLs por defecto."

**Veredicto:** ⚠️ **VAGO.** §15 menciona "lógica GMB Crush" como input pero no detalla el papel de competidores. El test GEO 3/6 (§34) sí está definido, pero no se conecta explícitamente con extraer Candidates de competidores.

**Propuesta de mejora — añadir a §15 una subsección "Método de Candidates":**

```text
§15.6 Método (extraer Candidate LCAs de competidores)

1. Tras fijar las Direct LCAs (que salen del NAP, §15 y §34), revisar
   las áreas de servicio declaradas por los 3-5 competidores top en
   Google Maps.
2. Listar todas las zonas (barrios, distritos, municipios) que
   aparecen en al menos 2 competidores y NO están ya en Direct.
3. Para cada zona candidata, aplicar el test de coherencia GEO 3/6
   (§34). Si pasa 3 de 6 criterios, queda como Candidate validable.
   Si no, se descarta.
4. Las Candidate aprobadas entran como contenido en LBS, GeoHub y
   GeoArticles. Solo generan URL si pasan a Approved Expansion (§16).
```

---

### Grupo D — Servicios principales (core services)

| Filas | Decisión | Fuente | §X canónica |
|---|---|---|---|
| 1.34–1.38 | Servicio principal (5 core services) | GMB Crush + Competidores | paso-01 §14 Servicios principales |

**Qué dice §14 hoy:**

> "Los core services son los servicios principales que generan Service Overview Pages y Páginas de servicio en la Main City. Patrón: `S = número de core services`. Regla final: cada core service importante debe tener página propia."

**Veredicto:** ❌ **AUSENTE.** §14 define qué son los core services y qué generan, pero no dice cómo identificarlos. No menciona competidores ni Local Pack.

**Propuesta de mejora — añadir a §14 una subsección "Método":**

```text
§14.6 Método (extraer de competidores)

1. Buscar en Google Maps "[categoría principal] [main city]" y abrir
   los 5 perfiles GBP mejor posicionados del Local Pack.
2. En cada perfil, abrir la sección "Servicios" del GBP y listar los
   servicios declarados.
3. Contar la frecuencia de cada servicio entre los 5 competidores.
   Seleccionar los 5 servicios más frecuentes (top 5 por frecuencia).
4. Cruzar con la oferta real del cliente. Si el cliente no ofrece uno
   de los servicios top, sustituirlo por el siguiente más frecuente
   que sí ofrezca.
5. Si hay empate de frecuencia, priorizar el servicio con más volumen
   de búsqueda local (cruce con keyword research).
```

---

### Grupo E — Trust signals

| Filas | Decisión | Fuente | §X canónica |
|---|---|---|---|
| 1.43, 1.45, 1.46, 1.47 | Trust signal (4 señales reales) | GMB Crush + Competidores | paso-01 §18 Trust Signals |

**Qué dice §18 hoy:**

> "Las señales de confianza ayudan al usuario, a Google y a sistemas de IA a validar autoridad. Patrón: `Reviews + years + certifications + guarantees`. Regla final: los trust signals deben ser reales y reutilizables."

**Veredicto:** ⚠️ **VAGO.** §18 lista qué tipos de trust signals son válidos (años, certificaciones, garantías…) pero no dice cómo benchmarkearlos contra competidores. El cliente puede mencionar 3 trust signals genéricos sin saber cuáles son los más diferenciadores en su sector.

**Propuesta de mejora — añadir a §18 una subsección "Método":**

```text
§18.6 Método (benchmark contra competidores)

1. Revisar las homepages y LBS de los 5 competidores top del Local Pack.
2. Listar los trust signals que aparecen en al menos 3 de los 5
   competidores (el "estándar" del sector).
3. Listar los trust signals que aparecen en 1 o 2 competidores (los
   "diferenciadores" que pocos usan).
4. Confirmar con el cliente cuáles puede acreditar como reales (años,
   certificaciones, garantías, equipo cualificado). Filtrar los que
   no puede demostrar.
5. Output: 3-5 trust signals que sean del estándar del sector + 1-2
   diferenciadores acreditables.
```

---

### Grupo F — Topics de GeoArticles

| Filas | Decisión | Fuente | §X canónica |
|---|---|---|---|
| 3.19–3.33 | GeoArticle topic (15 artículos) | GMB Crush + Datos de búsqueda | paso-03 §7 Regla 1 — Cada página tiene una fila |

**Qué dice paso-03 §7 hoy:**

> "Regla 1 — Cada página tiene una fila. La matriz base convierte arquitectura en producción. Si una página no tiene fila, no existe dentro del sistema operativo. Patrón: `One URL = one row = one page type = one function`. Regla final: toda página publicada debe existir primero en la matriz."

**Veredicto:** ❌ **AUSENTE.** paso-03 §7 es una regla matriz genérica (cada página tiene fila), no dice nada específico sobre cómo escoger topics de GeoArticles ni menciona keyword research.

**Problema crítico:** la referencia canónica que pusimos en los `Xb` para los GeoArticles apunta a `§7` que es genérico. Falta una `§X` específica que defina el método.

**Propuesta de mejora — opciones:**

```text
Opción A: añadir §X específica en paso-03 (ej. §16 GeoArticle Topics).
Opción B: mover la referencia canónica de los GeoArticles del Xb del
          paso-03 a paso-15 §14, donde sí hay método.

Lo cierto es que la fórmula maestra de paso-02 fija G=3 GeoArticles
por servicio core, pero ningún §X define cómo extraer los 3 topics
concretos por servicio.
```

**Propuesta de método (a colocar en la §X que se decida):**

```text
§X.Y Método para topics de GeoArticles (15 = G × S)

1. Por cada core service (paso 1.34-1.38), ejecutar keyword research
   con volumen ≥ X impresiones/mes y dificultad ≤ Y.
2. Filtrar queries con intent informativo (cómo, qué, cuándo, por qué,
   cuánto, mejor) que NO coincidan con la query de la LBS (intent
   transaccional).
3. Por servicio, seleccionar G topics (G=3 por defecto, ver paso-02 §11)
   priorizando: alto volumen + bajo competencia + complemento al LBS
   (no canibalización).
4. Si hay menos de G topics con volumen suficiente, usar topics con
   intent local ("[query] en [main city]") como fallback.
5. Slug del topic: la propia query como base, normalizada
   (paso-04 §17-§19).
```

---

## Resumen del Bloque 1

```text
Total grupos auditados:   6
Estado ✅ DEFINIDO:        0
Estado ⚠️ VAGO:            2 (Candidate LCAs §15, Trust signals §18)
Estado ❌ AUSENTE:         4 (Categoría principal §10, Categorías adicionales §11,
                              Servicios core §14, Topics GeoArticles paso-03 §7)
```

**Acción recomendada:** añadir una subsección `§X.6 Método` (o equivalente) a las 6 secciones canónicas afectadas. Sin esto, las 29 filas del Bloque 1 marcadas con `Competidores` o `Datos de búsqueda` no tienen método operativo definido en el sistema y dependen del operador para improvisar.

**Nota sobre paso-03 §7:** la referencia canónica de los GeoArticles está mal apuntada — debería existir un `§X` específico para topics con método de keyword research, o moverse al paso-15 §14 donde sí hay estructura.
