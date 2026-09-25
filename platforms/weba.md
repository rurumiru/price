<div align="center">

# Weba

### Flagship Next.js web-novel platform with 4 payment gateways and 5 social logins

**$599** · one-time license · Russian UI

[← Back to the price list](../README.md)

</div>

---

## In one paragraph

Weba is the largest and newest platform in the Next.js line; Solomonster is an earlier branch of the same code. It is a complete web-novel store for Russian-speaking audiences:
- readers top up coins through **RoboKassa, YooKassa, CloudPayments or PayAnyWay**
- readers sign in with Google, Yandex, VK ID, Mail.ru or Discord
- authors publish from a studio with version history
- the admin panel has about 50 pages and around 150 settings

It has a Kakao Page-inspired design in light and dark themes, was security-hardened after an internal audit in September 2026, and ships with EPUB / FB2 / TXT export, events and about 300 achievements.

---

## Stack

| Layer | Technology |
|---|---|
| Framework | **Next.js 16** (App Router, React Server Components, standalone build) |
| UI | **React 19**, TypeScript, Tailwind CSS 3, shadcn/ui (Radix), lucide icons |
| Database | **PostgreSQL 16** + **Prisma 5** |
| Auth | Encrypted cookie sessions with server-side revocation, **argon2id** |
| Social login | Google, Yandex, VK ID, Mail.ru, Discord, plus Telegram account linking |
| Editor | **TipTap 3** |
| Storage | Any S3-compatible bucket |
| Images | **sharp**: server-side re-encoding to WebP, metadata stripped |
| Real-time | Server-Sent Events over PostgreSQL `LISTEN / NOTIFY`, no Redis needed |
| Scheduled jobs | 12 cron endpoints protected by a secret |
| Mail | SMTP (Mailgun or any provider) |
| Geo | MaxMind GeoLite2, or a trusted Nginx / Cloudflare header |
| Deployment | Node 22, PM2, Nginx, Let's Encrypt (aaPanel guide) |

---

## Features

### Reader
- Two reader layouts ("lab" and "classic"), chosen per account
- Themes (light, sepia, dark), serif / sans, text width, spacing
- Auto-scroll, **read aloud** (Text-to-Speech), minutes-left estimate
- Table of contents with search, bookmarks, image lightbox, reading progress synced to the server

### Catalogue and discovery
- Filters: genre, tag, status, country, 18+; live search suggestions
- Rankings, updates, collections, editor's choice
- Home-page banner carousel
- **Live activity feed** (`/live`)

### Title page
- Rating (1–5 stars), favourites, "continue reading", chapter list split into volumes, prices on locked chapters
- Extra cover gallery (moderated), gifts to the author, new-chapter notifications
- **Download as EPUB / FB2 / TXT**; admins choose who is allowed to download

### Author studio
- TipTap editor with **version history** and edit-conflict protection
- **Import DOCX / TXT / MD / ZIP**; bulk publish, bulk pricing, renumbering
- Volumes, **scheduled publishing**, co-editors with 9 permission types, per-country blocking
- Character list with avatars, shown in chapters as **speech bubbles**
- Income and statistics pages
- **Rulate importer** (admin) with scheduled re-sync

### Monetization
- Coin wallet (1 coin = 1 RUB)
- Paid chapters with a platform commission (20% by default), **early access**, chapters that unlock automatically later
- **Payment gateways:** RoboKassa, YooKassa, CloudPayments, PayAnyWay. Also manual methods: SBP, card, Boosty, crypto and others.
- Promo codes: balance, free chapters, free novel, subscription days
- Gifts, donations, refund requests, author withdrawal requests

### Engagement
- **~300 achievements** in about 27 families
- Daily check-in, reader challenges
- Events with tasks, tiers and rewards

### Community
- Threaded comments with likes, reports and stickers
- Reviews with a first-review reward
- Notifications and a weekly email digest
- **Private messages encrypted at rest** (AES-256-GCM)
- Blog, job postings, support tickets, public profiles

### Admin and moderation
- **~50 admin pages**:
  - users, with sanctions and staff notes
  - about 30 roles
  - moderation of titles, covers and comments, moderation threads
  - finances and refunds, promo codes, banners, pages, stickers, events
  - **~150 settings**, audit log, CSV export
- Built-in analytics:
  - view tracking
  - site and personal statistics with a heat map
  - author statistics
  - admin dashboard

### SEO
- Sitemap, robots.txt, RSS, OpenGraph image
- **PWA manifest** (installable)

### Security
- Internal security audit on 2026-09-16; `npm audit` reports 0 issues
- Rate limits on about 20 sensitive routes
- CSRF defence (Origin / Sec-Fetch-Site checks)
- 18+ gate based on date of birth; protection against faked country headers
- Every uploaded image re-encoded; SSRF guards on export
- List of active sessions and logins
- X-Frame-Options, nosniff, Referrer-Policy and Permissions-Policy headers

---

## Size

| Metric | Value |
|---|---|
| Pages | 146 |
| API routes | 259 |
| Data models | 119 + 21 enums |
| UI components | ~275 |
| QA | Playwright check scripts, security unit checks, strict type-check |

---

## Good to know

- **UI language:** Russian only. Strings are hard-coded, so translating the UI is a custom job.
- **Switched off in this edition:** the reader subscription and translation teams. The code is in the repository but disabled; if you need them, [Solomonster](solomonster.md) has both running, or we can enable them as custom work.
- Author payouts are approved and paid by an admin; no payout provider is connected.
- Search is simple PostgreSQL pattern matching.
- No Content-Security-Policy header and no 2FA yet.
- Rate limits are kept in memory (one app process).

---

<div align="center">

**Weba · $599**

[Order / ask for a demo](../README.md#how-to-buy) · [Compare platforms](../README.md#compare-platforms)

</div>
