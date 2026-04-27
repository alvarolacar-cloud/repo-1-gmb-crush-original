# Paso 9 — QA Checklist

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

## Bloque 1 — Ejemplo desarrollado

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 9.01 · Paso-09 §7 Regla 1 URL QA | Se decide auditar como ejemplo una LBS concreta | GMB Crush | La LBS es la página crítica del sistema. Se usa como ejemplo canónico de QA porque concentra más requisitos. | /cerrajero/madrid/cerrajero-urgente/ |
| 9.02 · Paso-09 §21 URL y page type correctos | Se asigna ID de QA | GMB Crush | El ID de QA permite controlar el estado de auditoría por URL de forma sistemática. | LBS-001 |
| 9.03 · Paso-09 §8 Regla 2 Page Type QA | Se define el tipo de página auditada | GMB Crush | El tipo de página determina qué checks aplican. Cada tipo tiene su propio conjunto de requisitos QA. | Location-Based Service |
| 9.04 · Paso-09 §9 Regla 3 One service only | Se define el servicio objetivo | IA sin respaldo | El servicio concreto está pendiente de validación con datos reales. | Cerrajero urgente |
| 9.05 · Paso-09 §10 Regla 4 One Main City only | Se define la Main City | Input humano | Madrid viene directamente de la dirección aportada por el cliente. | Madrid |
| 9.06 · Paso-09 §20 Final Publish Gate | Se define estado de QA | IA sin respaldo | Estado operativo asignado en el ejemplo. No representa una validación real realizada. | Ready for QA |
| 9.07 · Paso-09 §30 Final Approval documentado | Se define reviewer | IA sin respaldo | Rol genérico no asociado a persona real. Debe asignarse en ejecución real. | SEO Manager |
| 9.08 · Paso-09 §30 Final Approval documentado | Se define fecha de QA | IA sin respaldo | Fecha generada para el ejemplo. No corresponde a un calendario real confirmado. | 2026-04-24 |

## Bloque 2 — Checks obligatorios

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 9.09–9.20 · Paso-09 §19 QA por tipo de página | Se deciden checks obligatorios de QA | GMB Crush | El QA refleja todos los requisitos de estructura, schema, links, NAP y no falsa ubicación definidos en el framework. | parent page, GeoHub, related services, GeoArticle, schema, NAP, CTA, no falsa ubicación, no canibalización |

## Bloque 3 — Inventario QA

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 9.21 · Paso-09 §20 Final Publish Gate | Se decide que inventario SEO base tenga QA Status | GMB Crush | Ninguna URL puede publicarse sin pasar el QA Gate. El sistema exige aprobación explícita antes de producción. | 28 URLs |
| 9.22 · Paso-09 §26 NAP consistente | Se decide que /contacto/ también pase QA operativo | GMB Crush | La página de contacto debe ser funcional y consistente con el NAP del negocio, aunque no sea URL SEO base. | Página auxiliar |
| 9.23 · Paso-09 §20 Final Publish Gate | Se decide que resto de URLs queden Pending hasta ejecución real | GMB Crush | El estado Pending evita asumir aprobación no realizada. Todas las URLs parten de QA Pending hasta revisión explícita. | QA Pending |
