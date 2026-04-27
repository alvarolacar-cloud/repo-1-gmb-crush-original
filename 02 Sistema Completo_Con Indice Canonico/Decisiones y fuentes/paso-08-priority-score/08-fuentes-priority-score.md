# Paso 8 — Priority Score

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

## Bloque 1 — Fórmula de prioridad

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 8.01 · Paso-08 §7 Regla 1 Fórmula de prioridad | Se decide usar fórmula de seis factores | GMB Crush | GMB Crush define la fórmula de prioridad con seis factores: Revenue, Intent, GBP Relevance, Local Relevance, Gap y Urgency. Cada uno se puntúa de 1 a 5. | Revenue + Intent + GBP Relevance + Local Relevance + Gap + Urgency |
| 8.02 · Paso-08 §22 Local Relevance | Se decide no usar City Priority en la base | GMB Crush | En la fase base solo hay una Main City. City Priority se activa cuando hay múltiples ciudades en la expansión. | Se usa Local Relevance |

## Bloque 2 — Ejemplo canónico

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 8.03 · Paso-08 §17 Tabla de prioridad | Se decide evaluar LBS de Cerrajero urgente | GMB Crush + IA sin respaldo | La LBS de cerrajero urgente es la página canónica estructural del ejemplo. El servicio concreto está pendiente de validación. | /cerrajero/madrid/cerrajero-urgente/ |
| 8.04 · Paso-08 §19 Revenue Value | Se asigna Revenue Value | IA sin respaldo | No hay datos económicos ni de conversión documentados. El valor 5 es una estimación sin respaldo real. | 5 |
| 8.05 · Paso-08 §20 Search Intent | Se asigna Search Intent | IA sin respaldo | No hay keyword research documentado. El valor 5 es una estimación sin respaldo real. | 5 |
| 8.06 · Paso-08 §21 GBP Category Relevance | Se asigna GBP Category Relevance | GMB Crush + IA sin respaldo | La regla de alineación GBP es GMB Crush. La categoría y servicio concretos no están confirmados. | 5 |
| 8.07 · Paso-08 §22 Local Relevance | Se asigna Local Relevance | Input humano + GMB Crush | Madrid es la Main City aportada por el cliente. GMB Crush establece que la LBS de Main City tiene relevancia local máxima. | 5 |
| 8.08 · Paso-08 §23 Competition Gap | Se asigna Competition Gap | IA sin respaldo | No hay análisis competitivo documentado. El valor 4 es una estimación sin respaldo real. | 4 |
| 8.09 · Paso-08 §24 Conversion Urgency | Se asigna Conversion Urgency | IA sin respaldo | Plausible para servicios de urgencia, pero no validado con datos de comportamiento o conversión. | 5 |
| 8.10 · Paso-08 §17 Tabla de prioridad | Se calcula el score total | IA sin respaldo | Suma directa de los seis factores. El resultado depende de factores no validados. | 29 |
| 8.11 · Paso-08 §14 Regla 8 Priority Tiers | Se asigna prioridad | IA sin respaldo | La prioridad P1 deriva del score calculado. Queda pendiente de validación cuando los factores se confirmen. | P1 |

## Bloque 3 — Inventario completo

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 8.12 · Paso-08 §17 Tabla de prioridad | Se decide asignar Priority Score a las 28 URLs SEO base | GMB Crush | Cada URL del inventario debe tener prioridad asignada antes de producción. Ver matriz completa de scores en `08a-ejecucion-priority-score.md §17`. | 28 URLs |
| 8.13 · Paso-08 §26 LCA sin score propio | Se decide que /contacto/ tenga prioridad operativa, no SEO | GMB Crush | Contacto es página operativa. No forma parte del inventario SEO base y no recibe Priority Score. | Página auxiliar |
| 8.14 · Paso-08 §15 Regla 9 Páginas comerciales antes que semánticas | Se decide que GeoArticles se prioricen después de páginas padre | GMB Crush | Los GeoArticles apoyan LBS y GeoHub. No sustituyen páginas padre. Se producen en fases posteriores. | GeoArticle después de LBS |
