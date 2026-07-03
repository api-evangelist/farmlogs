# FarmLogs (farmlogs)

FarmLogs was a farm management platform founded in 2011 (by Jesse Vollmar and Brad Koch, operating as AgriSight Inc.) offering field mapping, in-season satellite imagery, weather/rainfall tracking, yield estimation, and profitability tools for row-crop farmers. FarmLogs was acquired by Bushel in June 2021, and in March 2023 Bushel retired the FarmLogs brand in favor of "Bushel Farm," the next generation of its farm management software. As of this review, farmlogs.com 301-redirects to bushelfarm.com, which itself redirects to bushelpowered.com - the standalone FarmLogs product and website no longer exist. Bushel does publish a public API, but it is for a separate product line (Bushel Fulfillment and Bushel Production, covering grain contracts and scale-ticket data for grain merchandising) rather than for the FarmLogs-lineage farm-management capabilities (fields, imagery, weather, yield). No self-serve, openly documented public API exists for the farm-management product as of the review date.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/farmlogs/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/farmlogs/refs/heads/main/apis.yml)

## Operating Status

**Discontinued as a standalone brand.** FarmLogs was **acquired by Bushel** on 2021-06-15. Bushel operated FarmLogs as a distinct brand for about two years, then on 2023-03-02 announced **"Bushel Farm"** as the next generation of farm management software, replacing FarmLogs. `farmlogs.com` now redirects to `bushelfarm.com`, which redirects to `bushelpowered.com/farmers`. The product lineage (field mapping, satellite imagery, weather, yield, profitability) lives on under the Bushel Farm brand and the `app.bushelfarm.com` application, but there is no surviving FarmLogs-branded product, website, or API to review independently.

## API Availability

**No self-serve, openly documented public API exists** for FarmLogs or its Bushel Farm successor. Bushel operates a public API documentation site (`bushelfulfillment.bushelops.com`) for **Bushel Fulfillment** and **Bushel Production**, but that covers a separate product line — grain contracts and scale-ticket data sharing for grain merchandising — authenticated with a static shared key against endpoints under `centre.scaleticket.net`. It does not surface field mapping, satellite imagery, weather, or yield endpoints, and is not related to the FarmLogs lineage. Bushel's farm-management marketing page mentions farmers can share crop production records "into your ERP or database using an API connection," but publishes no base URL, authentication scheme, or endpoint reference for that connection. This catalog documents FarmLogs' historical product surfaces honestly; the OpenAPI artifact intentionally carries an empty `paths: {}` because no public endpoints are documented, and no endpoints were fabricated.

## Tags

- Agriculture
- Farm Management
- Precision Agriculture
- Satellite Imagery
- Acquired
- Discontinued Brand

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### FarmLogs Fields

Field boundary mapping and per-field record-keeping, the original core of FarmLogs. This capability now lives inside Bushel Farm; no self-serve public REST reference, base URL, or endpoint catalog has ever been published for it.

- **Human URL:** [https://bushelpowered.com/solutions/farm-management/](https://bushelpowered.com/solutions/farm-management/)

#### Tags

- Fields
- Mapping
- Boundaries

#### Properties

- [Documentation](https://bushelpowered.com/solutions/farm-management/)
- [OpenAPI](openapi/farmlogs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/farmlogs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/farmlogs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### FarmLogs Satellite Imagery / NDVI

In-season multispectral satellite imagery used to spot yield threats, stress, and management issues field-by-field. A marquee FarmLogs feature historically; no openly documented public imagery API endpoints were ever published, and the standalone FarmLogs product no longer exists.

- **Human URL:** [https://bushelpowered.com/solutions/farm-management/](https://bushelpowered.com/solutions/farm-management/)

#### Tags

- Satellite Imagery
- NDVI
- Crop Health

#### Properties

- [Documentation](https://bushelpowered.com/solutions/farm-management/)
- [OpenAPI](openapi/farmlogs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/farmlogs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/farmlogs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### FarmLogs Weather & Rainfall

Field-level rainfall and weather tracking with season-over-season comparisons. Bushel Farm continues to market a "Stop Checking Your Rain Gauges" rainfall feature descended from FarmLogs, but exposes it only inside the product, not through a documented public API.

- **Human URL:** [https://bushelpowered.com/farmers](https://bushelpowered.com/farmers)

#### Tags

- Weather
- Rainfall
- Field-Level

#### Properties

- [Documentation](https://bushelpowered.com/farmers)
- [OpenAPI](openapi/farmlogs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/farmlogs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/farmlogs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### FarmLogs Yield & Profitability

Yield tracking, cost-of-production, and field/crop/farm-level profit-and-loss calculations. Bushel Farm's marketing page notes production records can be shared "into your ERP or database using an API connection," but no self-serve developer reference, base URL, or authentication scheme is published.

- **Human URL:** [https://bushelpowered.com/solutions/farm-management/](https://bushelpowered.com/solutions/farm-management/)

#### Tags

- Yield
- Profitability
- Cost Of Production

#### Properties

- [Documentation](https://bushelpowered.com/solutions/farm-management/)
- [OpenAPI](openapi/farmlogs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/farmlogs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/farmlogs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### FarmLogs Activities & Scouting

Field activity logging and in-field scouting notes, plus machine/equipment activity ingested from John Deere Operations Center and Climate FieldView integrations. These are inbound partner integrations into Bushel Farm, not an outbound public API for third-party developers.

- **Human URL:** [https://bushelpowered.com/solutions/farm-management/](https://bushelpowered.com/solutions/farm-management/)

#### Tags

- Activities
- Scouting
- Field Notes

#### Properties

- [Documentation](https://bushelpowered.com/solutions/farm-management/)
- [OpenAPI](openapi/farmlogs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/farmlogs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/farmlogs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/farmlogs)
- [Website](https://www.farmlogs.com)
- [Documentation](https://bushelpowered.com/solutions/farm-management/)
- [Plans](plans/farmlogs-plans-pricing.yml)
- [Rate Limits](rate-limits/farmlogs-rate-limits.yml)
- [Fin Ops](finops/farmlogs-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
