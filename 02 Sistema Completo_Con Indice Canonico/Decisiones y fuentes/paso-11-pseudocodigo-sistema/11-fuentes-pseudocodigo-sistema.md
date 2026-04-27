# Paso 11 — Pseudocódigo del Sistema

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

## Bloque 1 — Inputs, slugs y categorías

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 11.01 | Se decide cargar inputs base | Business name, URL, NAP, Main City, servicios, LCA, GBP status | GMB Crush | El sistema necesita inputs antes de generar arquitectura. | Validada |
| 11.02 | Se decide normalizar slugs | Cerrajero urgente → cerrajero-urgente | GMB Crush | URLs limpias requieren normalización. | Validada |
| 11.03 | Se decide validar categorías adicionales | Cubierta / necesita página | GMB Crush | Evita duplicados y asegura soporte a categorías. | Validada |

## Bloque 2 — Generación base

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 11.04 | Se decide generar Homepage | HP-001 | GMB Crush | Root Entity Anchor. | Validada |
| 11.05 | Se decide generar Service Overview Pages | 5 páginas | GMB Crush + IA sin respaldo | Patrón válido; lista de servicios pendiente. | Parcialmente validada |
| 11.06 | Se decide generar GeoHub de Madrid | /madrid/ | GMB Crush + Input humano | GeoHub de Main City. | Validada |
| 11.07 | Se decide generar LBS de Madrid | 5 páginas | GMB Crush + IA sin respaldo | Patrón válido; servicios pendientes. | Parcialmente validada |
| 11.08 | Se decide generar Additional Category Page efectiva | /cerrajero/madrid/duplicado-llaves/ | GMB Crush + IA sin respaldo | Tipo válido; categoría pendiente. | Parcialmente validada |
| 11.09 | Se decide generar GeoArticles | 15 artículos | GMB Crush + IA sin respaldo | Cantidad válida; temas pendientes de datos. | Parcialmente validada |

## Bloque 3 — LCA y expansión

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 11.10 | Se decide inyectar LCA en contenido y schema | LCA como señales GEO | GMB Crush + Geografía | LCA directas validadas; candidatas pendientes de test GEO. | Parcialmente validada |
| 11.11 | Se decide no generar expansión si no está aprobada | Approved Expansion Areas: None | GMB Crush | No crear URLs fuera de Main City sin aprobación. | Validada |

## Bloque 4 — Enlaces, prioridad, QA y outputs

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 11.12 | Se decide asignar enlaces internos por tipo | Internal Linking Map | GMB Crush | Jerarquía de enlaces del framework. | Validada |
| 11.13 | Se decide calcular prioridad por página | Priority Score | GMB Crush | Orden de producción requiere scoring. | Validada |
| 11.14 | Se decide comprobar dependencias | LBS requiere Service Overview + GeoHub | GMB Crush | Evita páginas huérfanas o sin padre. | Validada |
| 11.15 | Se decide ejecutar QA antes de publicar | QA Matrix | GMB Crush | No publicar sin QA. | Validada |
| 11.16 | Se decide producir matrices finales | URL Matrix, Internal Linking Matrix, Schema Map, Priority Score, Publishing Plan, QA Matrix | GMB Crush | El output operativo son matrices, no contenido suelto. | Validada |

