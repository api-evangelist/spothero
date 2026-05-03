# SpotHero

SpotHero is the leading digital parking marketplace in North America, offering a flexible parking API and developer toolkit that connects vehicles, drivers, and mobility apps with the largest network of off-street parking facilities. The platform enables navigation apps, rideshare services, connected cars, and enterprise fleets to seamlessly book and manage parking reservations. SpotHero was acquired by Uber in 2026 to power parking reservation experiences within the Uber app.

- **Website:** https://spothero.com
- **Developer Portal:** https://spothero.com/developers
- **API Documentation:** https://api.spothero.com/v2/docs
- **Contact:** partner.support@spothero.com

## APIs

### SpotHero Parking API

The SpotHero Parking API provides programmatic access to the largest network of off-street parking facilities in North America. Partners can search for available parking spots, check real-time availability, create and manage reservations, and access facility details including pricing, amenities, and directions.

- **Base URL:** https://api.spothero.com/v2
- **Authentication:** API Key (X-API-Key header)
- **Documentation:** https://spothero.com/developers

**Key Capabilities:**
- Search parking by location, coordinates, or address
- Real-time availability across 8,000+ facilities in 400+ cities
- Create and cancel reservations with barcode access credentials
- Facility details including amenities, hours, and pricing
- White-label integration with partner branding support

**Use Cases:**
- Urban mobility and navigation app integration
- Connected car dashboard parking search
- Event venue parking pre-booking
- Enterprise fleet parking management
- Carshare and rental fleet parking coordination

### SpotHero SpotNow API

SpotNow is SpotHero's real-time parking server and API built in Kotlin, enabling instant parking availability and on-demand bookings via the HeroLab platform.

- **Repository:** https://github.com/spothero/herolab-spotnow

## Artifacts

### OpenAPI Specifications

| Spec | Description |
|---|---|
| [spothero-parking-openapi.yml](openapi/spothero-parking-openapi.yml) | SpotHero Parking API v2 — search, facilities, availability, rates, and reservations |

### JSON Schema

| Schema | Description |
|---|---|
| [spothero-reservation-schema.json](json-schema/spothero-reservation-schema.json) | Reservation object schema with driver, vehicle, barcode, and price fields |
| [spothero-facility-schema.json](json-schema/spothero-facility-schema.json) | Parking facility schema with address, coordinates, hours, and amenities |

### JSON Structure

| Structure | Description |
|---|---|
| [spothero-reservation-structure.json](json-structure/spothero-reservation-structure.json) | Hierarchical field map for the Reservation object |
| [spothero-facility-structure.json](json-structure/spothero-facility-structure.json) | Hierarchical field map for the Facility object |

### JSON-LD Context

| Context | Description |
|---|---|
| [spothero-context.jsonld](json-ld/spothero-context.jsonld) | Linked data context mapping SpotHero vocabulary to schema.org |

### Examples

| Example | Description |
|---|---|
| [spothero-search-parking-example.json](examples/spothero-search-parking-example.json) | Search parking near a location with request and response |
| [spothero-create-reservation-example.json](examples/spothero-create-reservation-example.json) | Create a parking reservation with full request/response |

### Spectral Rules

| Ruleset | Description |
|---|---|
| [spothero-rules.yml](rules/spothero-rules.yml) | Spectral ruleset enforcing SpotHero API conventions |

### Capabilities

| Capability | Description |
|---|---|
| [parking-mobility.yaml](capabilities/parking-mobility.yaml) | Full parking lifecycle: search, book, manage reservations (8 MCP tools) |
| [shared/spothero-parking.yaml](capabilities/shared/spothero-parking.yaml) | Shared SpotHero Parking API definition |

### Vocabulary

| Vocabulary | Description |
|---|---|
| [spothero-vocabulary.yml](vocabulary/spothero-vocabulary.yml) | Domain vocabulary covering parking, reservations, facilities, and mobility |

## Integration Options

SpotHero offers three integration levels for partners:

1. **Parking API** — Full programmatic control for custom implementations
2. **Web Widget** — Copy-and-paste embed for website integration (700+ partners)
3. **Parking Link** — Deep-link routing to SpotHero for minimal development

## Network Scale

- 100M+ parking reservations facilitated
- 400+ cities across North America
- 8,000+ parking locations in network
- Integrated with Apple Maps, Uber, and 700+ partners

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
