# Repo 1 — GMB Crush Website Build System (Versión Original)

Sistema completo en 12 pasos para construir una web local desde cero siguiendo la metodología GMB Crush.

## ¿Qué es este repositorio?

Este repositorio contiene los **12 documentos SOP originales** del sistema GMB Crush, más el documento maestro que los integra en un único flujo operativo. Estos documentos representan la versión de referencia del sistema: esquemas estructurados, fórmulas, reglas y matrices que definen la metodología completa.

> **Nota:** Para la versión expandida con mayor profundidad procedimental, ejemplos detallados y plantillas de producción completas, consulta el **Repo 2 — Versión Literal del Chat**.

---

## Flujo del sistema

```
Input → Architecture → URL Matrix → Page Briefs → Internal Links → Schema → Priority → QA → Publish → Track → Optimize
```

## Jerarquía de páginas

| Nivel | Tipo de Página | Función |
| :---: | :--- | :--- |
| 1 | **Homepage** | Entidad raíz — Root Entity Anchor |
| 2 | **Service Overview Pages** | Autoridad temática — sin ciudad |
| 3 | **Location-Based Service Pages** | Conversión local — servicio + ciudad |
| 4 | **Additional Category Pages** | Soporte de categorías GBP adicionales |
| 5 | **GeoHub Pages** | Contenedores de silo de ciudad |
| 6 | **GeoArticle Pages** | Boosters semánticos de cola larga |

---

## Estructura del repositorio

```
repo-1-gmb-crush-original/
├── README.md                                        ← Este archivo
├── docs/
│   ├── 01_paso-1-intake-form.docx                  ← Recolección de datos del negocio
│   ├── 02_paso-2-formula-maestra-de-arquitectura.docx ← Cálculo del número de páginas
│   ├── 03_paso-3-matriz-base.docx                  ← Matriz URL operativa
│   ├── 04_paso-4-url-rules.docx                    ← Reglas de estructura de URLs
│   ├── 05_paso-5-page-type-rules.docx              ← Plantillas por tipo de página
│   ├── 06_paso-6-internal-linking-rules.docx       ← Mapa de enlaces internos
│   ├── 07_paso-7-priority-score.docx               ← Sistema de priorización P1–P4
│   ├── 08_paso-8-qa-checklist.docx                 ← Control de calidad pre-publicación
│   ├── 09_paso-9-produccion-en-fases.docx          ← Plan de publicación por fases
│   ├── 10_paso-10-pseudocodigo-del-sistema.docx    ← Lógica repetible del sistema
│   ├── 11_paso-11-master-prompt-reutilizable.docx  ← Prompt maestro para IA
│   ├── 12_paso-12-sistema-final-operativo.docx     ← SOP final integrado
│   └── gmb_crush_sistema_completo.docx             ← Documento maestro (todos los pasos)
```

---

## Descripción de cada paso

| Paso | Documento | Objetivo |
| :---: | :--- | :--- |
| 01 | Intake Form | Recoger NAP, categoría GBP, servicios y ciudades antes de crear ninguna URL |
| 02 | Fórmula Maestra | Calcular el total de páginas con la fórmula `1 + S + C + (S×C) + (A×C) + (G×S×C)` |
| 03 | Matriz Base | Convertir la arquitectura en una hoja de cálculo operativa con 18 columnas |
| 04 | URL Rules | Fijar patrones de URL por tipo de página y reglas anti-canibalización |
| 05 | Page Type Rules | Definir H1, metadata, schema, word count y CTAs por tipo de página |
| 06 | Internal Linking | Construir silos de ciudad y servicio mediante enlaces internos estructurados |
| 07 | Priority Score | Puntuar páginas (1–30) para decidir el orden de publicación |
| 08 | QA Checklist | Verificar cada página antes de publicar (URL, schema, NAP, CTA, enlaces) |
| 09 | Producción en Fases | Publicar por fases: Entity Foundation → Local Conversion → Semantic Expansion → Optimization |
| 10 | Pseudocódigo | Expresar el sistema como lógica repetible y automatizable |
| 11 | Master Prompt | Prompt maestro para generar arquitecturas GMB Crush con IA |
| 12 | Sistema Final | SOP integrado de 20 pasos desde intake hasta optimización continua |

---

## Fórmula de arquitectura

```
Total páginas = 1 + S + C + (S × C) + (A × C) + (G × S × C)

Donde:
  S = Servicios principales
  C = Ciudades objetivo
  A = Categorías GBP adicionales (sin duplicados)
  G = GeoArticles por servicio × ciudad
```

**Ejemplo (ABC Locksmith):** 1 + 5 + 5 + (5×5) + (1×5) + (3×5×5) = **111 páginas**

---

## Reglas no negociables

- No crear páginas sin función clara.
- No mezclar servicios en una landing local.
- No mezclar ciudades en una landing local.
- No crear categorías adicionales duplicadas.
- No publicar artículos antes que sus páginas comerciales.
- No fingir ubicación física.
- No dejar páginas huérfanas.
- No publicar sin schema, CTA, enlaces internos ni QA aprobado.

---

*Sistema desarrollado por GMB Crush. Para la versión con mayor detalle operativo, ver Repo 2.*
