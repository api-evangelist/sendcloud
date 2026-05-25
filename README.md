# Sendcloud (sendcloud)

Sendcloud is Europe's leading shipping platform for ecommerce, headquartered in Eindhoven, Netherlands. The platform connects 30,000+ merchants to 160+ carriers (DHL, DPD, UPS, GLS, FedEx, PostNL, bpost, La Poste, Royal Mail, Hermes and many more) and 100+ commerce / WMS / marketplace integrations across the UK, Netherlands, Belgium, France, Germany, Austria, Italy, and Spain.

**URL:** [Visit APIs.yml URL](https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Shipping, Logistics, Ecommerce, Carriers, Labels, Returns, Tracking, Europe

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

The Sendcloud platform exposes a versioned REST surface on `https://panel.sendcloud.sc` — `v3` is current, `v2` remains documented for legacy integrations. Auth is HTTP Basic (public key as username, private key as password) or OAuth 2.0 client credentials at `https://account.sendcloud.com/oauth2/token` (scope `api`).

### v3 APIs (current)

| API | Base | OpenAPI |
|---|---|---|
| Shipments | `/api/v3/shipments` | [openapi/sendcloud-shipments-openapi.yml](openapi/sendcloud-shipments-openapi.yml) |
| Orders | `/api/v3/orders` | [openapi/sendcloud-v3-orders-openapi.yml](openapi/sendcloud-v3-orders-openapi.yml) |
| Ship an Order | `/api/v3/ship-an-order` | [openapi/sendcloud-v3-ship-an-order-openapi.yml](openapi/sendcloud-v3-ship-an-order-openapi.yml) |
| Returns | `/api/v3/returns` | [openapi/sendcloud-v3-returns-openapi.yml](openapi/sendcloud-v3-returns-openapi.yml) |
| Service Points | `/api/v3/service-points` | [openapi/sendcloud-v3-service-points-openapi.yml](openapi/sendcloud-v3-service-points-openapi.yml) |
| Parcel Tracking | `/api/v3/parcels/tracking` | [openapi/sendcloud-v3-parcel-tracking-openapi.yml](openapi/sendcloud-v3-parcel-tracking-openapi.yml) |
| Parcel Documents | `/api/v3/parcel-documents` | [openapi/sendcloud-v3-parcel-documents-openapi.yml](openapi/sendcloud-v3-parcel-documents-openapi.yml) |
| Webhooks | `/api/v3/webhooks` | [openapi/sendcloud-v3-webhooks-openapi.yml](openapi/sendcloud-v3-webhooks-openapi.yml) |
| Event Subscriptions | `/api/v3/event-subscriptions` | [openapi/sendcloud-v3-event-subscriptions-openapi.yml](openapi/sendcloud-v3-event-subscriptions-openapi.yml) |
| Integrations | `/api/v3/integrations` | [openapi/sendcloud-v3-integrations-openapi.yml](openapi/sendcloud-v3-integrations-openapi.yml) |
| Analytics | `/api/v3/analytics` | [openapi/sendcloud-v3-analytics-openapi.yml](openapi/sendcloud-v3-analytics-openapi.yml) |
| Reporting | `/api/v3/reporting` | [openapi/sendcloud-v3-reporting-openapi.yml](openapi/sendcloud-v3-reporting-openapi.yml) |

### v2 APIs (legacy)

| API | Base | OpenAPI |
|---|---|---|
| Parcels | `/api/v2/parcels` | [openapi/sendcloud-v2-parcels-openapi.yml](openapi/sendcloud-v2-parcels-openapi.yml) |
| Labels | `/api/v2/labels` | [openapi/sendcloud-v2-labels-openapi.yml](openapi/sendcloud-v2-labels-openapi.yml) |
| Tracking | `/api/v2/tracking` | [openapi/sendcloud-v2-tracking-openapi.yml](openapi/sendcloud-v2-tracking-openapi.yml) |
| Webhooks | `/api/v2/webhooks` | [openapi/sendcloud-v2-webhooks-openapi.yml](openapi/sendcloud-v2-webhooks-openapi.yml) |
| Integrations | `/api/v2/integrations` | [openapi/sendcloud-v2-integrations-openapi.yml](openapi/sendcloud-v2-integrations-openapi.yml) |
| Parcel Documents | `/api/v2/parcel-documents` | [openapi/sendcloud-v2-parcel-documents-openapi.yml](openapi/sendcloud-v2-parcel-documents-openapi.yml) |
| Analytics | `/api/v2/analytics` | [openapi/sendcloud-v2-analytics-openapi.yml](openapi/sendcloud-v2-analytics-openapi.yml) |
| Reporting | `/api/v2/reporting` | [openapi/sendcloud-v2-reporting-openapi.yml](openapi/sendcloud-v2-reporting-openapi.yml) |

## Capabilities

| Capability | Description |
|---|---|
| [capabilities/european-shipping-fulfillment.yaml](capabilities/european-shipping-fulfillment.yaml) | End-to-end European fulfillment: orders -> service points -> announce -> tracking -> returns |
| [capabilities/sendcloud-shipments.yaml](capabilities/sendcloud-shipments.yaml) | Per-API capability for Sendcloud Shipments v3 |
| [capabilities/sendcloud-orders.yaml](capabilities/sendcloud-orders.yaml) | Per-API capability for Sendcloud Orders v3 |
| [capabilities/sendcloud-returns.yaml](capabilities/sendcloud-returns.yaml) | Per-API capability for Sendcloud Returns v3 |
| [capabilities/sendcloud-service-points.yaml](capabilities/sendcloud-service-points.yaml) | Per-API capability for Sendcloud Service Points v3 |
| [capabilities/sendcloud-parcel-tracking.yaml](capabilities/sendcloud-parcel-tracking.yaml) | Per-API capability for Sendcloud Parcel Tracking v3 |
| [capabilities/sendcloud-parcel-documents.yaml](capabilities/sendcloud-parcel-documents.yaml) | Per-API capability for Sendcloud Parcel Documents v3 |
| [capabilities/sendcloud-event-subscriptions.yaml](capabilities/sendcloud-event-subscriptions.yaml) | Per-API capability for Sendcloud Event Subscriptions v3 |

## Artifacts

| Type | File |
|---|---|
| OpenAPI | 20 specs under [openapi/](openapi/) (12 v3, 8 v2) |
| JSON Schema | 9 schemas under [json-schema/](json-schema/) |
| JSON Structure | [json-structure/sendcloud-shipment-structure.json](json-structure/sendcloud-shipment-structure.json), [json-structure/sendcloud-return-structure.json](json-structure/sendcloud-return-structure.json) |
| JSON-LD | [json-ld/sendcloud-context.jsonld](json-ld/sendcloud-context.jsonld) |
| Examples | [examples/sendcloud-announce-shipment-example.json](examples/sendcloud-announce-shipment-example.json), [examples/sendcloud-create-return-example.json](examples/sendcloud-create-return-example.json), [examples/sendcloud-list-service-points-example.json](examples/sendcloud-list-service-points-example.json) |
| Spectral Rules | [rules/sendcloud-rules.yml](rules/sendcloud-rules.yml) |
| Vocabulary | [vocabulary/sendcloud-vocabulary.yml](vocabulary/sendcloud-vocabulary.yml) |
| Plans | [plans/sendcloud-plans-pricing.yml](plans/sendcloud-plans-pricing.yml) |
| Rate Limits | [rate-limits/sendcloud-rate-limits.yml](rate-limits/sendcloud-rate-limits.yml) |
| FinOps | [finops/sendcloud-finops.yml](finops/sendcloud-finops.yml) |

## Common Properties

- [Website](https://www.sendcloud.com)
- [Developer Portal](https://sendcloud.dev)
- [Documentation](https://sendcloud.dev/docs/getting-started/)
- [API Reference (v3)](https://sendcloud.dev/api/v3/)
- [Getting Started](https://sendcloud.dev/docs/getting-started/)
- [Authentication](https://sendcloud.dev/docs/getting-started/authentication/)
- [Rate Limits](https://sendcloud.dev/docs/getting-started/rate-limits/)
- [Pagination](https://sendcloud.dev/api/v3/pagination/)
- [API Version Guide](https://sendcloud.dev/docs/getting-started/api-version-guide/)
- [Migration Guide v2 -> v3](https://sendcloud.dev/docs/getting-started/migration-guidelines-for-api-v3/)
- [v3 Changelog](https://sendcloud.dev/api/v3/changelog/) | [v2 Changelog](https://sendcloud.dev/api/v2/changelog/)
- [Postman](https://sendcloud.dev/docs/getting-started/postman/)
- [Pricing](https://www.sendcloud.com/pricing/)
- [Blog](https://www.sendcloud.com/blog/)
- [Support](https://support.sendcloud.com/)
- [Release Log](https://releaselog.sendcloud.com/)
- [GitHub Organization](https://github.com/Sendcloud)
- [LinkedIn](https://www.linkedin.com/company/sendcloud/)
- [llms.txt](https://sendcloud.dev/llms.txt)

## Pricing (snapshot)

| Plan | Monthly | Labels included | Extra label |
|---|---|---|---|
| Free | EUR 0 | 50 (unstamped letter) | n/a |
| Lite | EUR 33 | 400 | EUR 0.11 |
| Growth | EUR 99 | 1,000 | EUR 0.10 |
| Premium | EUR 195 | 10,000 | EUR 0.09 |
| Pro | EUR 799 | 30,000 | EUR 0.07 |
| Enterprise | Custom | Custom | Custom |

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
