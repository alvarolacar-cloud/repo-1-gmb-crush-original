# Módulo 15b — Decisiones tomadas y fuentes

Fase 2 de trazabilidad · Capa de Salida al Mercado · Sistema GMB Crush  
Módulo auditado: `15-modulo-redaccion-final-por-url.md`

---

## Objetivo del documento

Este documento lista las decisiones que toma el **Módulo 15 — Redacción final por URL** y asigna una fuente a cada una.

El módulo 15 no cambia la arquitectura SEO. Su función es convertir la arquitectura aprobada en contenido final listo para diseño, construcción y QA.

---

## Fuentes permitidas

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

## Criterio aplicado

```text
GMB Crush = estructura, regla, tipo de página, contenido por Page Type, schema, interlinking o no invención.
Input humano = dato aportado por el usuario o cliente.
IA heredada = valor arrastrado desde una decisión previa ya marcada como no validada.
IA sin respaldo = valor nuevo generado sin fuente real.
GMB Crush + IA sin respaldo = la regla viene de GMB Crush, pero el valor concreto necesita validación.
Decisión de diseño = decisión de presentación del módulo, no de arquitectura SEO.
```

---

# Bloque 1 — Función del módulo

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 15.01 · Módulo-15 §1 Objetivo | Se decide que el módulo transforme la arquitectura aprobada en contenido final por URL | GMB Crush | GMB Crush define que cada tipo de página necesita contenido propio, metadata, FAQs, CTA, schema e internal links. El módulo convierte esa estructura en copy publicable. | Redacción final por URL |
| 15.02 · Módulo-15 §1 Objetivo | Se decide que el módulo no modifique la arquitectura SEO | GMB Crush | La arquitectura ya queda definida en los pasos 1–14. Este módulo solo ejecuta contenido sobre URLs y Page Types aprobados. | No modifica URLs, servicios, categorías ni Page Types |
| 15.03 · Módulo-15 §1 Objetivo | Se decide que el contenido incluya H1, H2, FAQs, CTA, metadata, entidades, LCA y schema notes | GMB Crush | La doctrina GMB Crush exige que las páginas tengan H1, meta, contenido semántico, FAQs, CTA, schema e interlinking según su tipo. | H1, H2, FAQs, CTA, metadata, entidades, LCA y schema notes |
| 15.04 · Módulo-15 §1 Objetivo | Se decide bloquear datos marcados como IA sin respaldo | GMB Crush | El sistema no debe convertir placeholders o claims no confirmados en contenido publicable. La redacción debe respetar decisiones/fuentes. | Datos sin respaldo quedan como pendiente de validación |

---

# Bloque 2 — Momento de ejecución

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 15.05 · Módulo-15 §2 Cuándo se ejecuta | Se decide ejecutar el módulo después de cerrar los pasos 1–14 | GMB Crush | La redacción final depende de URL Matrix, Page Type Rules, Content Architecture, Internal Linking, Schema Map, Priority Score y estado de decisiones/fuentes. | Ejecutar después de pasos 1–14 |
| 15.06 · Módulo-15 §2 Cuándo se ejecuta | Se decide no ejecutar si faltan URL Matrix, Page Type, servicios, Main City, NAP, CTA, links, schema o estado de fuentes | GMB Crush | Sin esos outputs, el contenido podría inventar estructura, páginas o datos no validados. | Bloqueo si falta cualquier fuente interna obligatoria |
| 15.07 · Módulo-15 §2 Cuándo se ejecuta | Se decide que el estado de datos sin respaldo sea una entrada obligatoria | GMB Crush | El módulo de contenido debe saber qué puede afirmar y qué debe bloquear. | Usar Decisiones y fuentes antes de redactar |

---

