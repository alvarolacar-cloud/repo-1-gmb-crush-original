# Paso 19 — Acciones Futuro y Escalado

Fase 2 de trazabilidad del sistema GMB Crush.

Fuentes permitidas:

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

## Bloque 1 — Vigilancia post-launch

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 19.01 · Paso-19 §7.1 Vigilancia | Se decide medir el flujo GeoArticle → Location | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Métrica obligatoria post-launch. | GA4: eventos de click en puentes narrativos (Paso 15 §14.5); páginas/sesión cuando entrada es GeoArticle |
| 19.02 · Paso-19 §7.2 Vigilancia | Se decide medir la autoridad del GeoHub | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Métrica obligatoria post-launch. | GSC: impresiones y posiciones de /madrid/ para queries informativas amplias |
| 19.03 · Paso-19 §7.3 Vigilancia | Se decide medir la conversión del Servicio Core en su LBS | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Métrica obligatoria post-launch. | GA4: tasa de envío de formulario y clicks `tel:` en /cerrajero/madrid/cerrajero-urgente/ |

## Bloque 2 — Criterios de escalado a páginas de barrio

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 19.04 · Paso-19 §8.3 Orden | Se decide el orden de construcción (SO → LBS → GeoArticles → Páginas de Barrio) | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Las páginas de barrio se construyen al final, no al principio. | Cluster base completo antes de evaluar barrios |
| 19.05 · Paso-19 §9.4 Regla 2-de-3 | Se decide aplicar la regla "2 de 3 triggers cumplidos" para autorizar páginas de barrio | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Sin 2 de 3, no se escala. | Ejemplo Almagro: pendiente — esperar baseline 4–8 semanas |
| 19.06 · Paso-19 §9.1 Trigger 1 | Se decide validar Trigger 1 (Location ya responde) con métricas concretas | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Indicadores: impresiones >100/mes, clicks >10/mes, posición <30 para alguna keyword. | LBS Cerrajero urgente Madrid: pendiente medir |
| 19.07 · Paso-19 §9.2 Trigger 2 | Se decide validar Trigger 2 (GeoArticles traen tráfico) con métricas concretas | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Indicadores: 1+ GeoArticle con >50 impresiones/mes y >5 clicks/mes. | GeoArticles del cluster Cerrajero urgente: pendiente medir |
| 19.08 · Paso-19 §9.3 Trigger 3 | Se decide validar Trigger 3 (SERP cambia con barrio) con análisis del §10 | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Indicador: SERP segmentada con 3+ páginas específicas del barrio. | Análisis SERP por barrio pendiente de ejecutar |

## Bloque 3 — Análisis SERP por barrio

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 19.09 · Paso-19 §10.1 Input | Se decide documentar input del análisis: servicio + ciudad + barrio | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Sin input concreto, no hay análisis. | Servicio: Cerrajero urgente; Ciudad: Madrid; Barrio: [a definir por candidato] |
| 19.10 · Paso-19 §10.2 Doble búsqueda | Se decide ejecutar doble búsqueda en Google ("servicio ciudad" vs "servicio barrio") | GMB Crush | El framework define esta regla metodológica. Se aplica igual en todos los proyectos. La ejecución en producción usa Datos de búsqueda (queries reales) y Competidores (análisis de SERP). | Búsquedas reales en Google con resultados orgánicos comparados |
| 19.11 · Paso-19 §10.2 Comparación | Se decide responder las 4 preguntas de comparación SERP | GMB Crush | El framework define esta regla metodológica. Se aplica igual en todos los proyectos. La ejecución en producción usa Competidores (análisis de SERPs reales). | Las 4 preguntas: similitud, páginas específicas, URLs orientadas al barrio, intención mantenida |
| 19.12 · Paso-19 §10.2 Clasificación | Se decide clasificar el resultado en Escenario A (sin segmentación) o B (con segmentación) | GMB Crush | El framework define esta regla metodológica. Se aplica igual en todos los proyectos. La clasificación se ejecuta sobre el análisis del Trigger 3 (Competidores en producción real). | Pendiente de ejecutar para cada candidato |
| 19.13 · Paso-19 §10.3 Output | Se decide documentar output con decisión CREAR / NO CREAR + justificación + nivel de confianza | GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. Sin output documentado, la decisión queda sin trazabilidad. | Output completo con decisión, justificación 3–5 líneas, confianza Alta/Media/Baja |
