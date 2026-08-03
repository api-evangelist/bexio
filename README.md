# bexio (bexio)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
