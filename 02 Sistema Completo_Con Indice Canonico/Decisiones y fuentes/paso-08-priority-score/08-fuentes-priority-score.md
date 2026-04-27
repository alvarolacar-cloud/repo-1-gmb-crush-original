# Paso 8 — Priority Score

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

## Bloque 1 — Fórmula de prioridad

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 8.01 | Se decide usar fórmula de seis factores | Revenue + Intent + GBP Relevance + Local Relevance + Gap + Urgency | GMB Crush | Prioriza por valor, intención y relevancia local. | Validada |
| 8.02 | Se decide no usar City Priority en la base | Se usa Local Relevance | GMB Crush | La base tiene una Main City; no hay comparación multi-ciudad. | Validada |

## Bloque 2 — Ejemplo canónico

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 8.03 | Se decide evaluar LBS de Cerrajero urgente | /cerrajero/madrid/cerrajero-urgente/ | GMB Crush + IA sin respaldo | LBS canónica estructural; servicio concreto pendiente. | Parcialmente validada |
| 8.04 | Se asigna Revenue Value | 5 | IA sin respaldo | No hay datos económicos o de conversión. | IA sin respaldo |
| 8.05 | Se asigna Search Intent | 5 | IA sin respaldo | No hay keyword research documentado. | IA sin respaldo |
| 8.06 | Se asigna GBP Category Relevance | 5 | GMB Crush + IA sin respaldo | Parece alineado con cerrajero, pero categoría/servicio no confirmados. | Parcialmente validada |
| 8.07 | Se asigna Local Relevance | 5 | Input humano + GMB Crush | Madrid es Main City; LBS de Madrid es estructuralmente relevante. | Validada |
| 8.08 | Se asigna Competition Gap | 4 | IA sin respaldo | No hay análisis competitivo documentado. | IA sin respaldo |
| 8.09 | Se asigna Conversion Urgency | 5 | IA sin respaldo | Plausible para urgencias, pero no validado con datos. | Pendiente de validación |
| 8.10 | Se calcula el score total | 29 | IA sin respaldo | Suma de factores no validados. | Pendiente de validación |
| 8.11 | Se asigna prioridad | P1 | IA sin respaldo | Deriva del score pendiente de validación. | Pendiente de validación |

## Bloque 3 — Inventario completo

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 8.12 | Se decide asignar Priority Score a las 28 URLs SEO base | 28 URLs | GMB Crush | Cada URL debe tener prioridad para producción. | Validada |
| 8.13 | Se decide que /contacto/ tenga prioridad operativa, no SEO | Página auxiliar | GMB Crush | Contacto no forma parte del inventario SEO base. | Validada |
| 8.14 | Se decide que GeoArticles se prioricen después de páginas padre | GeoArticle después de LBS | GMB Crush | GeoArticles apoyan LBS/GeoHub, no sustituyen páginas padre. | Validada |

