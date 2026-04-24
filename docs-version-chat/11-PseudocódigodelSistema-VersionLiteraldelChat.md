**GMB Crush — Paso 11: Pseudocódigo del Sistema**
Versión literal del chat · Sistema GMB Crush para webs locales

Documento generado a partir de la conversación paso a paso sobre el sistema GMB Crush para construir una web local desde cero.


# Índice

**1. Paso 11 — Pseudocódigo del Sistema**


# Paso 11 — Pseudocódigo del sistema


## Objetivo del Paso 10


Ahora convertimos todo lo anterior en una lógica casi automática.

Hasta ahora hemos diseñado el sistema manualmente:

Inputs
Arquitectura
URLs
Tipos de página
Enlaces internos
Prioridades
QA
Fases

En este paso lo convertimos en un motor lógico que pueda generar una matriz completa para cualquier negocio local.


## Lo que tienes que rellenar


Business Name:

Website Root Domain:

Canonical Domain:
https://www.domain.com or https://domain.com

Primary GBP Category:

Primary Category Slug:

Main City:

Physical Location City:

Target Cities:
1.
2.
3.
4.
5.

Core Services:
1.
2.
3.
4.
5.

Service Slugs:
1.
2.
3.
4.
5.

Additional GBP Categories:
1.
2.
3.

Additional Category Slugs:
1.
2.
3.

Additional Categories Already Covered by Core Services:
1.
2.

Effective Additional Categories That Need Pages:
1.
2.

GeoArticles per Service x City:
Default: 3

GeoHub URL Style:
/city/ or /category/city/

GeoArticle URL Style:
/city/article-topic/ or /category/city/article-topic/

Phone:

Email:

NAP:
- Name:
- Address:
- Phone:

GBP URL:

Top Priority Services:
1.
2.
3.

Top Priority Cities:
1.
2.
3.

Publishing Capacity:
Pages per week:

Tracking Tools:
GMB Crush / GSC / GA4 / Other


## Ejemplo rellenado


Business Name:
ABC Locksmith

Website Root Domain:
https://www.abclocksmith.com

Canonical Domain:
https://www.abclocksmith.com

Primary GBP Category:
Locksmith

Primary Category Slug:
locksmith

Main City:
Miami

Physical Location City:
Miami

Target Cities:
1. Miami
2. Hialeah
3. Coral Gables
4. Doral
5. Hollywood

Core Services:
1. Emergency Locksmith
2. Car Locksmith
3. Residential Locksmith
4. Commercial Locksmith
5. Lock Rekeying

Service Slugs:
1. emergency-locksmith
2. car-locksmith
3. residential-locksmith
4. commercial-locksmith
5. lock-rekeying

Additional GBP Categories:
1. Emergency Locksmith Service
2. Key Duplication Service

Additional Category Slugs:
1. emergency-locksmith
2. key-duplication

Additional Categories Already Covered by Core Services:
1. Emergency Locksmith Service

Effective Additional Categories That Need Pages:
1. Key Duplication Service

GeoArticles per Service x City:
3

GeoHub URL Style:
/city/

GeoArticle URL Style:
/city/article-topic/

Phone:
+1 305 000 0000

Email:
info@abclocksmith.com

NAP:
- Name: ABC Locksmith
- Address: 123 Main St, Miami, FL
- Phone: +1 305 000 0000

GBP URL:
https://google.com/business/abc-locksmith

Top Priority Services:
1. Emergency Locksmith
2. Car Locksmith
3. Commercial Locksmith

Top Priority Cities:
1. Miami
2. Hialeah
3. Coral Gables

Publishing Capacity:
5 pages per week

Tracking Tools:
GMB Crush Geo Grid, Google Search Console, GA4


## Pseudocódigo general


START

1. Load business inputs
2. Normalize all names and slugs
3. Validate GBP category alignment
4. Detect duplicate additional categories
5. Generate Homepage
6. Generate Service Overview Pages
7. Generate GeoHub Pages
8. Generate Location-Based Service Pages
9. Generate Additional Category Pages
10. Generate GeoArticle Ideas
11. Assign schema by page type
12. Assign internal links by page type
13. Calculate Priority Score
14. Assign publishing phase
15. Run QA checklist
16. Output URL Matrix
17. Output Internal Linking Matrix
18. Output Schema Map
19. Output Publishing Plan
20. Output QA Status

END


## 1. Cargar inputs


INPUT business_name
INPUT website_root_domain
INPUT canonical_domain
INPUT primary_gbp_category
INPUT primary_category_slug
INPUT main_city
INPUT physical_location_city
INPUT target_cities[]
INPUT core_services[]
INPUT service_slugs[]
INPUT additional_gbp_categories[]
INPUT geoarticles_per_service_city
INPUT phone
INPUT email
INPUT nap
INPUT gbp_url


