<div align="center">

# Solomonster

### Web-novel publishing platform with PLUS subscription and translation teams

**$499** · one-time license · Russian UI

[← Back to the price list](../README.md)

</div>

---

## In one paragraph

Solomonster is a full web-novel portal for authors and translation teams, in the style of Korean novel portals. Readers get a feature-rich reader and ranked discovery. Authors get a writing studio and bulk import. The site earns money through coins, paid and early-access chapters, and a **PLUS reader subscription** whose revenue is split between authors automatically. Translation teams share revenue inside the platform. It runs on Next.js with PostgreSQL.

---

## Stack

| Layer | Technology |
|---|---|
| Framework | **Next.js 16** (App Router, React Server Components, standalone build) |
| UI | **React 19**, TypeScript, Tailwind CSS 3, shadcn/ui (Radix), lucide icons |
| Database | **PostgreSQL 16** + **Prisma 5** |
| Auth | Encrypted cookie sessions (iron-session), **argon2id** password hashes, forced logout, device / login log |
| Editor | TipTap |
| Storage | Any S3-compatible bucket, with presigned uploads |
| Images | Client-side WebP compression, AVIF / WebP delivery |
| Real-time | Server-Sent Events over PostgreSQL `LISTEN / NOTIFY`, no Redis needed |
| Caching | Next.js data cache with audience-segmented revalidation |
| Mail | SMTP (Mailgun or any provider) |
| Geo | MaxMind GeoIP2 |
| Deployment | Node 22, PM2, Nginx, Let's Encrypt, cron endpoints, backup script (aaPanel guide) |

---

## Features

### Reader
- Themes (light, sepia, dark, black), fonts, size, line spacing, column width, justify
- **Focus mode**, auto-scroll, "time left" based on your reading speed
- **Read aloud** paragraph by paragraph (Text-to-Speech)
- Table of contents with search, image lightbox, bookmarks, likes, error reports
- Resume at the exact position, synced to the server; reading history
- **Character dialogue bubbles** with avatars inside chapters

### Catalogue and discovery
- Filters: genre, tag, status, country, 18+; search with autocomplete
- Rankings by day / month / year from a 5-signal score, updates feed
- Collections, editor's choice, banners
- **Live activity feed** with an online counter; public site statistics with charts

### Title page
- Rating, favourites, chapter list with volumes, lock icons and prices
- Release activity and next-chapter countdown
- Gifts to the author, "notify me"
- **Download as EPUB / FB2 / TXT**

### Author studio
- Novels, volumes and chapters in a TipTap editor with **version history** and scheduled publishing
- Renumber / reorder, bulk actions and bulk pricing (up to 500 chapters at once), character list
- **Import DOCX / TXT / MD / ZIP** with automatic chapter splitting
- **Rulate importer** (admin): pulls titles and chapters, re-syncs on a schedule, copies images to S3
- Co-editors with 9 permission types, per-country blocking, income and statistics pages

### Translation teams
- Members, invites, applications, recruitment
- **Revenue shares and payouts** inside the team, chapter assignments

### Monetization
- Coin wallet on a ledger; paid chapters with a platform commission (20% by default); early access
- **PLUS subscription**:
  - plans for 1 week, 1 month, 6 months and 12 months
  - subscribers can read paid chapters, up to 25% of a novel per week
  - **83% of subscription revenue goes to authors**, calculated automatically
- Promo codes, donations, author withdrawal requests
- Top-up: manual (admin approves) or **RoboKassa** (enable it with your merchant keys)

### Engagement
- Daily check-in, reader challenges, seasonal events with a coin multiplier
- **~300 achievements**

### Community
- Comment trees with likes, recommendations and stickers; reports auto-flag spam
- Reviews with a first-review reward
- Notifications (8 types) and an email digest
- **Private messages encrypted at rest** (AES-256-GCM), with reports
- Blog, job openings, support tickets, public profiles

### Admin and moderation
- About 30 admin sections:
  - dashboard
  - users: warn, ban, restrict, wipe comments, CSV export
  - about 30 roles
- Novel moderation: text and media reviewed separately; banned-word and duplicate-title audit
- Finance: transactions, withdrawals, PLUS queue and revenue distribution
- Promo codes, stickers, pages and posts, settings, logs, moderation hub

### SEO and security
- Sitemap, robots.txt, RSS, web manifest, OpenGraph, per-page metadata
- Rate limits on login, registration, password reset and email change
- Geo-blocking, with protection against faked country headers
- Staff-only middleware gate; bans checked on every request
- 18+ flags, cookie consent
- The app refuses to start in production with missing secrets

---

## Size

| Metric | Value |
|---|---|
| Pages | 126 |
| API routes | 216 (82 admin) |
| Data models | 98 + 21 enums |
| UI components | ~216 |

---

## Good to know

- **UI language:** Russian only. Strings are hard-coded, so translating the UI is a custom job.
- **Payments:** RoboKassa ships switched off. Payouts to authors are approved and paid by an admin.
- Email verification is off by default (accounts are active immediately).
- Self-service team creation is behind an admin switch.
- Rate limits are kept in memory (one app process).
- **Tests:** no unit-test suite; QA is a crawler that checks about 300 routes.

---

<div align="center">

**Solomonster · $499**

[Order / ask for a demo](../README.md#how-to-buy) · [Compare platforms](../README.md#compare-platforms)

</div>
