# Paso 7 — Internal Linking Rules

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

## Bloque 1 — Enlaces desde Homepage

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 7.01 | Homepage enlaza a Service Overview Pages | 5 Service Overview Pages | GMB Crush | Homepage debe enlazar a Service Overviews. | Validada |
| 7.02 | Homepage enlaza al GeoHub de Madrid | /madrid/ | GMB Crush | Homepage debe enlazar al Main GeoHub. | Validada |
| 7.03 | Homepage enlaza a Additional Category Page | /cerrajero/madrid/duplicado-llaves/ | GMB Crush | Additional Category Pages deben estar enlazadas. | Validada |
| 7.04 | Homepage enlaza a contacto | /contacto/ | GMB Crush | Contacto es destino operacional obligatorio. | Validada |

## Bloque 2 — Enlaces desde Service Overview y LBS

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 7.05 | Service Overview enlaza a versión local en Madrid | /cerrajero/[service]/ → /cerrajero/madrid/[service]/ | GMB Crush | Service Overview enlaza a versiones city/service. | Validada |
| 7.06 | Service Overview enlaza a servicios relacionados | Cross-links entre servicios | GMB Crush | Cross-linking refuerza silo semántico. | Validada |
| 7.07 | LBS enlaza a página padre | LBS → Service Overview | GMB Crush | LBS debe enlazar a parent service. | Validada |
| 7.08 | LBS enlaza al GeoHub | LBS → /madrid/ | GMB Crush | LBS debe enlazar al GeoHub. | Validada |
| 7.09 | LBS enlaza a servicios relacionados en Madrid | LBS → otras LBS | GMB Crush | Mismo city silo. | Validada |
| 7.10 | LBS enlaza a GeoArticles relacionados | LBS → GeoArticles | GMB Crush | GeoArticles refuerzan LBS. | Validada |

## Bloque 3 — GeoHub y GeoArticles

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 7.11 | GeoHub enlaza a todas las LBS de Madrid | 5 LBS | GMB Crush | GeoHub agrupa servicios de ciudad. | Validada |
| 7.12 | GeoHub enlaza a Additional Category Page | /cerrajero/madrid/duplicado-llaves/ | GMB Crush | GeoHub agrupa categorías locales. | Validada |
| 7.13 | GeoHub enlaza a GeoArticles | 15 GeoArticles | GMB Crush | GeoHub agrupa artículos ciudad/servicio. | Validada |
| 7.14 | GeoArticles enlazan a LBS correspondiente | GeoArticle → LBS | GMB Crush | Interlink obligatorio. | Validada |
| 7.15 | GeoArticles enlazan al GeoHub | GeoArticle → /madrid/ | GMB Crush | Interlink obligatorio. | Validada |

## Bloque 4 — Restricciones de enlaces

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 7.16 | No enlazar LCA sin URL aprobada | No enlazar /almagro/ | GMB Crush | No se enlaza a URLs inexistentes/no aprobadas. | Validada |
| 7.17 | Usar anchors contextuales | Anchors naturales | GMB Crush | Anchors contextuales evitan exact-match forzado. | Validada |
| 7.18 | Usar breadcrumbs | Home > Madrid > Servicio | GMB Crush | BreadcrumbList y navegación jerárquica. | Validada |

