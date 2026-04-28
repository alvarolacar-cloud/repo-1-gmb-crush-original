# Paso 8 — Priority Score

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

## Bloque 1 — Fórmula de prioridad

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 8.01 · Paso-08 §7 Fórmula | Se decide usar una fórmula de seis factores | GMB Crush | Doctrina GMB Crush | El framework define la fórmula canónica de 6 factores. | Revenue + Intent + GBP Relevance + Local Relevance + Gap + Urgency |
| 8.02 · Paso-08 §11 Local Relevance | Se decide no usar City Priority en la base | GMB Crush | Doctrina GMB Crush | El framework dicta sustituir City Priority por Local Relevance en la base con una sola Main City. | Se usa Local Relevance |

## Bloque 2 — Ejemplo canónico

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 8.03 · Paso-08 §17 Tabla ejemplo | Se decide evaluar como ejemplo la LBS de Cerrajero urgente | GMB Crush | Heredado del paso 1.34 | El framework dicta usar el servicio core como ejemplo canónico. Servicio heredado del paso 1.34. | /cerrajero/madrid/cerrajero-urgente/ |
| 8.04 · Paso-08 §8 Revenue Value | Se asigna Revenue Value | GMB Crush | Input humano | El framework define el factor Revenue. El valor concreto requiere ticket medio + márgenes del cliente; pendiente de validar en producción real. | 5 |
| 8.05 · Paso-08 §9 Search Intent | Se asigna Search Intent | GMB Crush | Datos de búsqueda | El framework define el factor Search Intent. El valor concreto requiere keyword research (volumen + intent type); pendiente de validar. | 5 |
| 8.06 · Paso-08 §10 GBP Category Relevance | Se asigna GBP Category Relevance | GMB Crush | Competidores | El framework define el factor GBP Category Relevance. El valor concreto requiere matching con catálogo oficial GBP y análisis de qué categorías usan los rivales del Local Pack; pendiente de validar. | 5 |
| 8.07 · Paso-08 §11 Local Relevance | Se asigna Local Relevance | GMB Crush | Heredado del paso 1.20 | El framework define el factor Local Relevance. La LBS Madrid es estructuralmente relevante porque Madrid es la Main City heredada del paso 1.20. | 5 |
| 8.08 · Paso-08 §12 Competition Gap | Se asigna Competition Gap | GMB Crush | Competidores | El framework define el factor Competition Gap. El valor concreto requiere SERP analysis y gap competitivo; pendiente de validar. | 4 |
| 8.09 · Paso-08 §13 Conversion Urgency | Se asigna Conversion Urgency | GMB Crush | Decisión de diseño | El framework define el factor Conversion Urgency. El valor concreto se justifica por la naturaleza urgente del servicio — decisión del operador en función del posicionamiento del negocio. | 5 |
| 8.10 · Paso-08 §17 Tabla ejemplo | Se calcula el score total | GMB Crush | Heredado del paso 8.04–8.09 | El framework define el cálculo como suma de factores. El valor concreto deriva de los factores anteriores; pendiente de validación. | 29 |
| 8.11 · Paso-08 §17 Tabla ejemplo | Se asigna prioridad | GMB Crush | Heredado del paso 8.10 | El framework define la tabla de tiers (P1 ≥ 26). La prioridad deriva del score; pendiente de validación. | P1 |

## Bloque 3 — Inventario completo

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Origen del dato | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|---|
| 8.12 · Paso-08 §31.1 Inventario completo | Se decide asignar Priority Score a las 28 URLs SEO base | GMB Crush | Doctrina GMB Crush | El framework dicta asignar Priority Score a cada URL del inventario. | 28 URLs |
| 8.13 · Paso-08 §31.1 Inventario completo | Se decide que `/contacto/` tenga prioridad operativa, no SEO | GMB Crush | Doctrina GMB Crush | El framework define `/contacto/` como página auxiliar. | Página auxiliar |
| 8.14 · Paso-08 §18 Orden | Se decide que GeoArticles se prioricen después de sus páginas padre | GMB Crush | Doctrina GMB Crush | El framework define la regla de dependencias: GeoArticle siempre después de su LBS. | GeoArticle después de LBS |
| 8.15 · Paso-08 §31.1 Inventario completo | Se decide que la matriz completa de scores de las 28 URLs está documentada en el paso del sistema | GMB Crush | Doctrina GMB Crush | El framework define que la tabla canónica vive en `08-priority-score.md`. | Ver tabla completa con score y prioridad por URL |
