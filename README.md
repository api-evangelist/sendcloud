# Sendcloud (sendcloud)

Sendcloud is Europe's leading shipping platform for e-commerce, headquartered in Eindhoven, Netherlands. The platform connects 30,000+ merchants to 160+ carriers (DHL, DPD, UPS, GLS, FedEx, PostNL, bpost, La Poste, Royal Mail, Hermes, and many more) and 100+ commerce / WMS / marketplace integrations across the UK, Netherlands, Belgium, France, Germany, Austria, Italy, and Spain. The Sendcloud APIs cover the full fulfillment lifecycle — Orders, Ship an Order, Shipments, Service Points, Parcel Tracking, Parcel Documents, Returns, Event Subscriptions, Webhooks, Integrations, Analytics, and Reporting — over a versioned v2 / v3 REST surface on https://panel.sendcloud.sc, authenticated with HTTP Basic (public + private key) or OAuth 2.0 client credentials.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sendcloud/refs/heads/main/apis.yml)

## Scope

- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Shipping
- Logistics
- Ecommerce
- Carriers
- Labels
- Returns
- Tracking
- Europe

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Sendcloud Shipments API v3

Create, announce, retrieve, and cancel outgoing shipments and their associated parcels on the Sendcloud platform. Supports synchronous and asynchronous announcement, shipping-rules-driven defaults, address validation, multicollo multi-parcel shipments, and return-portal generation across 160+ European carriers.

