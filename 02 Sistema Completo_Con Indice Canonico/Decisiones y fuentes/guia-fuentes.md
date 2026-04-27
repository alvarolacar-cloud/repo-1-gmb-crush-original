# Guía de fuentes — Cómo rellenar las tablas de trazabilidad

Cada archivo de fuentes (`XX-fuentes-nombre-paso.md`) tiene 5 columnas:

```
ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo
```

Las dos columnas que hay que rellenar son **Fuente para la decisión** y **Funcionamiento de la fuente**. Están directamente vinculadas: para cada valor de fuente hay una frase fija de funcionamiento.

---

## Tabla de referencia

| Fuente para la decisión | Funcionamiento de la fuente |
|---|---|
| Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. |
| GMB Crush | El framework define esta regla. Se aplica igual en todos los proyectos. |
| Input humano + GMB Crush | El cliente proporciona el dato y el framework determina cómo usarlo. |
| Geografía | Se deriva de la ubicación física del negocio o de la proximidad geográfica a la Main City. |
| Input humano + Geografía | El cliente aporta la dirección y la geografía determina las zonas de cobertura. |
| GMB Crush + Geografía | El framework define el uso de zonas; la geografía determina cuáles aplican. |
| Datos de búsqueda | Se valida con volumen de búsqueda real. Requiere keyword research antes de confirmar. |
| Competidores | Se valida con análisis de competencia. Requiere revisión antes de confirmar. |
| IA sin respaldo | Valor generado para el ejemplo sin dato real. Debe sustituirse en ejecución real. |
| GMB Crush + IA sin respaldo | El patrón es del framework pero el valor concreto está pendiente de validación. |
| Input humano + IA sin respaldo | El dato base es del cliente pero algún campo concreto está pendiente de confirmación. |

---

## Cómo rellenar una fila

1. Rellena **Fuente para la decisión** con uno de los valores de la tabla anterior.
2. Copia la frase fija correspondiente en **Funcionamiento de la fuente**.
3. Si la decisión tiene un matiz específico que la frase fija no cubre, añádelo al final separado por un punto.

**Ejemplo:**

| ID · Ref. canónica | Decisión que se toma | Fuente para la decisión | Funcionamiento de la fuente | Decisión en el ejemplo |
|---|---|---|---|---|
| 1.01 · Paso-01 §7 Business Name | Se define el nombre del negocio | Input humano | El cliente proporciona este dato directamente. El sistema lo recoge sin transformación. | Cerrajeros Madrid 24h |
| 1.03 · Paso-01 §8 Website URL | Se define el dominio canónico | IA sin respaldo | Valor generado para el ejemplo sin dato real. Debe sustituirse en ejecución real. | https://www.cerrajerosmadrid24h.com |
| 3.04 · Paso-03 §9 Fórmula base | Se calcula el volumen total de páginas | GMB Crush + IA sin respaldo | El patrón es del framework pero el valor concreto está pendiente de validación. La fórmula es 1+S+1+S+A+G×S; los valores de S y A dependen del cliente. | 28 páginas |

---

## Valores de fuente disponibles

```text
Input humano
GMB Crush
Input humano + GMB Crush
Geografía
Input humano + Geografía
GMB Crush + Geografía
Datos de búsqueda
Competidores
IA sin respaldo
GMB Crush + IA sin respaldo
Input humano + IA sin respaldo
```
