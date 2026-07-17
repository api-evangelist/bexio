# bexio (bexio)

bexio is a Swiss cloud business-management platform for SMBs and self-employed, covering accounting, invoicing (incl. Swiss QR-bill), contacts, sales orders, projects and time tracking, banking, purchasing, and payroll. The bexio REST API at api.bexio.com/2.0 exposes these modules over HTTPS with JSON, secured by OAuth 2.0 (OpenID Connect) or Personal Access Tokens.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/apis.yml)

## Tags

- Accounting
- ERP
- Invoicing
- SMB
- Switzerland

## Timestamps

- **Created:** 2026-07-17
- **Modified:** 2026-07-17

## APIs

### bexio Contacts API

Manage contacts, relations, groups, and sectors - the shared address book behind bexio quotes, orders, invoices, and projects. Scopes contact_show / contact_edit.

- **Human URL:** [https://docs.bexio.com/](https://docs.bexio.com/)
- **Base URL:** `https://api.bexio.com/2.0`

#### Tags

- Contacts
- CRM
- Address Book

#### Properties

- [Documentation](https://docs.bexio.com/)
- [API Reference](https://docs.bexio.com/)
- [OpenAPI](openapi/bexio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bexio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### bexio Sales Order Management API

Create and manage quotes (Offerte), orders (Auftrag), and invoices (Rechnung), including Swiss QR-bill (QR-Rechnung) PDF generation and payments. Scopes kb_offer_*, kb_order_*, kb_invoice_*.

- **Human URL:** [https://docs.bexio.com/](https://docs.bexio.com/)
- **Base URL:** `https://api.bexio.com/2.0`

#### Tags

- Invoicing
- Quotes
- Orders
- QR-Bill

#### Properties

- [Documentation](https://docs.bexio.com/)
- [OpenAPI](openapi/bexio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bexio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### bexio Accounting API

Chart of accounts (Konten), Swiss VAT (MWST) tax rates, currencies, and manual journal entries (Buchungen). Scope accounting.

- **Human URL:** [https://docs.bexio.com/](https://docs.bexio.com/)
- **Base URL:** `https://api.bexio.com/2.0`

#### Tags

- Accounting
- Ledger
- VAT

#### Properties

- [Documentation](https://docs.bexio.com/)
- [OpenAPI](openapi/bexio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bexio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### bexio Items API

Manage items / products (Artikel) with sale and purchase prices and stock. Scopes article_show / article_edit.

- **Human URL:** [https://docs.bexio.com/](https://docs.bexio.com/)
- **Base URL:** `https://api.bexio.com/2.0`

#### Tags

- Products
- Inventory
- Catalog

#### Properties

- [Documentation](https://docs.bexio.com/)
- [OpenAPI](openapi/bexio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bexio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### bexio Projects & Time Tracking API

Projects, timesheets, and tasks for billable work. Scopes project_show / project_edit, task_show / task_edit.

- **Human URL:** [https://docs.bexio.com/](https://docs.bexio.com/)
- **Base URL:** `https://api.bexio.com/2.0`

#### Tags

- Projects
- Time Tracking
- Timesheets

#### Properties

- [Documentation](https://docs.bexio.com/)
- [OpenAPI](openapi/bexio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bexio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### bexio Files API

Upload, list, and manage files and document attachments. Scope file.

- **Human URL:** [https://docs.bexio.com/](https://docs.bexio.com/)
- **Base URL:** `https://api.bexio.com/2.0`

#### Tags

- Files
- Documents
- Storage

#### Properties

- [Documentation](https://docs.bexio.com/)
- [OpenAPI](openapi/bexio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bexio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### bexio Purchase API

Supplier bills (Lieferantenrechnungen) and expenses (Spesen) on the accounts-payable side. Scopes kb_bill_*, kb_expense_*.

- **Human URL:** [https://docs.bexio.com/](https://docs.bexio.com/)
- **Base URL:** `https://api.bexio.com/2.0`

#### Tags

- Purchasing
- Bills
- Expenses

#### Properties

- [Documentation](https://docs.bexio.com/)
- [OpenAPI](openapi/bexio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bexio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### bexio Payroll API

Payroll employees, absences, and paystubs for Swiss salary processing. Scopes payroll_employee_*, payroll_absence_*, payroll_paystub_show.

- **Human URL:** [https://docs.bexio.com/](https://docs.bexio.com/)
- **Base URL:** `https://api.bexio.com/2.0`

#### Tags

- Payroll
- HR
- Absences

#### Properties

- [Documentation](https://docs.bexio.com/)
- [OpenAPI](openapi/bexio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bexio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### bexio Banking API

Bank accounts and bank payments (Swiss IBAN / QR-bill reconciliation). Scopes bank_account_*, bank_payment_*.

- **Human URL:** [https://docs.bexio.com/](https://docs.bexio.com/)
- **Base URL:** `https://api.bexio.com/2.0`

#### Tags

- Banking
- Payments
- IBAN

#### Properties

- [Documentation](https://docs.bexio.com/)
- [OpenAPI](openapi/bexio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bexio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

## Common Properties

- [Agentic Access](agentic-access/bexio-agentic-access.yml)
- [Trust Center](security/bexio-trust-center.yml)
- [Vulnerability Disclosure](security/bexio-vulnerability-disclosure.yml)
- [Domain Security](security/bexio-domain-security.yml)
- [Authentication](authentication/bexio-authentication.yml)
- [GitHub Organization](https://github.com/bexiocom)
- [LinkedIn](https://www.linkedin.com/company/bexio-ag)
- [Website](https://www.bexio.com/)
- [Documentation](https://docs.bexio.com/)
- [Plans](plans/bexio-plans-pricing.yml)
- [Rate Limits](rate-limits/bexio-rate-limits.yml)
- [Fin Ops](finops/bexio-finops.yml)
- [Blog](https://www.bexio.com/en-CH/blog)

## Notes

- **Spec provenance:** bexio does not publish a first-party OpenAPI definition as of 2026-07-17 (their docs state one is planned). `openapi/bexio-openapi.yml` is **modeled from the public documentation** at [docs.bexio.com](https://docs.bexio.com/) and the live OpenID Connect configuration.
- **Auth:** OAuth 2.0 Authorization Code / OpenID Connect (issuer `https://auth.bexio.com/realms/bexio`) or Personal Access Tokens; both sent as `Authorization: Bearer`.
- **No WebSocket / no native webhooks:** the bexio API is synchronous REST only. See `review.yml`.
- **Region & currency:** Swiss (CHF), Swiss QR-bill (QR-Rechnung) support, VAT (MWST) handling; data hosted in Switzerland. bexio AG is part of Die Mobiliar.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
