# Auditoría de trazabilidad — Paso 8: Priority Score

Documento auditado: `08-priority-score.md`
Sección: "Ejemplo rellenado" + "Tabla de prioridad para Cerrajeros Madrid 24h" + "Orden recomendado"
Negocio: Cerrajeros Madrid 24h

---

## A. Scores asignados por página (10 decisiones)

Cada fila muestra las 6 puntuaciones del scoring (Revenue, Search Intent, GBP Category Relevance, Local Relevance, Competition Gap, Conversion Urgency), el total y el tier resultante.

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 8.01 | Score Homepage (`/`) | R=5, I=5, G=5, L=5, Gap=4, U=5 → 29 → P1 |
| 8.02 | Score SO `/cerrajero/cerrajero-urgente/` | R=5, I=5, G=5, L=4, Gap=4, U=5 → 28 → P1 |
| 8.03 | Score SO `/cerrajero/apertura-puertas/` | R=4, I=5, G=4, L=4, Gap=4, U=5 → 26 → P1 |
| 8.04 | Score GeoHub `/madrid/` | R=4, I=4, G=5, L=5, Gap=4, U=4 → 26 → P1 |
| 8.05 | Score LBS `/cerrajero/madrid/cerrajero-urgente/` | R=5, I=5, G=5, L=5, Gap=4, U=5 → 29 → P1 |
| 8.06 | Score LBS `/cerrajero/madrid/apertura-puertas/` | R=4, I=5, G=4, L=5, Gap=4, U=5 → 27 → P1 |
| 8.07 | Score LBS `/cerrajero/madrid/cambio-bombines/` | R=5, I=4, G=4, L=5, Gap=3, U=4 → 25 → P2 |
| 8.08 | Score LBS `/cerrajero/madrid/cambio-cerraduras/` | R=4, I=4, G=4, L=5, Gap=3, U=4 → 24 → P2 |
| 8.09 | Score AC `/cerrajero/madrid/duplicado-llaves/` | R=2, I=3, G=4, L=5, Gap=3, U=2 → 19 → P3 |
| 8.10 | Score GA `/madrid/guia-precios-cerrajero-urgente/` | R=3, I=3, G=4, L=5, Gap=4, U=3 → 22 → P2 (after landing) |

---

## B. Notas estratégicas (1 decisión)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 8.11 | Notas estratégicas del LBS ejemplo | "Urgentee cerrajero is high-value, urgente, directly aligned with cerrajero intent, and important for Madrid Local Pack visibility" |

---

## C. Orden recomendado de publicación (1 decisión)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 8.12 | Orden de publicación | 1. Homepage → 2. SO prioritarias → 3. Main City GeoHub → 4. Madrid cerrajero urgente/apertura/cambio bombines → 5. Páginas servicio restantes → 6. AC → 7. GeoArticle clusters → 8. Optimización y revisión de expansión |

---

**Total decisiones detectadas en el paso 8: 12**

**Distribución por bloque:**
- A. Scores asignados por página: 10
- B. Notas estratégicas: 1
- C. Orden recomendado de publicación: 1
