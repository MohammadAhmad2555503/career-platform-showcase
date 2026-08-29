# Security and Privacy: Career Platform

## Privacy Model

The platform avoids fake profile facts and uses configurable seed content until real administrator-approved content is entered.

## Key Protections

- .env.example documents required variables without including secrets.
- Supabase service-role key is server-only.
- Admin access is based on an explicit admin_users table.
- No public registration route is exposed by default.
- Contact form uses Zod validation.
- Honeypot field quietly accepts bot submissions without sending mail.
- Rate limiting hashes the request source rather than storing raw IPs in app code.
- Contact messages can be stored in Supabase and delivered via Resend.
- Private files should live in non-public Supabase buckets and be served through signed URLs.

## Public Showcase Choice

This showcase repository contains documentation only. It is suitable for public employer review without exposing environment values, personal inbox data, private files, or unpublished profile content.