## 2. Normalizar slugs


FUNCTION generate_slug(text):
    text = lowercase(text)
    text = remove_accents(text)
    text = replace_spaces_with_hyphens(text)
    text = remove_symbols(text)
    text = remove_duplicate_hyphens(text)
    RETURN text

Ejemplo:

"Emergency Locksmith" → "emergency-locksmith"
"Coral Gables" → "coral-gables"
"Key Duplication Service" → "key-duplication"


## 3. Validar categorías adicionales


Objetivo: evitar duplicar páginas cuando una categoría adicional ya está cubierta por un servicio principal.

effective_additional_categories = []

FOR each additional_category IN additional_gbp_categories:
    IF additional_category matches core_service intent:
        mark_as_covered(additional_category)
    ELSE:
        add to effective_additional_categories

Ejemplo:

additional_gbp_categories = [
  "Emergency Locksmith Service",
  "Key Duplication Service"
]

core_services = [
  "Emergency Locksmith",
  "Car Locksmith",
  "Residential Locksmith",
  "Commercial Locksmith",
  "Lock Rekeying"
]

Result:
covered = ["Emergency Locksmith Service"]
effective_additional_categories = ["Key Duplication Service"]


## 4. Generar homepage


CREATE page
page.id = "HP-001"
page.type = "Homepage"
page.url = "/"
page.h1 = "[Business Name] – Trusted [Primary Service] in [Main City, ST]"
page.meta_title = "Top-Rated [Primary Service] in [Main City, ST] | [Business Name]"
page.schema = ["Organization", "WebSite", "LocalBusiness if valid", "FAQPage", "Speakable"]
page.priority = "P1"
page.phase = "Phase 1"
page.status = "Planned"


## 5. Generar Service Overview Pages


FOR each service IN core_services:

    service_slug = generate_slug(service)

    CREATE page
    page.id = "SO-" + counter
    page.type = "Service Overview"
    page.service = service
    page.city = null
    page.url = "/" + primary_category_slug + "/" + service_slug + "/"
    page.h1 = "Professional [Service] Services by [Business Name]"
    page.meta_title = "[Service] by [Business Name] | [Primary Category] Experts"
    page.schema = ["Service", "WebPage", "BreadcrumbList", "Speakable"]
    page.priority = calculate_service_priority(service)
    page.phase = assign_service_phase(priority)


## 6. Generar GeoHub Pages


FOR each city IN target_cities:

    city_slug = generate_slug(city)

    IF geohub_url_style == "/city/":
        url = "/" + city_slug + "/"
    ELSE:
        url = "/" + primary_category_slug + "/" + city_slug + "/"

    CREATE page
    page.id = "GH-" + counter
    page.type = "GeoHub"
    page.city = city
    page.url = url
    page.h1 = "[Business Name] – [Industry] Services in [City]"
    page.meta_title = "[Industry] Services in [City] | [Business Name]"
    page.schema = ["CollectionPage", "BreadcrumbList", "LocalBusiness if physical city"]
    page.priority = calculate_city_priority(city)
    page.phase = assign_geohub_phase(city)


## 7. Generar Location-Based Service Pages


FOR each city IN target_cities:
    FOR each service IN core_services:

        city_slug = generate_slug(city)
        service_slug = generate_slug(service)

        CREATE page
        page.id = "LBS-" + counter
        page.type = "Location-Based Service"
        page.service = service
        page.city = city
        page.url = "/" + primary_category_slug + "/" + city_slug + "/" + service_slug + "/"
        page.h1 = "[Business Name] – [Service] in [City]"
        page.meta_title = "Top [Service] in [City] | [Business Name]"
        page.schema = ["LocalBusiness", "BreadcrumbList", "FAQPage optional", "Speakable optional"]
        page.parent_service = "/" + primary_category_slug + "/" + service_slug + "/"
        page.geohub = "/" + city_slug + "/"
        page.priority_score = calculate_priority(service, city, page.type)
        page.phase = assign_phase(priority_score)


## 8. Generar Additional Category Pages


FOR each city IN target_cities:
    FOR each additional_category IN effective_additional_categories:

        city_slug = generate_slug(city)
        category_slug = generate_slug(additional_category)

        CREATE page
        page.id = "AC-" + counter
        page.type = "Additional Category"
        page.service = additional_category
        page.city = city
        page.url = "/" + primary_category_slug + "/" + city_slug + "/" + category_slug + "/"
        page.h1 = "[Business Name] – Expert [Service] in [City]"
        page.meta_title = "[Service] in [City] | [Business Name]"
        page.schema = ["Service with areaServed", "BreadcrumbList", "FAQPage optional"]
        page.geohub = "/" + city_slug + "/"
        page.priority_score = calculate_priority(additional_category, city, page.type)
        page.phase = assign_phase(priority_score)