# Bloque 3 — Inputs del proyecto

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 15.08 · Módulo-15 §3.1 Datos base | Se decide pedir Business Name | Input humano | El cliente proporciona el nombre del negocio. El módulo lo usa para H1, metadata, schema, CTA y copy. | Cerrajeros Madrid 24h |
| 15.09 · Módulo-15 §3.1 Datos base | Se decide pedir Website Root Domain | IA heredada (paso 1.02) | El dominio del ejemplo fue definido en el sistema previo y debe confirmarse antes de producción. | `https://www.cerrajerosmadrid24h.com` |
| 15.10 · Módulo-15 §3.1 Datos base | Se decide pedir Main City | Input humano + GMB Crush | El usuario aporta la ubicación y GMB Crush usa la Main City como base para páginas locales, GeoHub y contenido GEO. | Madrid |
| 15.11 · Módulo-15 §3.1 Datos base | Se decide pedir Primary GBP Category planificada | Input humano + GMB Crush | La categoría planificada alinea contenido, homepage, páginas y futuro GBP. Debe confirmarse antes de crear el perfil real. | Cerrajero |
| 15.12 · Módulo-15 §3.1 Datos base | Se decide pedir NAP final | Input humano + IA sin respaldo | Nombre y dirección vienen del ejemplo; teléfono sigue siendo placeholder hasta confirmación. | Cerrajeros Madrid 24h · Calle Rafael Calvo 12 · Madrid · +34 600 000 000 |
| 15.13 · Módulo-15 §3.1 Datos base | Se decide pedir email | IA heredada (paso 1.15) | El email deriva del dominio del ejemplo y debe confirmarse antes de publicarlo. | `info@cerrajerosmadrid24h.com` |
| 15.14 · Módulo-15 §3.1 Datos base | Se decide pedir teléfono | IA heredada (paso 1.14) | El teléfono es placeholder y no debe publicarse como dato real sin confirmación. | +34 600 000 000 |
| 15.15 · Módulo-15 §3.1 Datos base | Se decide pedir CTA principal | IA heredada (paso 1.42) | El CTA “Llamar ahora” es plausible para cerrajería, pero debe confirmarse como acción principal. | Llamar ahora |
| 15.16 · Módulo-15 §3.1 Datos base | Se decide pedir estado del GBP | Input humano | La situación inicial del sistema indica que el GBP no existe todavía. | Not Created |

---

# Bloque 4 — Fuentes internas obligatorias

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 15.17 · Módulo-15 §3.2 Fuentes internas | Se decide exigir URL Matrix validada | GMB Crush | La URL Matrix es la fuente de verdad de rutas. El contenido no puede inventar URLs. | URL Matrix requerida |
| 15.18 · Módulo-15 §3.2 Fuentes internas | Se decide exigir Page Type Rules | GMB Crush | Cada copy debe respetar su tipo de página: Homepage, Service Overview, LBS, Additional Category, GeoHub o GeoArticle. | Page Type Rules requeridas |
| 15.19 · Módulo-15 §3.2 Fuentes internas | Se decide exigir Content Architecture | GMB Crush | El contenido debe seguir la estructura aprobada de cada página y no improvisar secciones. | Content Architecture requerida |
| 15.20 · Módulo-15 §3.2 Fuentes internas | Se decide exigir Internal Linking Map | GMB Crush | Cada página debe enlazar según la jerarquía aprobada. | Internal Linking Map requerido |
| 15.21 · Módulo-15 §3.2 Fuentes internas | Se decide exigir Schema Map | GMB Crush | El copy debe preparar datos y FAQs compatibles con schema por Page Type. | Schema Map requerido |
| 15.22 · Módulo-15 §3.2 Fuentes internas | Se decide exigir Priority Score | GMB Crush | La producción de contenido debe seguir prioridad y dependencias. | Priority Score requerido |
| 15.23 · Módulo-15 §3.2 Fuentes internas | Se decide exigir Decisiones y fuentes | GMB Crush | La redacción debe saber qué datos están validados y cuáles no pueden publicarse. | Decisiones y fuentes requeridas |

---

# Bloque 5 — Inventario de URLs a redactar

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 15.24 · Módulo-15 §3.3 Inventario | Se decide que cada URL tenga ID, URL, Page Type, servicio, ciudad y estado | GMB Crush | El contenido se produce por URL y Page Type. La tabla evita redactar páginas sin función. | Tabla de inventario por URL |
| 15.25 · Módulo-15 §4.2 URLs ejemplo | Se decide mostrar una muestra representativa de URLs en el ejemplo | Decisión de diseño | El módulo enseña cómo se redactan distintos Page Types sin repetir el inventario completo. No sustituye la URL Matrix. | 6 URLs ejemplo |
| 15.26 · Módulo-15 §4.2 URLs ejemplo | Se incluye Homepage como ejemplo de redacción | GMB Crush | Homepage es Root Entity Anchor y debe tener contenido propio. | `HP-001` · `/` |
| 15.27 · Módulo-15 §4.2 URLs ejemplo | Se incluye Service Overview de cerrajero urgente | GMB Crush + IA heredada (paso 1.34) | La Service Overview viene de GMB Crush; el servicio concreto sigue pendiente de validación. | `/cerrajero/cerrajero-urgente/` |
| 15.28 · Módulo-15 §4.2 URLs ejemplo | Se incluye LBS de cerrajero urgente en Madrid | GMB Crush + IA heredada (paso 1.34) | La LBS `/category/city/service/` es GMB Crush; el servicio concreto sigue pendiente de validación. | `/cerrajero/madrid/cerrajero-urgente/` |
| 15.29 · Módulo-15 §4.2 URLs ejemplo | Se incluye Additional Category Page de duplicado de llaves | GMB Crush + IA heredada (paso 1.40) | GMB Crush exige soporte web a categorías adicionales; la categoría concreta queda pendiente de validación. | `/cerrajero/madrid/duplicado-llaves/` |
| 15.30 · Módulo-15 §4.2 URLs ejemplo | Se incluye GeoHub de Madrid | Input humano + GMB Crush | Madrid viene del input y GMB Crush define el GeoHub como contenedor de ciudad. | `/madrid/` |
| 15.31 · Módulo-15 §4.2 URLs ejemplo | Se incluye GeoArticle de coste de cerrajero urgente | GMB Crush + IA heredada (paso 3.19) | GMB Crush define GeoArticles; el topic concreto requiere keyword research. | `/madrid/cuanto-cuesta-un-cerrajero-urgente/` |

