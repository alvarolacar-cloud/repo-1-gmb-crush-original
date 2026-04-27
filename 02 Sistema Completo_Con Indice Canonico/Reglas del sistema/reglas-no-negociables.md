# Reglas no negociables — Sistema GMB Crush V6.4

Las reglas estructurales que definen el sistema. Si una se viola, el sistema deja de ser coherente.

Cada regla apunta a su sección canónica donde se define con detalle (`paso-XX §Y`).

---

## A. Arquitectura base

1. **Fórmula maestra**: `1 + S + 1 + S + A + G×S = 28 páginas SEO base`. Con S=5 servicios core, A=1 categoría adicional con página, G=3 GeoArticles por servicio.
   → paso-02 §16, paso-13 §21

2. **`/contacto/` es página auxiliar**, no entra en el cálculo de las 28 SEO base.
   → paso-02 §16

3. **Una sola Main City crea la arquitectura**. No se multiplica la fórmula por zonas de cobertura.
   → paso-02 §8 (Regla 1), paso-02 §21

4. **Web first, GBP después**. El GBP se crea en paso 14, después de publicar la web base.
   → paso-14 §7 (Regla operativa)

5. **La URL Matrix es la fuente de verdad**. Si una página no existe en la matriz, no existe en producción.
   → paso-03 §27

---

## B. Geografía operativa

6. **Direct Local Coverage Areas** salen directamente de la dirección física del NAP.
   → paso-01 §35

7. **Candidate Local Coverage Areas** requieren pasar el **test de coherencia GEO**: cumplir al menos 3 de 6 criterios (ancla física, Main City, proximidad, intención local, demanda/competencia, no falsa ubicación).
   → paso-01 §34

8. **Las Local Coverage Areas NO generan URLs por defecto**. Se usan en contenido, FAQs, ejemplos locales y schema `areaServed`. Mencionar una zona ≠ crear una página.
   → paso-01 §15, paso-04 §15 (Regla 9), paso-06 §10

9. **Solo Approved Expansion Areas pueden generar URLs nuevas** y solo si hay justificación: demanda, valor comercial, oportunidad competitiva, contenido único.
   → paso-01 §16, §26, paso-06 §32

10. **No se inventa ubicación física en zonas de cobertura**. "Atendemos en Almagro" ≠ "tenemos oficina en Almagro".
    → paso-01 §24, paso-06 §11

---

## C. Page types

11. **Homepage = Root Entity Anchor**. URL = `/`. Siempre P1. Establece marca, categoría GBP principal, Main City, NAP, servicios core, enlaces clave.
    → paso-05 §7, paso-08 §16

12. **Service Overview = pillar temático sin ciudad**. URL `/[category]/[service]/`. NO geolocalizada — su función es autoridad temática, no conversión local.
    → paso-05 §8, paso-04 §10

13. **Location-Based Service = convertidor local**. URL `/[category]/[main-city]/[service]/`. Un servicio + una Main City. NO mezclar varios servicios ni varias ciudades en una página.
    → paso-05 §9, paso-04 §12, paso-09 §9

14. **GeoHub = índice de Main City**. URL `/[main-city]/`. Agrupa servicios, categorías adicionales, GeoArticles y cobertura local.
    → paso-05 §11, paso-04 §11

15. **GeoArticle = booster semántico, NO landing comercial**. URL `/[main-city]/[topic]/`. Apoya un LBS específico con contenido long-tail. Siempre enlaza a su LBS padre.
    → paso-05 §12, paso-07 §13

---

## D. URLs y schema

16. **Una intención = una URL** (anti-canibalización). No crear dos páginas para la misma búsqueda.
    → paso-04 §21 (Regla 15), paso-09 §17

17. **Slugs limpios**: minúsculas, guiones medios, sin acentos, sin símbolos. **No usar** `near-me`, `best`, `cheap`, `top-rated` en URLs.
    → paso-04 §19 (Regla 13), paso-04 §17–§18

18. **Trailing slash uniforme**. Decisión binaria (con o sin), aplicada consistentemente en todo el sitio.
    → paso-04 §8

19. **Schema asignado por page type**:
    - Homepage: Organization + WebSite + LocalBusiness (si hay presencia física) + FAQPage
    - Service Overview: Service + WebPage + BreadcrumbList
    - LBS: LocalBusiness + BreadcrumbList
    - Additional Category: Service con `areaServed` + BreadcrumbList
    - GeoHub: CollectionPage + BreadcrumbList
    - GeoArticle: Article + FAQPage + BreadcrumbList + Speakable
    → paso-05 §19, paso-03 §22

20. **NAP único y consistente** en homepage, footer, página de contacto, schema y GBP. Una sola versión canónica.
    → paso-01 §19 (Regla operativa 1)

---

## E. GBP y confianza

21. **GBP Status = Not Created hasta paso 14**. Antes del paso 14: las categorías son `Planned`, no se inserta GBP URL en schema, no hay sameAs, no hay reseñas de Google.
    → paso-01 §1.4, paso-09 §33

22. **No se reclaman reseñas de Google antes de tener el perfil**. Antes del paso 14, los trust signals son cosas verificables (años de experiencia, certificaciones, garantías), nunca "250+ reseñas".
    → paso-14 §15

23. **`core_services` (variable interna) ≠ GBP Services (perfil)**. No mezclar los dos conjuntos. Una categoría adicional GBP con página propia se gestiona por `additional_categories_with_page`, NO entra en `core_services`.
    → Nota doctrinal al final de pasos 1, 5, 11, 14

24. **Categorías GBP confirmadas solo con soporte web real**. No añadir una categoría adicional al GBP si no hay página web que la respalde.
    → paso-14 §14

25. **Trust signals deben ser verificables y reutilizables**. Años, certificaciones, premios, garantías reales. No inventar.
    → paso-01 §25 (Regla operativa 7)

---

## F. Producción y QA

26. **Dependencias de páginas**: GeoArticles solo se publican después de su LBS padre. LBS solo después de su Service Overview padre y del GeoHub.
    → paso-02 §14 (Regla 7), paso-10 §13, paso-11 §20 (bloque 14)

27. **Sin QA aprobado no se publica**. Cada página debe pasar el QA Checklist antes de subir a producción.
    → paso-09 §20 (Final Publish Gate), paso-12 §32

28. **Producción en 5 fases con orden lógico**: Entity Foundation → Main City Conversion → Semantic Expansion → Optimization Loop → Optional Expansion. No saltar fases ni invertir el orden.
    → paso-10 §7–§11

---

## Cómo usar este documento

- **Si vas a editar el sistema**: lee estas 28 reglas antes. Cualquier cambio debe ser compatible.
- **Si encuentras una violación**: marca el archivo y la línea, y consulta la sección canónica para entender el porqué.
- **Si propones una excepción**: documéntala en `CHANGELOG.md` con justificación. No vale "es un caso especial" sin más.
- **Si una regla parece arbitraria**: lee la sección canónica completa. Suele haber una razón estructural detrás.

> Estas reglas no son sugerencias. Son los pilares que mantienen el sistema coherente entre los 14 pasos y replicable en cualquier negocio local.
