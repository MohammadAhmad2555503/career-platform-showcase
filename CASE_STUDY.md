# Case Study: Career Platform

## Problem

A normal portfolio site is often static, shallow, and hard to maintain. For employer-facing work, the better target is a career platform: projects, writing, CVs, contact, search, admin workflows, media, and analytics in one maintainable system.

## Solution

Career Platform is a production-oriented personal career hub built with Next.js App Router, TypeScript, Tailwind CSS, Supabase, and Resend. It intentionally starts with safe configurable seed content so no fake personal claims are hardcoded.

## What I Built

- Public routes for portfolio, about, projects, work, writing, articles, series, archive, CV, lab, trivia, search, and contact.
- A typed content model and repository layer that can switch from seed content to Supabase-backed content.
- Supabase schema with normalized tables for profile settings, professional links, skills, technologies, projects, files, articles, series, chapters, CVs, career data, media, contact messages, relationships, and analytics events.
- Admin-only CMS foundation using an admin_users table rather than public registration.
- Contact API with Zod validation, honeypot bot handling, IP hash rate limiting, optional database persistence, and Resend email delivery.
- Production-supporting routes for sitemap, robots, metadata, loading, error, and not-found states.

## Engineering Judgement

The project is built as a platform foundation instead of a one-off landing page. It separates content contracts, database persistence, API validation, admin access, email delivery, and user-facing routes. It also avoids hardcoding false profile claims, which is important for an employer-facing site.

## Employer Signal

This project demonstrates frontend product judgement, typed full-stack Next.js delivery, database/schema thinking, secure contact workflows, CMS architecture, and the ability to design an employer-facing product that can grow over time.
