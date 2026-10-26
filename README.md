# FarmLogs (farmlogs)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
