# Nominatim (nominatim)

Nominatim is an open-source (BSD-2-Clause) search engine for OpenStreetMap data, supporting forward geocoding (address to coordinates), reverse geocoding (coordinates to address), and address lookup by OSM ID. The OpenStreetMap Foundation runs a free public instance at nominatim.openstreetmap.org under a published usage policy, and the project is also widely self-hosted and resold by commercial providers (MapTiler, LocationIQ, Geocode Earth).

**URL:** [Visit APIs.json URL](https://nominatim.org/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Type

- **x-type:** opensource
- **x-license:** BSD-2-Clause
- **x-governance:** OpenStreetMap Foundation (operations)
- **x-tier:** 3 (bulk-registered from public-apis)

## Tags:

 - Geocoding, OpenStreetMap, Maps, LocationServices, OpenSource, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Nominatim API

HTTP API surface implemented by Nominatim. The same surface is exposed by the OSMF public instance, self-hosted Nominatim deployments, and most commercial Nominatim-compatible providers.

**Human URL:** [https://nominatim.org/release-docs/develop/api/Overview/](https://nominatim.org/release-docs/develop/api/Overview/)

**Base URL:** `https://nominatim.openstreetmap.org`

#### Tags:

 - Geocoding, Search, Reverse, Lookup

#### Properties

- [Documentation](https://nominatim.org/release-docs/develop/api/Overview/)
- [APIReference](https://nominatim.org/release-docs/develop/api/Search/)
- [OpenAPI](openapi/nominatim-openapi.yml)
- [JSONSchema — Place](json-schema/nominatim-place-schema.json)
- [JSONSchema — Address](json-schema/nominatim-address-schema.json)
- [JSONSchema — PlaceDetails](json-schema/nominatim-place-details-schema.json)
- [JSONSchema — Status](json-schema/nominatim-status-schema.json)
- [JSONStructure — Place](json-structure/nominatim-place-structure.json)
- [JSONStructure — Address](json-structure/nominatim-address-structure.json)
- [JSONStructure — Status](json-structure/nominatim-status-structure.json)
- [JSONLD Context](json-ld/nominatim-context.jsonld)
- [Example — Search](examples/nominatim-search-example.json)
- [Example — Reverse](examples/nominatim-reverse-example.json)
- [Example — Lookup](examples/nominatim-lookup-example.json)
- [Example — Details](examples/nominatim-details-example.json)
- [Example — Status](examples/nominatim-status-example.json)
- [Example — Place JSON-LD](examples/nominatim-place-example.json)
- [Example — Address JSON-LD](examples/nominatim-address-example.json)
- [RateLimits](rate-limits/nominatim-rate-limits.yml)
- [Plans](plans/nominatim-plans-pricing.yml)
- [SDK — Nominatim Python API](https://pypi.org/project/nominatim-api/)
- [SDK — geopy](https://pypi.org/project/geopy/)

## Common Properties

- [Website](https://nominatim.org/)
- [Documentation](https://nominatim.org/release-docs/develop/)
- [GitHubOrganization](https://github.com/osm-search)
- [GitHubRepository — Nominatim core](https://github.com/osm-search/Nominatim)
- [GitHubRepository — Nominatim UI](https://github.com/osm-search/nominatim-ui)
- [GitHubRepository — Data Analyser](https://github.com/osm-search/Nominatim-Data-Analyser)
- [GitHubRepository — Wikipedia/Wikidata](https://github.com/osm-search/wikipedia-wikidata)
- [GitHubRepository — TIGER data](https://github.com/osm-search/TIGER-data)
- [GitHubRepository — GB postcode data](https://github.com/osm-search/gb-postcode-data)
- [GitHubRepository — Country grid data](https://github.com/osm-search/country-grid-data)
- [GitHubRepository — Secondary importance](https://github.com/osm-search/secondary-importance)
- [TermsOfService — Nominatim Usage Policy](https://operations.osmfoundation.org/policies/nominatim/)
- [RateLimits](rate-limits/nominatim-rate-limits.yml)
- [Plans](plans/nominatim-plans-pricing.yml)
- [Vocabulary](vocabulary/nominatim-vocabulary.yml)
- [SpectralRules](rules/nominatim-rules.yml)
- [Tools — osmmcp (Nominatim + Overpass + OSRM MCP)](https://github.com/NERVsystems/osmmcp)
- [Tools — geocoding-ai/mcp (Node.js)](https://github.com/geocoding-ai/mcp)
- [Tools — geocode-mcp (Python)](https://github.com/X-McKay/geocode-mcp)
- [Tools — open-streetmap-mcp](https://github.com/jagan-shanmugam/open-streetmap-mcp)
- [Tools — Unofficial Nominatim OpenAPI](https://github.com/sparkfabrik/nominatim-openapi)

## Features

| Name | Description |
|------|-------------|
| Forward Geocoding | Convert free-form or structured addresses into coordinates and full place metadata. |
| Reverse Geocoding | Identify the closest OSM feature to a coordinate at a chosen administrative zoom level. |
| OSM Object Lookup | Resolve up to 50 OSM nodes/ways/relations to detailed address breakdowns per call. |
| Multi-Format Output | Returns json, jsonv2, geojson, geocodejson, and xml from a single endpoint via `format`. |
| Polygon Geometry | Optional geometry output as GeoJSON, KML, SVG, or WKT with a simplification tolerance. |
| Country And Layer Filtering | Bias or restrict results by ISO country code, viewbox, layer (address/poi/etc.), or feature type. |
| Service Health | /status endpoint exposes data freshness, software version, and database version for monitoring. |
| Self-Hostable | Install on your own infrastructure from a planet.osm.pbf import; BSD-2-Clause licensed. |

## Use Cases

| Name | Description |
|------|-------------|
| Map Search Box | Power "find a place" search boxes in OSM-based map applications. |
| Reverse Geocoding For Telemetry | Attach human-readable addresses to coordinates collected from devices, vehicles, or sensors. |
| Civic Tech And Open Data | Provide geocoding for public-interest tools where commercial pricing is a barrier. |
| Background Address Normalisation | When self-hosted, normalize address strings in pipelines without per-call costs. |
| AI Agents With Map Tools | Ground LLM agents in real-world places via an MCP server backed by Nominatim. |

## Integrations

| Name | Description |
|------|-------------|
| geopy | Python geocoding library shipping a built-in Nominatim adapter. |
| GeoDjango | Django GIS framework with Nominatim geocoder support. |
| Leaflet Control Geocoder | Leaflet plugin offering a Nominatim geocoder out of the box. |
| OpenLayers | Web mapping library frequently paired with Nominatim for search. |
| QGIS MMQGIS | Desktop GIS plugin that batch-geocodes via Nominatim. |
| MapTiler Cloud Geocoding | Commercial hosted Nominatim-style API from MapTiler. |
| LocationIQ | Commercial Nominatim-compatible geocoding/routing platform. |
| Geocode Earth | Commercial Pelias deployment (Nominatim-compatible workloads). |

## Solutions

| Name | Description |
|------|-------------|
| OSMF Public Instance | Free hosted Nominatim under the OSMF Usage Policy (1 req/sec ceiling). |
| Self-Hosted Nominatim | BSD-2-Clause stack you import a planet dump into; no upstream rate limits. |
| Commercial Hosted Nominatim | Paid hosted offerings from MapTiler, LocationIQ, Geocode Earth and others. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Nominatim API](openapi/nominatim-openapi.yml) — 7 operations (search, reverse, lookup, details, status, deletable, polygons)

### JSON Schema

- [Place](json-schema/nominatim-place-schema.json)
- [Address](json-schema/nominatim-address-schema.json)
- [PlaceDetails](json-schema/nominatim-place-details-schema.json)
- [Status](json-schema/nominatim-status-schema.json)

### JSON Structure

- [Place](json-structure/nominatim-place-structure.json)
- [Address](json-structure/nominatim-address-structure.json)
- [Status](json-structure/nominatim-status-structure.json)

### JSON-LD

- [Nominatim Context](json-ld/nominatim-context.jsonld)

### Examples

- [Search](examples/nominatim-search-example.json)
- [Reverse](examples/nominatim-reverse-example.json)
- [Lookup](examples/nominatim-lookup-example.json)
- [Details](examples/nominatim-details-example.json)
- [Status](examples/nominatim-status-example.json)
- [Place (JSON-LD)](examples/nominatim-place-example.json)
- [Address (JSON-LD)](examples/nominatim-address-example.json)

### Plans

- [Nominatim Plans And Pricing](plans/nominatim-plans-pricing.yml) — Free public OSMF instance, self-hosted FOSS, and commercial hosted alternatives.

### Rate Limits

- [Nominatim Rate Limits](rate-limits/nominatim-rate-limits.yml) — OSMF public-instance ceiling: 1 request/second across all callers, User-Agent and attribution required.

## Capabilities

Naftiko capabilities for Nominatim workflows.

| Workflow | APIs Combined | Persona |
|----------|--------------|---------|
| [Forward And Reverse Geocoding](capabilities/geocoding.yaml) | Nominatim /search + /reverse | Map application backend |
| [OSM Object Address Lookup](capabilities/address-lookup.yaml) | Nominatim /lookup | Data enrichment pipeline |
| [Nominatim Service Health Check](capabilities/service-health.yaml) | Nominatim /status | Self-hosted operator |

## Vocabulary

- [Nominatim Vocabulary](vocabulary/nominatim-vocabulary.yml) — 9 concepts, 3 OSM object types, 5 output formats, 5 feature layers, 4 policy terms, 3 deployment modes.

## Rules

- [Nominatim Spectral Rules](rules/nominatim-rules.yml) — 10 rules enforcing summaries, operationIds, tags, format enums, license, terms-of-service, and rate-limit documentation.

## Notes

This entry was bulk-registered as part of a public-apis catalog sweep on 2026-05-28 and enriched on 2026-05-29 via the full opensource pipeline.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
