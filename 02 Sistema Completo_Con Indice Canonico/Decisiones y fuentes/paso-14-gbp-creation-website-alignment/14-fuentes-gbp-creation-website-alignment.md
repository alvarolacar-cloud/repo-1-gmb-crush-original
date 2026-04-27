# Paso 14 — GBP Creation & Website Alignment

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

## Bloque 1 — Momento de creación y estado inicial

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 14.01 · Paso-14 §7 Crear GBP después de publicar web base | Crear GBP después de publicar web base | Input humano + GMB Crush | El flujo web-first está acordado con el cliente. La web debe estar publicada y soportar el GBP antes de crearlo. | After website launch |
| 14.02 · Paso-14 §4 Lo que tienes que rellenar | Estado inicial del GBP | Input humano | El estado Not Created es confirmado por el cliente. Determina qué pasos del Paso 14 están activos. | Not Created |
| 14.03 · Paso-14 §29 Cola de actualización post-GBP | Sincronizar GBP, web, schema y tracking al final | GMB Crush | El Paso 14 es el cierre del sistema. GBP, web y schema deben quedar alineados antes de dar el sistema por operativo. | Paso 14 como cierre |

## Bloque 2 — NAP, modelo y dirección

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 14.04 · Paso-14 §9 Validar NAP final antes de crear perfil | NAP final para el GBP | Input humano + IA sin respaldo | Nombre y dirección son válidos y aportados por el cliente. El teléfono es un placeholder no validado en el ejemplo. | Cerrajeros Madrid 24h + Calle Rafael Calvo 12 + Madrid + teléfono |
| 14.05 · Paso-14 §10 Elegir modelo de negocio correcto | Modelo de negocio | IA sin respaldo | El modelo SAB es plausible para un cerrajero, pero no está confirmado por el cliente. Debe validarse en ejecución. | Service Area Business |
| 14.06 · Paso-14 §9 Validar NAP final antes de crear perfil | Dirección física | Input humano | Dirección aportada directamente por el cliente. | Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí, Madrid |
| 14.07 · Paso-14 §10 Elegir modelo de negocio correcto | Mostrar dirección públicamente depende del modelo y elegibilidad | GMB Crush | No se afirma que la dirección sea pública hasta confirmar el modelo y la elegibilidad. Evita afirmaciones incorrectas sobre ubicación. | Depends on business model and eligibility |

## Bloque 3 — Main City y LCA

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 14.08 · Paso-14 §19 Alinear LCA con GBP | Main City para GBP | Input humano | Madrid viene directamente de la dirección aportada por el cliente. | Madrid |
| 14.09 · Paso-14 §19 Alinear LCA con GBP | Direct LCA para GBP | Input humano + Geografía | Almagro y Chamberí salen del NAP/dirección del cliente. Son las zonas de cobertura directa. | Almagro, Chamberí |
| 14.10 · Paso-14 §19 Alinear LCA con GBP | Candidate LCA para GBP | Geografía | Las Candidate LCA son zonas próximas con potencial. No todas están validadas para service areas del GBP. | Salamanca, Retiro, Centro, Tetuán, Chamartín, Arganzuela, Moncloa, Prosperidad |
| 14.11 · Paso-14 §7 Crear GBP después de publicar web base | No hay Approved Expansion Areas iniciales | GMB Crush | No se crean URLs ni se activa expansión sin aprobación explícita. | None in Phase 1 |

## Bloque 4 — Categorías GBP

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 14.12 · Paso-14 §8 Convertir categorías planificadas en confirmadas | Categoría principal prevista | Input humano + GMB Crush | Deriva del nombre del negocio. Debe confirmarse como categoría GBP disponible en el momento de creación. | Cerrajero |
| 14.13 · Paso-14 §8 Convertir categorías planificadas en confirmadas | Primera categoría adicional prevista | IA sin respaldo | Pendiente de confirmar disponibilidad y encaje en GBP. | Servicio de cerrajería de urgencia |
| 14.14 · Paso-14 §8 Convertir categorías planificadas en confirmadas | Segunda categoría adicional prevista | IA sin respaldo | Pendiente de confirmar disponibilidad y encaje en GBP. | Servicio de duplicado de llaves |
| 14.15 · Paso-14 §14 Usar categorías adicionales solo si tienen soporte real | No añadir categoría de seguridad sin soporte web real | GMB Crush | Cada categoría adicional debe tener soporte web real. No se añade "Proveedor de sistemas de seguridad" sin página web que lo respalde. | No añadir Proveedor de sistemas de seguridad |

