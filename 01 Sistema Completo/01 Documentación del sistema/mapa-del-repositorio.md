# Mapa del repositorio

Última actualización: 29 abril 2026

---

## Estructura general

```text
repos-1-y-2/
├── 01 Sistema Completo/       ← sistema canónico GMB Crush V6.4
├── 02 Varios/                 ← versiones anteriores y ejemplos
└── README.md
```

---

## 01 Sistema Completo

El sistema GMB Crush completo: 19 pasos en 6 bloques + documentación + reglas.

### Bloques

| Bloque | Nombre | Pasos | Qué hace |
|---|---|---|---|
| 1 | Fundamentos | 1–3 | Intake del cliente, fórmula de arquitectura, matriz base de URLs |
| 2 | Arquitectura | 4–7 | Reglas de URL, tipos de página, contenido local, internal linking |
| 3 | Priorización | 8–10 | Priority score, QA base, plan de producción en fases |
| 4 | Automatización | 11–13 | Pseudocódigo, master prompt, sistema final operativo |
| 5 | Salida a Mercado | 15–19 | Redacción, diseño, construcción, QA/deploy, escalado |
| 6 | GBP | 14 | Creación de Google Business Profile y alineación con la web |

### Archivos por paso

Cada carpeta de paso tiene 2 archivos canónicos:

- `XXa-ejecucion-{nombre}.md` — reglas, fórmulas, ejemplo ejecutado.
- `XXb-decisiones-tomadas-y-fuentes.md` — cada decisión con su fuente, qué dicta y dato en cascada (modelo final con 7 columnas).

Excepción: el Paso 15 tiene un tercer archivo `15c-content-pack-por-url.md` con el contenido final por URL listo para construcción.

### Bloque 5 — archivos adicionales en raíz

El Bloque 5 tiene 4 archivos meta en su raíz:

- `README.md` — visión general del bloque y reglas de integración con pasos 1–14.
- `INDICE-PACK-COMPLETO.md` — índice de todos los archivos con orden de uso.
- `indice-capa-salida-mercado.md` — índice corto con líneas por archivo.
- `VALIDACION-PACK-COMPLETO.md` — verificación de archivos incluidos y conteo de decisiones.

### Carpetas auxiliares

| Carpeta | Qué contiene |
|---|---|
| `01 Documentación del sistema/` | Catálogo de fuentes, mapa del repositorio, reglas no negociables, reglas relevantes del sistema, README general y índice temático |
| `Taller/` | Borradores y versiones intermedias de decisiones/fuentes (V1 y V2). No son canónicos. |

### Documentación del sistema — archivos

Dentro de `01 Documentación del sistema/`:

- `README.md` — presentación general del sistema.
- `indice-tematico.md` — índice temático cruzado.
- `mapa-del-repositorio.md` — este documento.
- `catalogo-de-fuentes.md` — modelo de Fuentes y Dato en cascada para los archivos `Xb`.
- `reglas-no-negociables.md` — 28 reglas estructurales del framework.
- `reglas-relevantes-sistema-gmb-crush.md` — referencia rápida de reglas operativas.

---

## 02 Varios

Versiones anteriores del sistema y ejemplos ejecutados con otros negocios. No son canónicos.

| Carpeta | Qué es |
|---|---|
| `01 Sistema_Vision Rapida/` | Primera versión del sistema (12 pasos, monolítico) |
| `Cerrajeros-Madrid-V5/` | Ejemplo ejecutado V5 con 13 pasos |
| `Miami-ABC-Locksmith-V4/` | Ejemplo ejecutado V4 en inglés (Miami) |
| `Sistema_ Vision Completa/` | Versión con 14 pasos + decisiones V1 por paso |

---

## Números clave

| Dato | Valor |
|---|---|
| Pasos canónicos | 19 |
| Bloques | 6 |
| Decisiones trazadas (pasos 1–14) | 334 |
| Decisiones trazadas (pasos 15–19) | 160 |
| Total decisiones | 494 |
| Fuentes en el catálogo | 6 únicas + 4 combinaciones (10 valores) |
| Filas con cascada `← X.YY` | 199 (~40%) |
| Filas pendientes de validación | 68 (~14%) |
