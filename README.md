# Nominatim (nominatim)

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

Nominatim is an open-source (BSD-2-Clause) search engine for OpenStreetMap data, supporting forward geocoding (address to coordinates), reverse geocoding (coordinates to address), and address lookup by OSM ID. The OpenStreetMap Foundation runs a free public instance at nominatim.openstreetmap.org under a published usage policy, and the project is also widely self-hosted and resold by commercial providers (MapTiler, LocationIQ, Geocode Earth).

**APIs.json:** [https://nominatim.org/](https://nominatim.org/)

## Tags

- Geocoding
- OpenStreetMap
- Maps
- LocationServices
- OpenSource
- Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Nominatim API

HTTP API surface implemented by Nominatim. The same surface is exposed by the OSMF public instance, self-hosted Nominatim deployments, and most commercial Nominatim-compatible providers.

- **Human URL:** [https://nominatim.org/release-docs/develop/api/Overview/](https://nominatim.org/release-docs/develop/api/Overview/)
- **Base URL:** `https://nominatim.openstreetmap.org`

#### Tags

- Geocoding
- Search
- Reverse
- Lookup

#### Properties

- [Documentation](https://nominatim.org/release-docs/develop/api/Overview/)
- [API Reference](https://nominatim.org/release-docs/develop/api/Search/)
- [OpenAPI](openapi/nominatim-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/nominatim.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nominatim.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/nominatim-place-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/nominatim-address-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/nominatim-place-details-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/nominatim-status-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/nominatim-place-structure.json)
- [JSON Structure](json-structure/nominatim-address-structure.json)
- [JSON Structure](json-structure/nominatim-status-structure.json)
- [JSON-LD](json-ld/nominatim-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/nominatim-search-example.json)
- [Example](examples/nominatim-reverse-example.json)
- [Example](examples/nominatim-lookup-example.json)
- [Example](examples/nominatim-details-example.json)
- [Example](examples/nominatim-status-example.json)
- [Example](examples/nominatim-place-example.json)
- [Example](examples/nominatim-address-example.json)
- [Rate Limits](rate-limits/nominatim-rate-limits.yml)
- [Plans](plans/nominatim-plans-pricing.yml)
- [SDK](https://pypi.org/project/nominatim-api/)
- [SDK](https://pypi.org/project/geopy/)

## Common Properties

- [Website](https://nominatim.org/)
- [Documentation](https://nominatim.org/release-docs/develop/)
- [GitHub Organization](https://github.com/osm-search)
- [GitHub Repository](https://github.com/osm-search/Nominatim)
- [GitHub Repository](https://github.com/osm-search/nominatim-ui)
- [GitHub Repository](https://github.com/osm-search/Nominatim-Data-Analyser)
- [GitHub Repository](https://github.com/osm-search/wikipedia-wikidata)
- [GitHub Repository](https://github.com/osm-search/TIGER-data)
- [GitHub Repository](https://github.com/osm-search/gb-postcode-data)
- [GitHub Repository](https://github.com/osm-search/country-grid-data)
- [GitHub Repository](https://github.com/osm-search/secondary-importance)
- [Terms of Service](https://operations.osmfoundation.org/policies/nominatim/)
- [Rate Limits](rate-limits/nominatim-rate-limits.yml)
- [Plans](plans/nominatim-plans-pricing.yml)
- [Vocabulary](vocabulary/nominatim-vocabulary.yml)
- [Spectral Rules](rules/nominatim-rules.yml)
- [Tools](https://github.com/NERVsystems/osmmcp)
- [Tools](https://github.com/geocoding-ai/mcp)
- [Tools](https://github.com/X-McKay/geocode-mcp)
- [Tools](https://github.com/jagan-shanmugam/open-streetmap-mcp)
- [Tools](https://github.com/sparkfabrik/nominatim-openapi)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
