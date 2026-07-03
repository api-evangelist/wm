# WM (wm)

WM (formerly Waste Management, Inc.) is North America's largest integrated environmental solutions company, serving nearly 20 million municipal, commercial, industrial, and residential customers through collection, transfer, recycling, landfill, and waste-to-energy operations.

**WM does not run a self-serve, publicly-signup developer platform.** It publishes a documented partner/customer REST API at [api.wm.com](https://api.wm.com/) covering account-level service and billing data - service details and pickup schedules, live service status and truck ETA, routing and hauling material information, pricing, invoices and aging balance, communication preferences, contacts, cases, tickets, and account activity notes. Access requires a WM-issued `ClientId` plus a JSON Web Token (JWT) and is granted on request to existing commercial/enterprise customers and integration partners by emailing [apiaccess@wm.com](mailto:apiaccess@wm.com); there is no open, self-serve API key signup.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/apis.yml)

## Tags

- Waste Management
- Recycling
- Environmental Services
- Field Services
- Logistics
- Account Management
- Enterprise
- B2B

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### WM Services API

Retrieve the services associated with a customer account - service names, material streams, equipment/container details, and pricing - plus today's service execution plan, completed-service status and history, next scheduled pickup date, and estimated truck arrival time (ETA) for an in-progress service.

- **Human URL:** [https://api.wm.com/Services/index.html](https://api.wm.com/Services/index.html)
- **Base URL:** `https://api.wm.com/v1`

#### Properties

- [Documentation](https://api.wm.com/servicesoverview/index.html)
- [API Reference](https://api.wm.com/Services/index.html)
- [OpenAPI](openapi/wm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WM Service Operations & Materials API

Retrieve routing information for a service, including the day of week it is serviced, and hauling material information (material code, name, special-handling and manifest flags) for all services on an account.

- **Human URL:** [https://api.wm.com/serviceoperations/](https://api.wm.com/serviceoperations/)
- **Base URL:** `https://api.wm.com/v1`

#### Properties

- [API Reference](https://api.wm.com/serviceoperations/)
- [API Reference](https://api.wm.com/servicematerial/)
- [OpenAPI](openapi/wm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WM Service Pricing API

Retrieve the base monthly rates for an account's services and the invoice fee schedule (disposal rate type/amount and other line-item fees) applied to those services.

- **Human URL:** [https://api.wm.com/serviceprice/](https://api.wm.com/serviceprice/)
- **Base URL:** `https://api.wm.com/v1`

#### Properties

- [API Reference](https://api.wm.com/serviceprice/)
- [OpenAPI](openapi/wm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WM Invoices & Balance API

Retrieve invoice history (invoice id, date, amount, payment information, remaining balance) and the current aging balance due on an account, broken out by Current, 30/60/90/120-day, and Future buckets, plus the last payment amount and date.

- **Human URL:** [https://api.wm.com/InvoiceS/index.html](https://api.wm.com/InvoiceS/index.html)
- **Base URL:** `https://api.wm.com/v1`

#### Properties

- [API Reference](https://api.wm.com/InvoiceS/index.html)
- [API Reference](https://api.wm.com/balance/index.html)
- [OpenAPI](openapi/wm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WM Profiles & Preferences API

Retrieve paperless billing and auto-pay settings plus WM.com login status established at signup, and retrieve or update account communication preferences against the published preference categories.

- **Human URL:** [https://api.wm.com/profiles/index.html](https://api.wm.com/profiles/index.html)
- **Base URL:** `https://api.wm.com/v1`

#### Properties

- [Documentation](https://api.wm.com/preferences_overview/index.html)
- [API Reference](https://api.wm.com/profiles/index.html)
- [API Reference](https://api.wm.com/preferences_get/index.html)
- [API Reference](https://api.wm.com/preferences_put/index.html)
- [API Reference](https://api.wm.com/preferencescategories/index.html)
- [OpenAPI](openapi/wm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WM Contacts API

Retrieve service and billing contact information (name, phone, fax, email, address) on file for an account, and update service or billing contact details.

- **Human URL:** [https://api.wm.com/contactsoverview/index.html](https://api.wm.com/contactsoverview/index.html)
- **Base URL:** `https://api.wm.com/v1`

#### Properties

- [Documentation](https://api.wm.com/contactsoverview/index.html)
- [API Reference](https://api.wm.com/Contactbilling/index.html)
- [OpenAPI](openapi/wm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WM Cases & Tickets API

List service cases (id, description, category, request date/time, status) and case detail, and list and retrieve detail for tickets - such as missed-pickup or extra-pickup requests - created against an account over a given date range.

- **Human URL:** [https://api.wm.com/cases/index.html](https://api.wm.com/cases/index.html)
- **Base URL:** `https://api.wm.com/v1`

#### Properties

- [API Reference](https://api.wm.com/cases/index.html)
- [API Reference](https://api.wm.com/caseid/index.html)
- [API Reference](https://api.wm.com/tickets/index.html)
- [API Reference](https://api.wm.com/ticketd/index.html)
- [OpenAPI](openapi/wm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WM Activities API

Retrieve special servicing instructions and account notes, system-generated or CSR-sent email communications, and portal-created issue requests for an account over a given date range.

- **Human URL:** [https://api.wm.com/activitiesoverview/index.html](https://api.wm.com/activitiesoverview/index.html)
- **Base URL:** `https://api.wm.com/v1`

#### Properties

- [Documentation](https://api.wm.com/activitiesoverview/index.html)
- [API Reference](https://api.wm.com/notes/index.html)
- [API Reference](https://api.wm.com/email/index.html)
- [API Reference](https://api.wm.com/issues/index.html)
- [OpenAPI](openapi/wm-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.wm.com)
- [Documentation](https://api.wm.com/)
- [LinkedIn](https://www.linkedin.com/company/waste-management)
- [Plans](plans/wm-plans-pricing.yml)
- [Rate Limits](rate-limits/wm-rate-limits.yml)
- [Fin Ops](finops/wm-finops.yml)

## Access Model

There is no public API key signup. WM's documentation directs prospective integrators to email **apiaccess@wm.com** with a brief description of their need and the API(s) they want access to. Approved partners/customers receive a `ClientId` and authenticate with a JSON Web Token (JWT) Bearer token, sent along with a `Request-Tracking-Id` header on every call. A separate test environment is published at `https://apitest.wm.com/v1` alongside production at `https://api.wm.com/v1`.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
