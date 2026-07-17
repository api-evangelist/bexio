---
name: Create a contact and issue an invoice
description: Create a customer contact in bexio, raise an invoice for them, and fetch the Swiss QR-bill PDF.
api: openapi/bexio-openapi.yml
operations: [createContact, createInvoice, getInvoicePdf]
scopes: [contact_edit, kb_invoice_edit, kb_invoice_show]
---

# Create a contact and issue an invoice

Use the bexio API (`https://api.bexio.com/2.0`) to onboard a customer and bill them.

## Auth
- Send `Authorization: Bearer <token>` on every request — an OAuth 2.0 access token
  (issuer `https://auth.bexio.com/realms/bexio`) or a Personal Access Token.
- Required scopes: `contact_edit`, `kb_invoice_edit`, `kb_invoice_show`.
- All bodies are `application/json`.

## Steps
1. **Create the contact** — `createContact` (`POST /contact`). Set `contact_type_id`
   (1 = company, 2 = person), `name_1`, and address fields. Capture the returned `id`.
2. **Create the invoice** — `createInvoice` (`POST /kb_invoice`). Reference the contact
   via `contact_id`, set `currency_id`, and provide `positions` (line items). Capture the
   invoice `id`.
3. **Fetch the QR-bill PDF** — `getInvoicePdf` (`GET /kb_invoice/{id}/pdf`) to retrieve the
   Swiss QR-bill (QR-Rechnung) rendered PDF for sending to the customer.

## Rules
- **No idempotency keys**: bexio does not deduplicate retried writes. Guard against duplicate
  contacts/invoices client-side (check before re-`POST`).
- **Errors**: a `422` means field/business-rule validation failed — read `error_code`/`message`
  in the JSON body (see `errors/bexio-problem-types.yml`). `403` means the token lacks the scope.
- **Rate limits**: back off on `429` until `RateLimit-Reset`.