## Bloque 5 — Servicios del GBP

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 14.16–14.21 · Paso-14 §13 Añadir servicios del GBP alineados con páginas web | Se definen servicios del GBP | IA sin respaldo | Los servicios son plausibles para un cerrajero pero no están confirmados con input del cliente, datos de búsqueda ni análisis de competencia. | Apertura, urgente, cerraduras, bombines, duplicado, seguridad |

## Bloque 6 — URLs conectadas al GBP

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 14.22 · Paso-14 §11 Conectar GBP a URL correcta | URL web conectada al GBP | IA sin respaldo | Dominio de ejemplo pendiente de confirmación por el cliente. | https://www.cerrajerosmadrid24h.com/ |
| 14.23 · Paso-14 §12 Usar UTM sin romper canonical ni NAP | URL de contacto/cita | GMB Crush + IA sin respaldo | El patrón /contacto/ es canónico en GMB Crush. El dominio concreto está pendiente de confirmación. | https://www.cerrajerosmadrid24h.com/contacto/ |

## Bloque 7 — Horarios y recursos visuales

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 14.24 · Paso-14 §18 Definir horarios sin contradicción | Horarios de apertura | IA sin respaldo | Inferido por el nombre "24h". Pendiente de confirmación por el cliente. | 24 horas, todos los días |
| 14.25 · Paso-14 §16 Preparar fotos antes de crear el GBP | Preparar logo | GMB Crush | El logo es el recurso visual de identidad primario. Debe estar listo antes de crear el GBP. | Logo del negocio |
| 14.26 · Paso-14 §16 Preparar fotos antes de crear el GBP | Preparar foto de portada | GMB Crush | La foto de portada es la imagen principal del perfil GBP. Debe transmitir el servicio principal. | Cover photo |
| 14.27 · Paso-14 §16 Preparar fotos antes de crear el GBP | Preparar foto exterior (condicional) | GMB Crush | Solo si hay oficina o punto de atención físico. Para SAB no es prioritaria. | Exterior si procede |
| 14.28 · Paso-14 §16 Preparar fotos antes de crear el GBP | No usar foto de interior para SAB | GMB Crush | Para Service Area Business sin oficina pública, la foto de interior no es relevante ni recomendable. | No aplica para SAB |
| 14.29 · Paso-14 §16 Preparar fotos antes de crear el GBP | Preparar foto del equipo | GMB Crush | Las fotos del equipo generan confianza y humanización del negocio. | Foto del equipo |
| 14.30 · Paso-14 §16 Preparar fotos antes de crear el GBP | Preparar foto del vehículo | GMB Crush | Para SAB, el vehículo es una señal de operación real y presencia local. | Foto del vehículo |
| 14.31 · Paso-14 §16 Preparar fotos antes de crear el GBP | Preparar fotos de trabajos realizados | GMB Crush | Las fotos de trabajos son prueba social visual directa del servicio. | Fotos de trabajos |
| 14.32 · Paso-14 §16 Preparar fotos antes de crear el GBP | No usar fotos de contexto local que finjan oficina | GMB Crush | No se usan fotos de barrios o calles para simular presencia física donde no existe. | Sin fotos de contexto local falso |