---

# Bloque 6 — Datos que no se pueden inventar

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 15.32 · Módulo-15 §3.4 Datos no inventables | Se decide bloquear años de experiencia si no están confirmados | GMB Crush | Trust signals solo se publican si están respaldados. | 10+ años queda pendiente |
| 15.33 · Módulo-15 §3.4 Datos no inventables | Se decide bloquear reseñas si no existe GBP o no hay reseñas reales | GMB Crush | No se inventan reseñas, estrellas ni social proof de Google. | Reseñas bloqueadas hasta crear GBP |
| 15.34 · Módulo-15 §3.4 Datos no inventables | Se decide bloquear precios si no hay datos reales | GMB Crush + IA sin respaldo | La estructura puede pedir rangos, pero el precio concreto requiere input, mercado o datos. | Precios pendientes |
| 15.35 · Módulo-15 §3.4 Datos no inventables | Se decide bloquear horarios si no están confirmados | IA heredada (paso 14.24) | El horario 24h se infiere por el nombre, pero debe confirmarse. | Horarios pendientes |
| 15.36 · Módulo-15 §3.4 Datos no inventables | Se decide bloquear garantías si no están confirmadas | IA heredada (paso 1.47) | “Garantía de trabajo” no puede publicarse como claim real sin confirmación. | Garantía pendiente |
| 15.37 · Módulo-15 §3.4 Datos no inventables | Se decide bloquear certificaciones si no están confirmadas | GMB Crush | Credenciales y certificaciones solo se publican con prueba real. | Certificaciones bloqueadas |
| 15.38 · Módulo-15 §3.4 Datos no inventables | Se decide bloquear fotos o casos reales si no existen | GMB Crush | No se inventan casos, fotos, oficinas, equipo ni pruebas visuales. | Fotos/casos pendientes |

---

# Bloque 7 — Reglas operativas de redacción

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 15.39 · Módulo-15 §5 Regla 1 | Se decide redactar por URL, no por servicio genérico | GMB Crush | Cada Page Type tiene función, intención y estructura propia. | Una URL = una función = un copy único |
| 15.40 · Módulo-15 §5 Regla 1 | Se decide evitar duplicar texto entre Service Overview y LBS | GMB Crush | Service Overview y Location-Based Service no son intercambiables. | No duplicar `/cerrajero/cerrajero-urgente/` y `/cerrajero/madrid/cerrajero-urgente/` |
| 15.41 · Módulo-15 §5 Regla 2 | Se decide que Homepage actúe como Root Entity Anchor | GMB Crush | La homepage establece quién es la marca, qué hace, dónde opera, NAP, servicios, confianza y enlaces internos. | Homepage con marca + servicio + Madrid |
| 15.42 · Módulo-15 §5 Regla 3 | Se decide que Service Overview no tenga ciudad como target principal | GMB Crush | Service Overview es topical authority pillar sin ubicación. | `/cerrajero/cerrajero-urgente/` sin target principal Madrid |
| 15.43 · Módulo-15 §5 Regla 4 | Se decide que LBS sea página de conversión servicio + ciudad | GMB Crush | La LBS rankea y convierte búsquedas de servicio en ciudad. | `/cerrajero/madrid/cerrajero-urgente/` |
| 15.44 · Módulo-15 §5 Regla 4 | Se decide permitir menciones de LCA sin crear URLs | GMB Crush | Las Local Coverage Areas refuerzan contexto GEO, pero no generan páginas por defecto. | Almagro y Chamberí como contexto |
| 15.45 · Módulo-15 §5 Regla 5 | Se decide que Additional Category Page soporte una categoría adicional | GMB Crush | Cada categoría adicional efectiva necesita soporte web específico. | Duplicado de llaves en Madrid |
| 15.46 · Módulo-15 §5 Regla 6 | Se decide que GeoHub sea contenedor de ciudad | GMB Crush | El GeoHub organiza servicios, categorías, artículos y cobertura local. | `/madrid/` |
| 15.47 · Módulo-15 §5 Regla 7 | Se decide que GeoArticles sean boosters semánticos, no landings | GMB Crush | GeoArticles responden intención long-tail y refuerzan LBS/GeoHub. | `/madrid/cuanto-cuesta-un-cerrajero-urgente/` |
| 15.48 · Módulo-15 §5 Regla 8 | Se decide no publicar datos sin respaldo | GMB Crush | El contenido final no convierte placeholders en claims reales. | No publicar “250+ reseñas” ni “10+ años” sin prueba |
| 15.49 · Módulo-15 §5 Regla 9 | Se decide que cada URL entregue Content Pack completo | GMB Crush | Para construir la web, cada URL necesita H1, metadata, H2s, copy, FAQs, CTA, links y schema notes. | Output final por URL |

