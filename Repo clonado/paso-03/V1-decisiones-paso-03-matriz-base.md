# Auditoría de trazabilidad — Paso 3: Matriz Base

Documento auditado: `03-matriz-base.md`
Sección: "Ejemplo rellenado" + "Ejemplo de URL Matrix base" + "Filas que NO se generan en la base"
Negocio: Cerrajeros Madrid 24h

---

## A. Configuración de la matriz e IDs (9 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 3.01 | Se define el nombre de la spreadsheet | Cerrajeros Madrid 24h – GMB Crush Website Architecture |
| 3.02 | Se elige el Default Page Status | Planned |
| 3.03 | Se elige la Default Priority | P3 |
| 3.04 | Se asigna ID a la Homepage | HP-001 |
| 3.05 | Se asigna ID al Service Overview ejemplo | SO-001 |
| 3.06 | Se asigna ID al Main City GeoHub | GH-001 |
| 3.07 | Se asigna ID al Location-Based Service ejemplo | LBS-001 |
| 3.08 | Se asigna ID a la Additional Category | AC-001 |
| 3.09 | Se asigna ID al GeoArticle ejemplo | GA-001 |

---

## B. URLs asignadas (7 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 3.10 | Se elige el GeoHub URL Style | Option A: `/city/` |
| 3.11 | URL Homepage | `/` |
| 3.12 | URL Service Overview ejemplo | `/cerrajero/cerrajero-urgente/` |
| 3.13 | URL Main City GeoHub | `/madrid/` |
| 3.14 | URL Location-Based Service ejemplo | `/cerrajero/madrid/cerrajero-urgente/` |
| 3.15 | URL Additional Category | `/cerrajero/madrid/duplicado-llaves/` |
| 3.16 | URL GeoArticle ejemplo | `/madrid/guia-precios-cerrajero-urgente/` |

---

## C. H1s asignados (6 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 3.17 | H1 Homepage | Cerrajeros Madrid 24h – Servicios de cerrajería de confianza en Madrid |
| 3.18 | H1 Service Overview ejemplo | Servicios profesionales de cerrajería urgente por Cerrajeros Madrid 24h |
| 3.19 | H1 Main City GeoHub | Cerrajeros Madrid 24h – Servicios de cerrajería en Madrid |
| 3.20 | H1 Location-Based Service ejemplo | Cerrajeros Madrid 24h – Cerrajero urgente en Madrid |
| 3.21 | H1 Additional Category | Cerrajeros Madrid 24h – Duplicado de llaves experto en Madrid |
| 3.22 | H1 GeoArticle ejemplo | How Much Does an Precio de cerrajero urgente en Madrid? |

---

## D. Schemas asignados (6 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 3.23 | Schema Homepage | Organization, WebSite, LocalBusiness |
| 3.24 | Schema Service Overview ejemplo | Service, WebPage, BreadcrumbList |
| 3.25 | Schema Main City GeoHub | CollectionPage, BreadcrumbList |
| 3.26 | Schema Location-Based Service ejemplo | LocalBusiness, BreadcrumbList |
| 3.27 | Schema Additional Category | Service, BreadcrumbList |
| 3.28 | Schema GeoArticle ejemplo | Article, FAQPage, BreadcrumbList |

---

## E. Prioridades asignadas (6 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 3.29 | Prioridad Homepage | P1 |
| 3.30 | Prioridad Service Overview ejemplo | P1 |
| 3.31 | Prioridad Main City GeoHub | P1 |
| 3.32 | Prioridad Location-Based Service ejemplo | P1 |
| 3.33 | Prioridad Additional Category | P3 |
| 3.34 | Prioridad GeoArticle ejemplo | P3 |

---

## F. Fases asignadas (6 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 3.35 | Fase Homepage | Phase 1 |
| 3.36 | Fase Service Overview ejemplo | Phase 1 |
| 3.37 | Fase Main City GeoHub | Phase 1 |
| 3.38 | Fase Location-Based Service ejemplo | Phase 2 |
| 3.39 | Fase Additional Category | Phase 2 |
| 3.40 | Fase GeoArticle ejemplo | Phase 3 |

---

## G. URLs no generadas en fase base (1 decisión)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 3.41 | Lista de URLs explícitamente NO generadas | `/almagro/`, `/cerrajero/almagro/cerrajero-urgente/`, `/chamberi/`, `/cerrajero/salamanca/apertura-puertas/`, `/retiro/guia-precios-cerrajero-urgente/` |

---

**Total decisiones detectadas en el paso 3: 41**

**Distribución por bloque:**
- A. Configuración de la matriz e IDs: 9
- B. URLs asignadas: 7
- C. H1s asignados: 6
- D. Schemas asignados: 6
- E. Prioridades asignadas: 6
- F. Fases asignadas: 6
- G. URLs no generadas: 1
