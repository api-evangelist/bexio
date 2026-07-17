---
name: Log billable time against a project
description: Find or create a bexio project and record a timesheet entry against it.
api: openapi/bexio-openapi.yml
operations: [listProjects, createProject, createTimesheet]
scopes: [project_show, project_edit, monitoring_edit]
---

# Log billable time against a project

Record billable work in bexio Projects & Time Tracking.

## Auth
- `Authorization: Bearer <token>`; scopes `project_show`/`project_edit` and `monitoring_edit`
  (time entries).

## Steps
1. **Find the project** — `listProjects` (`GET /pr_project`), page with `limit`/`offset`,
   match on `name` / `contact_id`.
2. **Create it if missing** — `createProject` (`POST /pr_project`). Set `name`, `contact_id`,
   `pr_state_id`, and optional `start_date`/`end_date`. Capture the `id`.
3. **Log time** — `createTimesheet` (`POST /timesheet`). Reference the project and the user,
   and record the duration and date of the billable work.

## Rules
- **No idempotency**: a retried `createTimesheet` creates a second entry — confirm success
  before retrying.
- **Errors**: read the `error_code`/`message` JSON body; `403` = missing scope, `429` = rate limited.
- **Auth model & scopes**: see `authentication/bexio-authentication.yml` and `scopes/bexio-scopes.yml`.