---

# Bloque 8 — Checklist y outputs

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 15.50 · Módulo-15 §6 Checklist | Se decide validar que todas las URLs tengan copy asignado | GMB Crush | La redacción final debe cubrir todo el inventario aprobado, no solo ejemplos. | Check URL Matrix |
| 15.51 · Módulo-15 §6 Checklist | Se decide validar que cada copy respete su Page Type | GMB Crush | La estructura de contenido depende del tipo de página. | Check Page Type |
| 15.52 · Módulo-15 §6 Checklist | Se decide validar que LBS usen ciudad y LCA sin falsas ubicaciones | GMB Crush | Las páginas locales deben usar contexto GEO sin fingir oficinas. | Check Local |
| 15.53 · Módulo-15 §6 Checklist | Se decide validar que GeoArticles enlacen a LBS y GeoHub | GMB Crush | GeoArticles son boosters conectados al cluster, no contenido aislado. | Check GeoArticles |
| 15.54 · Módulo-15 §6 Checklist | Se decide validar que no haya reseñas, años o garantías inventadas | GMB Crush | La capa de decisiones/fuentes bloquea claims no confirmados. | Check Trust |
| 15.55 · Módulo-15 §7 Outputs | Se decide entregar Content Pack por URL | GMB Crush | El constructor necesita contenido final por URL como fuente de verdad. | Content Pack por URL |
| 15.56 · Módulo-15 §7 Outputs | Se decide entregar Metadata Matrix | GMB Crush | Cada URL necesita meta title y description propios. | Metadata Matrix |
| 15.57 · Módulo-15 §7 Outputs | Se decide entregar FAQ Matrix | GMB Crush | FAQs alimentan contenido, schema y AI Overview. | FAQ Matrix |
| 15.58 · Módulo-15 §7 Outputs | Se decide entregar CTA Matrix | GMB Crush | Cada Page Type requiere CTA adaptado. | CTA Matrix |
| 15.59 · Módulo-15 §7 Outputs | Se decide entregar Internal Link Copy Matrix | GMB Crush | Los anchors y enlaces deben coincidir con el mapa de interlinking. | Internal Link Copy Matrix |
| 15.60 · Módulo-15 §7 Outputs | Se decide entregar Schema Content Notes | GMB Crush | El constructor necesita saber qué datos alimentan schema. | Schema Content Notes |
| 15.61 · Módulo-15 §7 Outputs | Se decide entregar datos bloqueados o pendientes | GMB Crush | El módulo debe impedir que datos no validados pasen a producción. | Datos bloqueados / pendientes |

---

# Lectura final

El Módulo 15 está alineado con el ejemplo **Cerrajeros Madrid 24h** en:

```text
Business Name
dominio de ejemplo
Main City = Madrid
GBP Status = Not Created
/contacto/
Page Types GMB Crush
Duplicado de llaves como Additional Category Page
GeoHub /madrid/
GeoArticle /madrid/cuanto-cuesta-un-cerrajero-urgente/
bloqueo de reseñas y datos no confirmados
```

Pero el inventario de ejemplo del Módulo 15 muestra solo una **muestra representativa** de URLs, no las 28 URLs SEO base completas. Eso no es un fallo si se entiende como ejemplo. Para ejecución real, el Content Pack debe cubrir todas las URLs aprobadas por la URL Matrix.
