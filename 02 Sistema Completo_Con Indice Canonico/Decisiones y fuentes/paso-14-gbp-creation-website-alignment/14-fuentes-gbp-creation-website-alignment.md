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