## Bloque 8 — Q&A, posts, reseñas y tracking

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 14.33 · Paso-14 §23 Preparar Q&A del GBP | Q&A 1: ¿Cuánto tarda un cerrajero urgente en Madrid? | GMB Crush | Pregunta real de usuario. Respuesta: 20-30 minutos en zonas centrales. Cubre la intención de urgencia. | ¿Cuánto tarda un cerrajero urgente en Madrid? → 20-30 min en zonas centrales |
| 14.34 · Paso-14 §23 Preparar Q&A del GBP | Q&A 2: ¿Tenéis precio fijo o presupuesto previo? | GMB Crush | Pregunta real de usuario sobre precio. Respuesta: presupuesto gratuito antes de actuar. Cubre objeción de coste. | ¿Tenéis precio fijo? → Presupuesto gratuito antes de actuar |
| 14.35 · Paso-14 §23 Preparar Q&A del GBP | Q&A 3: ¿Trabajáis en Chamberí y Almagro? | GMB Crush | Pregunta real de usuario sobre cobertura. Respuesta: sí, y también en Salamanca, Retiro y Centro. Cubre LCA. | ¿Trabajáis en Chamberí y Almagro? → Sí, y también Salamanca, Retiro, Centro |
| 14.36 · Paso-14 §24 Planificar Google Posts conectados con páginas web | Post 1: Servicio de cerrajero urgente | GMB Crush | Post de oferta/servicio conectado a la LBS de cerrajero urgente. Incluye CTA y UTM. | Cerrajero urgente en Madrid — enlace a /cerrajero/madrid/cerrajero-urgente/ |
| 14.37 · Paso-14 §24 Planificar Google Posts conectados con páginas web | Post 2: Duplicado de llaves | GMB Crush | Post de oferta/servicio conectado a la Additional Category Page. Incluye CTA y UTM. | Duplicado de llaves en Madrid — enlace a /cerrajero/madrid/duplicado-llaves/ |
| 14.38 · Paso-14 §24 Planificar Google Posts conectados con páginas web | Post 3: Novedades o contenido local | GMB Crush | Post de actualización conectado al GeoHub o a un GeoArticle. Refuerza señales locales. | Novedades del servicio en Madrid — enlace a /madrid/ |
| 14.39 · Paso-14 §15 No reclamar reseñas antes de tenerlas | Crear estrategia de reseñas reales | GMB Crush | No se inventan reseñas. Se recogen después de cada trabajo. Se pide reseña por WhatsApp o email con enlace directo al GBP. | Review Strategy: pedir tras cada trabajo |
| 14.40 · Paso-14 §12 Usar UTM sin romper canonical ni NAP | Crear UTM para el enlace GBP | GMB Crush | El UTM permite medir el tráfico procedente del GBP en GA4. No rompe el canonical ni el NAP. | https://www.cerrajerosmadrid24h.com/?utm_source=gmb&utm_medium=organic&utm_campaign=gbp-madrid |

## Bloque 9 — Ajustes post-GBP en la web

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 14.41 · Paso-14 §20 Actualizar schema después de crear el GBP | Actualizar schema después de crear GBP | GMB Crush | El sameAs solo se añade cuando existe la URL real del GBP. No se inventa antes. | Añadir sameAs cuando exista GBP URL |
| 14.42 · Paso-14 §21 Actualizar homepage después de verificar perfil | Actualizar Homepage tras crear GBP | GMB Crush | La Homepage se actualiza con la GBP URL, reseñas reales si existen y trust blocks. | Añadir GBP URL, reseñas reales si existen, trust blocks |
| 14.43 · Paso-14 §22 Actualizar página de contacto | Actualizar contacto tras crear GBP | GMB Crush | La página de contacto debe alinear NAP y GBP. Se añade mapa si procede. | Datos confirmados y mapa si procede |
| 14.44 · Paso-14 §28 Revisar LocalBusiness schema tras verificación | Actualizar LBS tras crear GBP | GMB Crush | Las LBS soportan el GBP y el Local Pack. Se ajusta schema, sameAs, reseñas y NAP. | Ajustar schema, sameAs, reseñas y NAP |
| 14.45 · Paso-14 §29 Cola de actualización post-GBP | Actualizar GeoHub tras crear GBP | GMB Crush | El GeoHub agrupa señales de ciudad y GBP. Se alinea cobertura, reviews y enlaces. | Alinear cobertura, reviews y enlaces |

## Bloque 10 — No invención

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 14.46 · Paso-14 §15 No reclamar reseñas antes de tenerlas | No inventar reseñas antes de que existan | GMB Crush | No se usa social proof inexistente. Las reseñas se recogen después de cada trabajo real. | Reseñas iniciales pendientes |
| 14.47 · Paso-14 §20 Actualizar schema después de crear el GBP | No inventar GBP URL antes de crear perfil | GMB Crush | No se añade sameAs ni GBP URL hasta que el perfil exista y esté verificado. | GBP URL N/A hasta creación |
