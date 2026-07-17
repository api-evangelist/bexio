---
name: Maintain the items/products catalog
description: List and create items/products (Artikel) with sale and purchase prices in bexio.
api: openapi/bexio-openapi.yml
operations: [listArticles, createArticle]
scopes: [article_show, article_edit]
---

# Maintain the items/products catalog

Manage the bexio items catalog (Artikel) that backs invoice and order line items.

## Auth
- `Authorization: Bearer <token>`; scopes `article_show` (read) and `article_edit` (write).

## Steps
1. **List existing items** — `listArticles` (`GET /article`). Use `limit`/`offset` to page
   (default page size 500, maximum 2000). Match on `intern_code` to avoid duplicates.
2. **Create an item** — `createArticle` (`POST /article`). Set `intern_name`, `intern_code`,
   `sale_price`, `purchase_price`, and `currency_id`. Prices are strings.

## Rules
- **Pagination**: iterate with `offset` until fewer than `limit` rows return.
- **No idempotency**: check by `intern_code` before creating to avoid duplicate items.
- **Errors**: `422` = validation failure (inspect `error_code`/`message`); `429` = slow down.
