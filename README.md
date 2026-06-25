# Monta (monta)

Monta is an EV-charging software platform that operates charge points, a consumer driver app, and back-office tools for installers, businesses, and charge point operators. The Monta Public API exposes charge points, charges (charging sessions), EVSE availability and pricing, and wallet transactions via a REST interface secured with OAuth2 client-credentials bearer tokens, plus signed webhooks for real-time platform events.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/monta/refs/heads/main/apis.yml)

## Tags

- EV Charging
- Electric Vehicles
- Charge Points
- Energy
- Mobility

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Monta Charge Points

List and read charge points (GET /charge-points, GET /charge-points/{id}), read AFIR-compliant roaming charge points, and read EVSE availability status and ad-hoc pricing. Requires the `charge-points` scope.

- **Human URL:** [https://docs.public-api.monta.com/reference/get-charge-points](https://docs.public-api.monta.com/reference/get-charge-points)
- **Base URL:** `https://public-api.monta.com/api/v1`

#### Tags

- Charge Points
- EVSE
- Roaming

#### Properties

- [Documentation](https://docs.public-api.monta.com/)
- [API Reference](https://docs.public-api.monta.com/reference/get-charge-points)
- [OpenAPI](openapi/monta-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/monta.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/monta.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Monta Charges and Sessions

List and read charges (charging sessions), start and stop charges on a charge point, and read per-charge kWh consumption. Reads require the `charge-transactions` scope; starting and stopping charges requires the `control-charging` scope.

- **Human URL:** [https://docs.public-api.monta.com/reference/start-charge](https://docs.public-api.monta.com/reference/start-charge)
- **Base URL:** `https://public-api.monta.com/api/v1`

#### Tags

- Charges
- Sessions
- Control Charging

#### Properties

- [Documentation](https://docs.public-api.monta.com/)
- [API Reference](https://docs.public-api.monta.com/reference/start-charge)
- [OpenAPI](openapi/monta-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/monta.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/monta.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Monta Teams

Team and operator account context for charge points, charges, and wallets on the Monta platform. Team-scoped resource management is exposed more fully through the Monta Partner API; the Public API surfaces team context implicitly via the authenticated application's access.

- **Human URL:** [https://docs.public-api.monta.com/](https://docs.public-api.monta.com/)
- **Base URL:** `https://public-api.monta.com/api/v1`

#### Tags

- Teams
- Accounts
- Operators

#### Properties

- [Documentation](https://docs.public-api.monta.com/)
- [OpenAPI](openapi/monta-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Monta Wallets and Transactions

List and read wallet transactions and read the personal wallet (GET /wallet-transactions, GET /wallet-transactions/{id}, GET /personal-wallet). Requires the `wallet-transactions` scope.

- **Human URL:** [https://docs.public-api.monta.com/reference/get-wallet-transactions](https://docs.public-api.monta.com/reference/get-wallet-transactions)
- **Base URL:** `https://public-api.monta.com/api/v1`

#### Tags

- Wallets
- Transactions
- Payments

#### Properties

- [Documentation](https://docs.public-api.monta.com/)
- [API Reference](https://docs.public-api.monta.com/reference/get-wallet-transactions)
- [OpenAPI](openapi/monta-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/monta.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/monta.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Monta Tariffs and Plans

Charge point pricing and tariffs. EVSE ad-hoc pricing is readable through the Public API EVSE status endpoint; full tariff and price-group management (price groups, availability schedules) is exposed through the Monta Partner API.

- **Human URL:** [https://docs.public-api.monta.com/](https://docs.public-api.monta.com/)
- **Base URL:** `https://public-api.monta.com/api/v1`

#### Tags

- Tariffs
- Pricing
- Price Groups

#### Properties

- [Documentation](https://docs.public-api.monta.com/)
- [Website](https://monta.com/en/features/public-api/)
- [OpenAPI](openapi/monta-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Monta Webhooks

Signed webhook payloads deliver real-time platform events without polling, covering charge transactions, OCPP messages, sites, teams, wallet transactions, and more. Webhook subscription configuration is managed through the Monta Partner API.

- **Human URL:** [https://docs.public-api.monta.com/](https://docs.public-api.monta.com/)
- **Base URL:** `https://public-api.monta.com/api/v1`

#### Tags

- Webhooks
- Events
- Real Time

#### Properties

- [Documentation](https://docs.public-api.monta.com/)
- [Website](https://monta.com/en/features/public-api/)

## Common Properties

- [GitHub Organization](https://github.com/monta-app)
- [LinkedIn](https://www.linkedin.com/company/montaapp)
- [Website](https://www.monta.com)
- [Documentation](https://docs.public-api.monta.com/)
- [Plans](plans/monta-plans-pricing.yml)
- [Rate Limits](rate-limits/monta-rate-limits.yml)
- [Fin Ops](finops/monta-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
