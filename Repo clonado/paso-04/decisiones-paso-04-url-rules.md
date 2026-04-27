# Auditoría de trazabilidad — Paso 4: URL Rules

Documento auditado: `04-url-rules.md`
Sección: "Ejemplo rellenado" + "Estructura final aprobada para Cerrajeros Madrid 24h" + "URLs no aprobadas en la fase base"
Negocio: Cerrajeros Madrid 24h

---

## A. Política de URL (3 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 4.01 | Política de trailing slash | Yes |
| 4.02 | Política sobre "near me" en URL | No |
| 4.03 | Política sobre "best/cheap/top-rated" en URL | No |

---

## B. Patrones URL por tipo de página (5 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 4.04 | Patrón de URL para Service Overview | `/cerrajero/[service-slug]/` |
| 4.05 | Patrón de URL para Main City GeoHub | `/madrid/` (Option A) |
| 4.06 | Patrón de URL para Location-Based Service | `/cerrajero/madrid/[service-slug]/` |
| 4.07 | Patrón de URL para Additional Category | `/cerrajero/madrid/[additional-category-slug]/` |
| 4.08 | Patrón de URL para GeoArticle | `/madrid/[article-topic-slug]/` (Option A) |

---

## C. URLs aprobadas (13 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 4.09 | URL Homepage | `/` |
| 4.10 | URL Service Overview 1 | `/cerrajero/cerrajero-urgente/` |
| 4.11 | URL Service Overview 2 | `/cerrajero/apertura-puertas/` |
| 4.12 | URL Service Overview 3 | `/cerrajero/cambio-cerraduras/` |
| 4.13 | URL Service Overview 4 | `/cerrajero/cambio-bombines/` |
| 4.14 | URL Service Overview 5 | `/cerrajero/instalacion-cerraduras-seguridad/` |
| 4.15 | URL Main City GeoHub | `/madrid/` |
| 4.16 | URL LBS 1 | `/cerrajero/madrid/cerrajero-urgente/` |
| 4.17 | URL LBS 2 | `/cerrajero/madrid/apertura-puertas/` |
| 4.18 | URL LBS 3 | `/cerrajero/madrid/cambio-cerraduras/` |
| 4.19 | URL LBS 4 | `/cerrajero/madrid/cambio-bombines/` |
| 4.20 | URL LBS 5 | `/cerrajero/madrid/instalacion-cerraduras-seguridad/` |
| 4.21 | URL Additional Category | `/cerrajero/madrid/duplicado-llaves/` |

---

## D. Topics y URLs de GeoArticle (6 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 4.22 | Topic GeoArticle 1 | `guia-precios-cerrajero-urgente` |
| 4.23 | URL GeoArticle 1 | `/madrid/guia-precios-cerrajero-urgente/` |
| 4.24 | Topic GeoArticle 2 | `que-hacer-si-no-puedes-entrar-casa` |
| 4.25 | URL GeoArticle 2 | `/madrid/que-hacer-si-no-puedes-entrar-casa/` |
| 4.26 | Topic GeoArticle 3 | `cuanto-tarda-un-cerrajero` |
| 4.27 | URL GeoArticle 3 | `/madrid/cuanto-tarda-un-cerrajero/` |

---

## E. URLs no aprobadas en fase base (1 decisión)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 4.28 | Lista de URLs explícitamente no aprobadas | `/almagro/`, `/cerrajero/almagro/cerrajero-urgente/`, `/chamberi/`, `/cerrajero/salamanca/apertura-puertas/`, `/retiro/guia-precios-cerrajero-urgente/` |

---

**Total decisiones detectadas en el paso 4: 28**

**Distribución por bloque:**
- A. Política de URL: 3
- B. Patrones URL por tipo: 5
- C. URLs aprobadas: 13
- D. Topics y URLs de GeoArticle: 6
- E. URLs no aprobadas: 1
