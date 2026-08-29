# Architecture Brief: Career Platform

## Stack

- Next.js App Router
- TypeScript
- Tailwind CSS
- Supabase SSR/client libraries
- Supabase Postgres and RLS-aware schema
- Resend for contact email delivery
- Zod validation

## Core Boundaries

- src/lib/content/types.ts: typed content contracts.
- src/lib/content/seed.ts: safe local bootstrap content.
- src/lib/content/repository.ts: content access layer.
- src/lib/supabase: server and browser Supabase clients.
- src/app/api/contact: validated contact endpoint with honeypot, rate limiting, database inbox, and email delivery.
- src/app/api/search: global search endpoint.
- src/app/admin: private CMS shell and setup-aware login.
- supabase/migrations/0001_initial_schema.sql: normalized platform schema.

## Data Model

The schema includes profile settings, links, skills, technologies, categories, tags, media, projects, project files, articles, series, chapters, trivia, CVs, career entries, contact messages, relationships, and analytics events.