## 9. Generar GeoArticle ideas


FOR each city IN target_cities:
    FOR each service IN core_services:
        FOR article_number FROM 1 TO geoarticles_per_service_city:

            article_topic = generate_article_topic(service, city, article_number)
            article_slug = generate_slug(article_topic)

            CREATE page
            page.id = "GA-" + counter
            page.type = "GeoArticle"
            page.service = service
            page.city = city
            page.url = "/" + city_slug + "/" + article_slug + "/"
            page.h1 = "[Article Topic] in [City]"
            page.meta_title = "[Article Topic] in [City] | [Business Name]"
            page.schema = ["Article", "FAQPage", "BreadcrumbList", "Speakable"]
            page.supports = "/" + primary_category_slug + "/" + city_slug + "/" + service_slug + "/"
            page.geohub = "/" + city_slug + "/"
            page.priority = assign_geoarticle_priority(service, city)
            page.phase = "Phase 3"


## 10. Asignar schema por tipo de página


FUNCTION assign_schema(page_type):

    IF page_type == "Homepage":
        RETURN ["Organization", "WebSite", "LocalBusiness if valid", "FAQPage", "Speakable"]

    IF page_type == "Service Overview":
        RETURN ["Service", "WebPage", "BreadcrumbList", "Speakable"]

    IF page_type == "Location-Based Service":
        RETURN ["LocalBusiness", "BreadcrumbList", "FAQPage optional", "Speakable optional"]

    IF page_type == "Additional Category":
        RETURN ["Service with areaServed", "BreadcrumbList", "FAQPage optional"]

    IF page_type == "GeoHub":
        RETURN ["CollectionPage", "BreadcrumbList", "LocalBusiness if valid"]

    IF page_type == "GeoArticle":
        RETURN ["Article", "FAQPage", "BreadcrumbList", "Speakable"]


## 11. Asignar enlaces internos


FUNCTION assign_internal_links(page):

    IF page.type == "Homepage":
        link_to Service Overview Pages
        link_to Main GeoHub
        link_to Main Additional Category Pages
        link_to Contact Page

    IF page.type == "Service Overview":
        link_to Homepage
        link_to all city-specific versions of same service
        link_to related Service Overview Pages
        link_to relevant GeoArticle

    IF page.type == "Location-Based Service":
        link_to parent Service Overview
        link_to matching GeoHub
        link_to other services in same city
        link_to same service in nearby cities
        link_to related GeoArticles
        link_to Contact Page

    IF page.type == "Additional Category":
        link_to matching GeoHub
        link_to related services in same city
        link_to related GeoArticles
        link_to Contact Page

    IF page.type == "GeoHub":
        link_to Homepage
        link_to all services in city
        link_to all additional categories in city
        link_to all GeoArticles in city
        link_to Contact Page

    IF page.type == "GeoArticle":
        link_to matching Location-Based Service Page
        link_to matching GeoHub
        link_to related GeoArticle
        link_to Contact Page


## 12. Calcular Priority Score


FUNCTION calculate_priority(service, city, page_type):

    revenue_value = get_revenue_value(service)
    search_intent = get_search_intent(service, page_type)
    gbp_relevance = get_gbp_relevance(service, primary_gbp_category, additional_categories)
    city_priority = get_city_priority(city)
    competition_gap = estimate_competition_gap(service, city)
    conversion_urgency = get_conversion_urgency(service)

    total_score =
        revenue_value
        + search_intent
        + gbp_relevance
        + city_priority
        + competition_gap
        + conversion_urgency

    IF total_score >= 26:
        priority = "P1"
    ELSE IF total_score >= 21:
        priority = "P2"
    ELSE IF total_score >= 16:
        priority = "P3"
    ELSE IF total_score >= 10:
        priority = "P4"
    ELSE:
        priority = "Hold"

    RETURN total_score, priority


## 13. Asignar fase de publicación