- **Human URL:** [https://sendcloud.dev/api/v3/shipments/](https://sendcloud.dev/api/v3/shipments/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Shipping
- Labels
- Logistics
- Carriers

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/shipments/)
- [OpenAPI](https://sendcloud.dev/.openapi/v3/shipments/openapi.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/sendcloud-shipments-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-shipments.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-shipments.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [API Reference](https://sendcloud.dev/api/v3/shipments/create-and-announce-a-shipment-synchronously)
- [JSON Structure](json-structure/sendcloud-shipment-structure.json)
- [Example](examples/sendcloud-announce-shipment-example.json)

### Sendcloud Orders API v3

Manage orders pulled in from connected commerce platforms and marketplaces. List, retrieve, update, and delete orders before converting them into shipments via the Ship an Order flow.

- **Human URL:** [https://sendcloud.dev/api/v3/orders/](https://sendcloud.dev/api/v3/orders/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Orders
- Ecommerce

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/orders/)
- [OpenAPI](openapi/sendcloud-v3-orders-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-orders.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-orders.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/sendcloud-order-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Sendcloud Ship an Order API v3

Composite v3 flow that turns an existing order into a shipment, requests a label, and returns a usable parcel in one call.

- **Human URL:** [https://sendcloud.dev/api/v3/ship-an-order/](https://sendcloud.dev/api/v3/ship-an-order/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Orders
- Shipping
- Fulfillment

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/ship-an-order/)
- [OpenAPI](openapi/sendcloud-v3-ship-an-order-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-ship-an-order.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-ship-an-order.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Returns API v3

Create, validate, list, announce, and cancel return shipments. Supports drop-off at service point, in-store, home pickup, and postbox delivery options across European carriers.

- **Human URL:** [https://sendcloud.dev/api/v3/returns/](https://sendcloud.dev/api/v3/returns/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Returns
- Reverse Logistics

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/returns/)
- [OpenAPI](openapi/sendcloud-v3-returns-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-returns.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-returns.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/sendcloud-return-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sendcloud-deliveryoption-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/sendcloud-return-structure.json)
- [Example](examples/sendcloud-create-return-example.json)

### Sendcloud Service Points API v3

Look up parcel-shop, locker, and post-office drop-off / pickup locations across 160+ European carriers, filter by country, postcode, carrier, and radius, and check service-point availability.

- **Human URL:** [https://sendcloud.dev/api/v3/service-points/](https://sendcloud.dev/api/v3/service-points/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Service Points
- Carriers
- Last Mile

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/service-points/)
- [OpenAPI](openapi/sendcloud-v3-service-points-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-service-points.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-service-points.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/sendcloud-servicepoint-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sendcloud-servicepointdetail-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sendcloud-servicepointaddress-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/sendcloud-list-service-points-example.json)

### Sendcloud Parcel Tracking API v3

Retrieve normalised tracking information for a parcel by tracking number and register external parcels for Sendcloud's branded tracking experience and webhook notifications.

- **Human URL:** [https://sendcloud.dev/api/v3/parcel-tracking/](https://sendcloud.dev/api/v3/parcel-tracking/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Tracking
- Last Mile

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/parcel-tracking/)
- [OpenAPI](openapi/sendcloud-v3-parcel-tracking-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-parcel-tracking.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-parcel-tracking.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/sendcloud-parceltrackingresponse-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sendcloud-parceltrackingcreaterequest-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Sendcloud Parcel Documents API v3

Retrieve shipping labels, customs declarations (CN22 / CN23), commercial invoices, and QR codes for individual parcels or in batch.

- **Human URL:** [https://sendcloud.dev/api/v3/parcel-documents/](https://sendcloud.dev/api/v3/parcel-documents/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Labels
- Customs
- Documents

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/parcel-documents/)
- [OpenAPI](openapi/sendcloud-v3-parcel-documents-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-parcel-documents.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-parcel-documents.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Webhooks API v3

Outbound webhook delivery surface — parcel-status-changed, return-created and other typed events sent to merchant-configured HTTPS endpoints.

- **Human URL:** [https://sendcloud.dev/api/v3/webhooks/](https://sendcloud.dev/api/v3/webhooks/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Webhooks
- Events

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/webhooks/)
- [OpenAPI](openapi/sendcloud-v3-webhooks-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-webhooks.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-webhooks.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Event Subscriptions API v3

Manage typed event subscriptions and webhook delivery connections — register endpoints, list subscriptions, and broadcast test events.

- **Human URL:** [https://sendcloud.dev/api/v3/event-subscriptions/](https://sendcloud.dev/api/v3/event-subscriptions/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Webhooks
- Events
- Subscriptions

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/event-subscriptions/)
- [OpenAPI](openapi/sendcloud-v3-event-subscriptions-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-event-subscriptions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-event-subscriptions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Integrations API v3

Manage connectors between Sendcloud and external commerce / WMS / marketplace platforms (Shopify, WooCommerce, Magento, Amazon, Etsy, etc.).

- **Human URL:** [https://sendcloud.dev/api/v3/integrations/](https://sendcloud.dev/api/v3/integrations/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Integrations
- Marketplaces

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/integrations/)
- [OpenAPI](openapi/sendcloud-v3-integrations-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-integrations.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-integrations.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Analytics API v3

Aggregated shipping spend, carrier mix, service-level performance, and return-rate analytics.

- **Human URL:** [https://sendcloud.dev/api/v3/analytics/](https://sendcloud.dev/api/v3/analytics/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Analytics
- Reporting

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/analytics/)
- [OpenAPI](openapi/sendcloud-v3-analytics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-analytics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-analytics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Reporting API v3

Per-shipment cost reports and billing line items for back-office reconciliation.

- **Human URL:** [https://sendcloud.dev/api/v3/reporting/](https://sendcloud.dev/api/v3/reporting/)
- **Base URL:** `https://panel.sendcloud.sc/api/v3`

#### Tags

- Reporting
- Billing

#### Properties

- [Documentation](https://sendcloud.dev/api/v3/reporting/)
- [OpenAPI](openapi/sendcloud-v3-reporting-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v3-reporting.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v3-reporting.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Parcels API v2

Legacy v2 Parcels surface for announcing shipments and retrieving parcel state. Superseded by the v3 Shipments API; documented for migration paths.

- **Human URL:** [https://sendcloud.dev/api/v2/parcels/](https://sendcloud.dev/api/v2/parcels/)
- **Base URL:** `https://panel.sendcloud.sc/api/v2`

#### Tags

- Parcels
- Legacy
- Shipping

#### Properties

- [Documentation](https://sendcloud.dev/api/v2/parcels/)
- [OpenAPI](openapi/sendcloud-v2-parcels-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v2-parcels.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v2-parcels.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Labels API v2

Legacy v2 Labels surface for downloading the shipping label PDF / ZPL associated with a parcel. Superseded by the v3 Parcel Documents API.

- **Human URL:** [https://sendcloud.dev/api/v2/labels/](https://sendcloud.dev/api/v2/labels/)
- **Base URL:** `https://panel.sendcloud.sc/api/v2`

#### Tags

- Labels
- Legacy

#### Properties

- [Documentation](https://sendcloud.dev/api/v2/labels/)
- [OpenAPI](openapi/sendcloud-v2-labels-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v2-labels.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v2-labels.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Tracking API v2

Legacy v2 Tracking surface. Superseded by the v3 Parcel Tracking API.

- **Human URL:** [https://sendcloud.dev/api/v2/tracking/](https://sendcloud.dev/api/v2/tracking/)
- **Base URL:** `https://panel.sendcloud.sc/api/v2`

#### Tags

- Tracking
- Legacy

#### Properties

- [Documentation](https://sendcloud.dev/api/v2/tracking/)
- [OpenAPI](openapi/sendcloud-v2-tracking-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v2-tracking.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v2-tracking.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Webhooks API v2

Legacy v2 Webhooks surface. Superseded by the v3 Event Subscriptions API.

- **Human URL:** [https://sendcloud.dev/api/v2/webhooks/](https://sendcloud.dev/api/v2/webhooks/)
- **Base URL:** `https://panel.sendcloud.sc/api/v2`

#### Tags

- Webhooks
- Legacy

#### Properties

- [Documentation](https://sendcloud.dev/api/v2/webhooks/)
- [OpenAPI](openapi/sendcloud-v2-webhooks-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v2-webhooks.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v2-webhooks.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Integrations API v2

Legacy v2 Integrations surface managing connectors to commerce platforms.

- **Human URL:** [https://sendcloud.dev/api/v2/integrations/](https://sendcloud.dev/api/v2/integrations/)
- **Base URL:** `https://panel.sendcloud.sc/api/v2`

#### Tags

- Integrations
- Legacy

#### Properties

- [Documentation](https://sendcloud.dev/api/v2/integrations/)
- [OpenAPI](openapi/sendcloud-v2-integrations-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v2-integrations.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v2-integrations.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Analytics API v2

Legacy v2 Analytics surface exposing aggregated shipping metrics.

- **Human URL:** [https://sendcloud.dev/api/v2/analytics/](https://sendcloud.dev/api/v2/analytics/)
- **Base URL:** `https://panel.sendcloud.sc/api/v2`

#### Tags

- Analytics
- Legacy

#### Properties

- [Documentation](https://sendcloud.dev/api/v2/analytics/)
- [OpenAPI](openapi/sendcloud-v2-analytics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v2-analytics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v2-analytics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Reporting API v2

Legacy v2 Reporting surface for shipment-level billing line items.

- **Human URL:** [https://sendcloud.dev/api/v2/reporting/](https://sendcloud.dev/api/v2/reporting/)
- **Base URL:** `https://panel.sendcloud.sc/api/v2`

#### Tags

- Reporting
- Legacy

#### Properties

- [Documentation](https://sendcloud.dev/api/v2/reporting/)
- [OpenAPI](openapi/sendcloud-v2-reporting-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v2-reporting.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v2-reporting.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sendcloud Parcel Documents API v2

Legacy v2 Parcel Documents surface for retrieving labels and customs paperwork.

- **Human URL:** [https://sendcloud.dev/api/v2/parcel-documents/](https://sendcloud.dev/api/v2/parcel-documents/)
- **Base URL:** `https://panel.sendcloud.sc/api/v2`

#### Tags

- Documents
- Customs
- Legacy

#### Properties

- [Documentation](https://sendcloud.dev/api/v2/parcel-documents/)
- [OpenAPI](openapi/sendcloud-v2-parcel-documents-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sendcloud-v2-parcel-documents.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sendcloud-v2-parcel-documents.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Website](https://www.sendcloud.com)
- [Developer Portal](https://sendcloud.dev)
- [Documentation](https://sendcloud.dev/docs/getting-started/)
- [API Reference](https://sendcloud.dev/api/v3/)
- [Getting Started](https://sendcloud.dev/docs/getting-started/)
- [Quickstart](https://sendcloud.dev/docs/getting-started/)
- [Authentication](https://sendcloud.dev/docs/getting-started/authentication/)
- [Rate Limits](https://sendcloud.dev/docs/getting-started/rate-limits/)
- [Pagination](https://sendcloud.dev/api/v3/pagination/)
- [A P I Version Guide](https://sendcloud.dev/docs/getting-started/api-version-guide/)
- [Migration Guide](https://sendcloud.dev/docs/getting-started/migration-guidelines-for-api-v3/)
- [Changelog](https://sendcloud.dev/api/v3/changelog/)
- [Changelog](https://sendcloud.dev/api/v2/changelog/)
- [Glossary](https://sendcloud.dev/docs/getting-started/glossary/)
- [Postman](https://sendcloud.dev/docs/getting-started/postman/) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Pricing](https://www.sendcloud.com/pricing/)
- [Blog](https://www.sendcloud.com/blog/)
- [Support](https://support.sendcloud.com/)
- [Release Notes](https://releaselog.sendcloud.com/)
- [GitHub Organization](https://github.com/Sendcloud)
- [LinkedIn](https://www.linkedin.com/company/sendcloud/)
- [L L Ms Txt](https://sendcloud.dev/llms.txt)
- [Spectral Rules](rules/sendcloud-rules.yml)
- [Vocabulary](vocabulary/sendcloud-vocabulary.yml)
- [JSON-LD](json-ld/sendcloud-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Plans](plans/sendcloud-plans-pricing.yml)
- [Rate Limits](rate-limits/sendcloud-rate-limits.yml)
- [Fin Ops](finops/sendcloud-finops.yml)
- [SDK](https://github.com/Sendcloud/SendCloud-API-PHP-Wrapper)
- [SDK](https://github.com/Sendcloud/api-integration-example)
- [Integration](https://github.com/Sendcloud/prestashop-thirtybees-module)
- [Integration](https://github.com/Sendcloud/sendcloud)
- [Integration](https://github.com/Sendcloud/salesforce-b2c-commerce-cartridge)
- [Integration](https://github.com/Sendcloud/spp-integration-example)
- [Features](undefined)
- [Use Cases](undefined)
- [Solutions](undefined)
- [Integrations](https://www.sendcloud.com/integrations/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
