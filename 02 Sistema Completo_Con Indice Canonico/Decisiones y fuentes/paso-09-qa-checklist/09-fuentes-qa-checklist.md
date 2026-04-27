# Paso 9 — QA Checklist

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

## Bloque 1 — Ejemplo desarrollado

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 9.01 | Se decide auditar como ejemplo una LBS concreta | /cerrajero/madrid/cerrajero-urgente/ | GMB Crush | LBS es página crítica para QA. | Validada |
| 9.02 | Se asigna ID de QA | LBS-001 | GMB Crush | ID permite control de QA por URL. | Validada |
| 9.03 | Se define el tipo de página auditada | Location-Based Service | GMB Crush | Tipo de página del framework. | Validada |
| 9.04 | Se define el servicio objetivo | Cerrajero urgente | IA sin respaldo | Servicio pendiente de validación. | Pendiente de validación |
| 9.05 | Se define la Main City | Madrid | Input humano | Madrid sale de dirección. | Validada |
| 9.06 | Se define estado de QA | Ready for QA | IA sin respaldo | Estado operativo asignado en el ejemplo, no validación real. | Pendiente de validación |
| 9.07 | Se define reviewer | SEO Manager | IA sin respaldo | Rol genérico no asociado a persona real. | Pendiente de validación |
| 9.08 | Se define fecha de QA | 2026-04-24 | IA sin respaldo | Fecha generada en ejemplo, no calendario real confirmado. | Pendiente de validación |

## Bloque 2 — Checks obligatorios

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 9.09-9.20 | Se deciden checks obligatorios de QA | parent page, GeoHub, related services, GeoArticle, schema, NAP, CTA, no falsa ubicación, no canibalización | GMB Crush | QA refleja requisitos de estructura, schema, links, NAP y no falsa ubicación. | Validada |

## Bloque 3 — Inventario QA

| ID | Decisión tomada | Valor decidido en el ejemplo | Fuente | Justificación | Estado |
|---|---|---|---|---|---|
| 9.21 | Se decide que inventario SEO base tenga QA Status | 28 URLs | GMB Crush | Ninguna URL debe publicarse sin QA. | Validada |
| 9.22 | Se decide que /contacto/ también pase QA operativo | Página auxiliar | GMB Crush | Contacto debe ser funcional y consistente con NAP. | Validada |
| 9.23 | Se decide que resto de URLs queden Pending hasta ejecución real | QA Pending | GMB Crush | Estado pendiente evita asumir aprobación no realizada. | Validada |

