# Auditoría de trazabilidad — Paso 2: Fórmula Maestra de Arquitectura

Documento auditado: `02-formula-maestra-arquitectura.md`
Sección: "Ejemplo rellenado" + "Tabla de inventario base"
Negocio: Cerrajeros Madrid 24h

---

## A. Slugs (8 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 2.01 | Se define el slug de la categoría principal | `cerrajero` |
| 2.02 | Se define el slug de la Main City | `madrid` |
| 2.03 | Se define el slug del 1er servicio | `cerrajero-urgente` |
| 2.04 | Se define el slug del 2º servicio | `apertura-puertas` |
| 2.05 | Se define el slug del 3er servicio | `cambio-cerraduras` |
| 2.06 | Se define el slug del 4º servicio | `cambio-bombines` |
| 2.07 | Se define el slug del 5º servicio | `instalacion-cerraduras-seguridad` |
| 2.08 | Se define el slug de la categoría adicional con página | `duplicado-llaves` |

---

## B. Aplicación de servicios a Main City (1 decisión)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 2.09 | Se decide si todos los servicios aplican a la Main City | Yes (sin exclusiones) |

---

## C. Variables y total (4 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 2.10 | Se calcula la variable S (servicios core) | 5 |
| 2.11 | Se calcula la variable A (categorías adicionales efectivas) | 1 |
| 2.12 | Se aplica la variable G (GeoArticles por servicio) | 3 |
| 2.13 | Se calcula el total de páginas base | 28 |

---

## D. Inventario por tipo de página (6 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 2.14 | Cantidad de Homepage | 1 |
| 2.15 | Cantidad de Service Overview | 5 |
| 2.16 | Cantidad de Main City GeoHub | 1 |
| 2.17 | Cantidad de Main City Location-Based Service | 5 |
| 2.18 | Cantidad de Páginas de categoría adicional | 1 |
| 2.19 | Cantidad de GeoArticles Main City | 15 |

---

## E. Expansión opcional (1 decisión)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 2.20 | Páginas de expansión opcional para fase 1 | 0 (None in Phase 1) |

---

**Total decisiones detectadas en el paso 2: 20**

**Distribución por bloque:**
- A. Slugs: 8
- B. Aplicación de servicios a Main City: 1
- C. Variables y total: 4
- D. Inventario por tipo de página: 6
- E. Expansión opcional: 1