FUNCTION assign_publish_phase(page):

    IF page.type == "Homepage":
        RETURN "Phase 1"

    IF page.type == "Contact":
        RETURN "Phase 1"

    IF page.type == "Service Overview" AND page.priority == "P1":
        RETURN "Phase 1"

    IF page.type == "GeoHub" AND page.city == main_city:
        RETURN "Phase 1"

    IF page.type == "Location-Based Service" AND page.city == main_city:
        RETURN "Phase 2"

    IF page.type == "Additional Category" AND page.city == main_city:
        RETURN "Phase 2"

    IF page.type == "GeoHub" AND page.city != main_city:
        RETURN "Phase 2"

    IF page.type == "Location-Based Service" AND page.city != main_city:
        RETURN "Phase 2 or Phase 3 depending priority"

    IF page.type == "GeoArticle":
        RETURN "Phase 3"

    ELSE:
        RETURN "Phase 4 or Hold"


## 14. Comprobar dependencias


FUNCTION check_dependencies(page):

    IF page.type == "Location-Based Service":
        REQUIRE Homepage exists
        REQUIRE parent Service Overview exists
        REQUIRE matching GeoHub exists

    IF page.type == "Additional Category":
        REQUIRE Homepage exists
        REQUIRE matching GeoHub exists
        REQUIRE related services exist

    IF page.type == "GeoArticle":
        REQUIRE matching Location-Based Service Page exists
        REQUIRE matching GeoHub exists

    IF dependencies_missing:
        page.status = "Blocked"
    ELSE:
        page.status = "Ready for QA"


## 15. Ejecutar QA


FUNCTION run_qa(page):

    CHECK url_matches_page_type
    CHECK h1_matches_page_type
    CHECK meta_title_exists
    CHECK meta_description_exists
    CHECK word_count_matches_page_type
    CHECK one_service_only
    CHECK one_city_only_if_applicable
    CHECK schema_matches_page_type
    CHECK required_internal_links_exist
    CHECK nap_consistency
    CHECK no_false_location_claim
    CHECK no_canibalization
    CHECK cta_exists

    IF all_checks_pass:
        page.qa_status = "Approved"
    ELSE:
        page.qa_status = "Needs Revision"


## Output final del sistema


Debe generar 5 outputs:

1. URL Matrix
2. Internal Linking Matrix
3. Schema Map
4. Publishing Plan
5. QA Matrix


## Pseudocódigo completo en bloque único


START GMB_CRUSH_WEBSITE_BUILD_SYSTEM

INPUT:
    business_name
    website_root_domain
    canonical_domain
    primary_gbp_category
    primary_category_slug
    main_city
    physical_location_city
    target_cities[]
    core_services[]
    additional_gbp_categories[]
    phone
    email
    nap
    gbp_url
    geoarticles_per_service_city

NORMALIZE:
    Generate city_slugs[]
    Generate service_slugs[]
    Generate additional_category_slugs[]

VALIDATE:
    Confirm primary GBP category
    Confirm services support category
    Confirm cities are valid service areas
    Detect additional categories already covered by core services

GENERATE:
    Homepage
    Service Overview Pages for each core service
    GeoHub Pages for each target city
    Location-Based Service Pages for each service x city
    Additional Category Pages for each effective additional category x city
    GeoArticle ideas for each service x city x article count

ASSIGN:
    URL pattern by page type
    H1 by page type
    Meta title by page type
    Meta description by page type
    Schema by page type
    Internal links by page type
    Breadcrumb path by page type

SCORE:
    Calculate Revenue Value
    Calculate Search Intent
    Calculate GBP Category Relevance
    Calculate City Priority
    Calculate Competition Gap
    Calculate Conversion Urgency
    Generate Total Priority Score
    Assign P1 / P2 / P3 / P4 / Hold

PHASE:
    Assign Phase 1 Entity Foundation
    Assign Phase 2 Local Conversion Layer
    Assign Phase 3 Semantic Expansion Layer
    Assign Phase 4 Optimization Loop

CHECK DEPENDENCIES:
    Service pages require Homepage
    City-service pages require Service Overview + GeoHub
    GeoArticles require Location-Based Service Page + GeoHub
    Additional Category pages require GeoHub + related services

QA:
    Validate URL
    Validate page type
    Validate one service
    Validate one city
    Validate H1
    Validate metadata
    Validate schema
    Validate internal links
    Validate NAP
    Validate no false location claim
    Validate no canibalization
    Validate CTA

OUTPUT:
    URL Matrix
    Internal Linking Matrix
    Schema Map
    Publishing Plan
    QA Matrix

END


## Decisión final del Paso 10


A partir de este punto, el sistema ya no depende de memoria ni improvisación.

Para cualquier negocio local, el proceso será:

1. Rellenar inputs
2. Normalizar slugs
3. Generar arquitectura
4. Crear URLs
5. Asignar page type
6. Asignar schema
7. Asignar enlaces internos
8. Calcular prioridad
9. Asignar fase
10. Pasar QA
11. Publicar
12. Optimizar con tracking