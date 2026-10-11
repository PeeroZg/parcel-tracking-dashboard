# Parcel Tracking Dashboard

Full-stack parcel tracking dashboard developed as a technical recruitment assignment.

## Tech stack

- Nuxt 4, Vue 3, TypeScript, Nuxt UI
- Node.js / Nuxt server API
- PostgreSQL (`pg`)

## Features

- Parcel list with server-side pagination and filtering
- Filters by parcel number, customer, status and pickup date
- Detailed view of individual parcels and tracking history
- SQL queries executed by server API endpoints (no direct database access from the browser)
- Sample database schema and seed data for local testing

## Run locally

Requires Node.js, pnpm and PostgreSQL.

1. Create a PostgreSQL database named `parcel_tracking`.
2. Execute `database/schema.sql`, followed by `database/seed.sql`.
3. Copy `.env.example` to `.env` and adjust your local database credentials.
4. Install dependencies and start the development server:

   ```bash
   pnpm install
   pnpm dev
   ```

5. Open <http://localhost:3000>.

## Project structure

- `app/pages/` — user interface
- `server/api/` — API endpoints
- `server/utils/database.ts` — PostgreSQL connection pool
- `database/` — database schema and sample data
- `types/` — TypeScript types

## Notes

This is a local demonstration / technical assignment project, not a deployed production service. Database credentials are kept in `.env`, which is excluded from Git. Docker was used in local development but its configuration is not included in this repository.
