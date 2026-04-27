# Sistema GMB Crush para webs locales — V6.1 Cerrajeros Madrid 24h — basada en V5

Este directorio contiene los 14 documentos del sistema GMB Crush para construir una web local desde cero.

Esta versión se basa en la V5, mantiene su estructura, profundidad y formato, y añade el escenario web-first con GBP posterior para:

```text
Negocio: Cerrajeros Madrid 24h
Dirección: Calle Rafael Calvo 12, Barrio Almagro, Distrito Chamberí, Madrid
Main City: Madrid
```

## Lógica base del sistema

Esta versión parte de la V5 y añade el escenario web-first: el GBP no existe todavía, la web se construye primero y el GBP se crea y sincroniza después en el Paso 14.

```text
Main City = crea la arquitectura base.
Local Coverage Areas = enriquecen contenido, FAQs, ejemplos locales y schema areaServed.
Approved Expansion Areas = generan URLs propias solo cuando se aprueban.
```

## Regla clave

```text
Las Local Coverage Areas no generan URLs por defecto.
```

Se usan como señales GEO dentro del contenido, FAQs, ejemplos locales, secciones de cobertura y schema `areaServed`.

## Índice

```text
01. Intake Form
02. Fórmula Maestra de Arquitectura
03. Matriz Base
04. URL Rules
05. Page Type Rules
06. Estructura de Contenido + Áreas de Cobertura Local
07. Internal Linking Rules
08. Priority Score
09. QA Checklist
10. Producción en Fases
11. Pseudocódigo del Sistema
12. Master Prompt Reutilizable
13. Sistema Final Operativo
14. GBP Creation & Website Alignment
```

## Archivos

```text
01-intake-form.md
02-formula-maestra-arquitectura.md
03-matriz-base.md
04-url-rules.md
05-page-type-rules.md
06-estructura-contenido-areas-cobertura-local.md
07-internal-linking-rules.md
08-priority-score.md
09-qa-checklist.md
10-produccion-en-fases.md
11-pseudocodigo-sistema.md
12-master-prompt.md
13-sistema-final-operativo.md
14-gbp-creation-website-alignment.md
gmb-crush-sistema-completo-v6-1-based-on-v5.md
```

## Validación aplicada

- Se mantiene la estructura fija: cabecera, índice corto, objetivo, campos a rellenar, ejemplo rellenado, cuerpo operativo, checklist y outputs.
- Se usa Cerrajeros Madrid 24h como negocio de ejemplo en todos los documentos.
- Se mantiene el modelo Main City + Local Coverage Areas + Approved Expansion Areas.
- El ejemplo geográfico queda centrado en Madrid y sus Local Coverage Areas.
- Se eliminan referencias antiguas a servicios en inglés del ejemplo anterior.
- Cada regla operativa mantiene nombre semántico y contenido específico.
- Las Local Coverage Areas no generan URLs por defecto.
