# Sistema GMB Crush — V6.4

Sistema de 19 pasos en 6 bloques para construir webs locales optimizadas para SEO + GBP. Web-first, con GBP como cierre del ecosistema.

---

## Cómo leer el sistema

1. Este `README.md` — entrada del sistema, principios y estructura.
2. `reglas-del-sistema.md` — las reglas estructurales y operativas.
3. `indice-tematico.md` — índice cruzado de conceptos con referencia canónica `§X`.
4. `catalogo-de-fuentes.md` — modelo de Fuentes para los archivos `Xb` de cada paso.
5. Los 19 pasos en orden de bloques (ver tabla abajo).

---

## Estructura del repositorio

```text
repos-1-y-2/
├── 01 Sistema Completo/       ← sistema canónico GMB Crush V6.4
│   ├── 01 Documentación del sistema/   ← este README + 3 docs auxiliares + auditoría
│   ├── 02 Ejecución del sistema/       ← los 19 pasos en 6 bloques
│   │   ├── Bloque 1 — Fundamentos/         ← pasos 1–3
│   │   ├── Bloque 2 — Arquitectura/        ← pasos 4–7
│   │   ├── Bloque 3 — Priorizacion/        ← pasos 8–10
│   │   ├── Bloque 4 — Automatizacion/      ← pasos 11–13
│   │   ├── Bloque 5 — Salida a Mercado/    ← pasos 15–19
│   │   └── Bloque 6 — GBP/                 ← paso 14
│   ├── 03 Taller/                      ← borradores y versiones intermedias (no canónicas)
│   └── 04 Varios/                      ← versiones anteriores y ejemplos en otros negocios
└── README.md
```

### Bloques y pasos

| Bloque | Pasos | Qué hace |
|---|---|---|
| 1 — Fundamentos | 1–3 | Intake del cliente, fórmula de arquitectura, matriz base de URLs |
| 2 — Arquitectura | 4–7 | URL Rules, Page Type Rules, estructura de contenido + LCAs, internal linking |
| 3 — Priorización | 8–10 | Priority Score, QA Checklist, plan de producción en fases |
| 4 — Automatización | 11–13 | Pseudocódigo, Master Prompt, sistema final operativo |
| 5 — Salida a Mercado | 15–19 | Redacción, extracción de diseño, construcción, QA + deploy, escalado |
| 6 — GBP | 14 | Creación del Google Business Profile y alineación con la web |

### Orden de ejecución real

```text
1 → 2 → 3 → 4 → 5 (15-18) → 6 (14) → 5 (19)
```

El Paso 14 (GBP) se ejecuta tras la web base (15-18) y antes del módulo de escalado (19).

---

## Archivos por paso

Cada carpeta de paso tiene 2 archivos canónicos:

- `XXa-ejecucion-{nombre}.md` — reglas, fórmulas, ejemplo ejecutado con `§X` en cada encabezado.
- `XXb-decisiones-tomadas-y-fuentes.md` — cada decisión con su Fuente, Qué dicta la fuente, Dato en cascada y referencia canónica `§X`.

Excepción: el Paso 15 tiene un tercer archivo `15c-content-pack-por-url.md` con el contenido final por URL listo para construcción.

### Archivos meta del Bloque 5

- `README.md` — visión general del bloque.
- `INDICE-PACK-COMPLETO.md` — índice de archivos con orden de uso.
- `indice-capa-salida-mercado.md` — índice corto.
- `VALIDACION-PACK-COMPLETO.md` — verificación y conteo de decisiones.

---

## Principios del sistema

- **Web first, GBP después.** El GBP se crea en el Paso 14, después de publicar la web base.
- **Main City única** crea la arquitectura. No se multiplica por zonas.
- **Local Coverage Areas no generan URLs por defecto.** Refuerzan contenido y schema.
- **Approved Expansion Areas** generan URLs solo con aprobación explícita.
- **28 páginas SEO base:** `1 + S + 1 + S + A + G×S` (con S=5 servicios, A=1 categoría adicional, G=3 GeoArticles).
- **GBP Status = Not Created hasta el Paso 14.** Antes: categorías "Planned", sin GBP URL en schema, sin sameAs, sin reseñas.

Las 28 reglas estructurales completas: ver `reglas-del-sistema.md`.

---

## Trazabilidad de decisiones

Los archivos `XXb-decisiones-tomadas-y-fuentes.md` usan **7 columnas**:

```text
ID | Decisión | Ejemplo | Fuente | Qué dicta la fuente | Dato en cascada | Funcionamiento
```

- **Fuentes permitidas:** GMB Crush, Input humano, Decisión de diseño, Competidores, Datos de búsqueda, IA sin respaldo.
- **Combinaciones permitidas con `+`:** GMB Crush + Competidores, GMB Crush + Datos de búsqueda, GMB Crush + IA sin respaldo, GMB Crush + Input humano.
- **Dato en cascada:** `no` o `← X.YY`.
- **Total decisiones trazadas:** 494 en los 19 pasos.

Detalle completo del modelo: `catalogo-de-fuentes.md`.

---

## Estado

```text
Versión:         V6.4 (estado cerrado)
Última revisión: 2026-04-29
Decisiones:      494 trazadas (425 cerradas, 68 pendientes de validación)
Cascadas:        199 filas con `← X.YY` (~40%)
Cambios:         19 pasos consolidados, índice canónico §X, modelo de Fuentes
                 con Qué dicta + Dato en cascada, Direct/Candidate LCAs,
                 28 páginas SEO base, Bloque GBP (paso 14) separado.
```

---

## 04 Varios

Versiones anteriores del sistema y ejemplos ejecutados con otros negocios. No son canónicos.

| Carpeta | Qué es |
|---|---|
| `01 Sistema_Vision Rapida/` | Primera versión del sistema (12 pasos, monolítico) |
| `Cerrajeros-Madrid-V5/` | Ejemplo ejecutado V5 con 13 pasos |
| `Miami-ABC-Locksmith-V4/` | Ejemplo ejecutado V4 en inglés (Miami) |
| `Sistema_ Vision Completa/` | Versión con 14 pasos + decisiones V1 por paso |
