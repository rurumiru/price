<div align="center">

# XI PROJECTS · Platform Store

### Ready-made web-novel platforms. Buy the source code and launch under your own brand.

**6 platforms · 4 technology lines · one-time license · self-hosted**

<br>

![Platforms](https://img.shields.io/badge/platforms-6-7c3aed?style=for-the-badge)
![From](https://img.shields.io/badge/from-%24299-16a34a?style=for-the-badge)
![License](https://img.shields.io/badge/license-one--time-111111?style=for-the-badge)
![Source](https://img.shields.io/badge/source%20code-included-2563eb?style=for-the-badge)

<br>

[Price list](#price-list) •
[Which one fits?](#which-one-fits) •
[Platforms](#platforms) •
[Compare](#compare-platforms) •
[What you get](#whats-included) •
[Services](#add-on-services) •
[How to buy](#how-to-buy) •
[FAQ](#faq) •
[Contacts](#contacts)

</div>

---

## Price list

| Platform | Stack | Database | UI language | Price |
|---|---|---|---|---:|
| [**erIIIba**](platforms/eriiiba.md) | Laravel 12 · Filament 3 · Livewire 3 | MySQL / MariaDB | Russian | **$299** |
| [**NineHeavens**](platforms/nineheavens.md) | Yii 1.1 · PHP 8.3 / 8.4 | PostgreSQL | English | **$399** |
| [**Solomonster**](platforms/solomonster.md) | Next.js 16 · React 19 · Prisma | PostgreSQL 16 | Russian | **$499** |
| [**Weba**](platforms/weba.md) | Next.js 16 · React 19 · Prisma | PostgreSQL 16 | Russian | **$599** |
| [**Baxilib**](platforms/baxilib.md) | 🔒 Secret engine | PostgreSQL 17 | Russian (+ English switch) | **$939** |
| [**Dragons Heaven**](platforms/dragons-heaven.md) | 🔒 Secret engine | PostgreSQL 17 | English | **$939** |

> **One-time payment. Full source code. No mandatory monthly fees.**
> Every platform is a working product with its own feature set. Nothing is locked behind an artificial "tier": what is listed on a platform's page is in its code.

---

## Which one fits?

| You need… | Take |
|---|---|
| An **English** site where a team **translates together** (segments, versions, voting) | **NineHeavens** |
| An **English** site with coins, early access, **PayPal and crypto**, strong security and automated tests | **Dragons Heaven** |
| A **Russian** site with the **most features** on a mainstream JS stack: 4 payment gateways, 5 social logins | **Weba** |
| A **Russian** site with a **reader subscription** (PLUS) and **teams that share revenue** | **Solomonster** |
| A **Russian** site with **teams**, **monthly passes**, **payouts** and **takeover of abandoned translations** | **Baxilib** |
| The **lowest price**, ordinary PHP + MySQL hosting, a Laravel codebase to extend | **erIIIba** |
| Nothing but PostgreSQL on the server: no Redis, no search server | **Baxilib** or **Dragons Heaven** |

---

## Platforms

### erIIIba · $299
**Laravel web-novel library with a Filament admin panel**

`PHP 8.2+` `Laravel 12` `Filament 3` `Livewire 3` `Tailwind 4` `MySQL / MariaDB`

- Filament admin panel + separate moderator panel with pre-moderation of novels, covers and descriptions
- Live catalogue with URL filters; **home-page layout builder** (ranked blocks, grid / list / swiper, HTML banners)
- Paid chapters, **paid title promotion**, subscription and withdrawal requests (payments confirmed by admin)
- **EPUB / FB2 / TXT** downloads; import TXT / FB2 / DOC / DOCX and ZIP; Rulate parser
- Beta readers with notes, typo reports, scraper blocking, geo-block, 18+ gate
- Public read-only **REST API**

**[Full specification →](platforms/eriiiba.md)**

---

### NineHeavens · $399
**Collaborative translation platform for web novels**

`PHP 8.3 / 8.4` `Yii 1.1` `PostgreSQL` `WebP pipeline` `JSON API`

- **Translate together:** segments → versions → voting → published chapter; rich editor with translator's notes and images
- Teams with 7 roles and a per-title access matrix; beta readers see unreleased chapters
- **Bulk import:** ZIP / many files, or one big TXT / MD / HTML / **DOCX / EPUB** split by headings
- Paid chapters and early access on a database ledger (manual and Ko-fi top-up)
- **XP cultivation realms** (Mortal → Immortal Emperor), GIF comments, 5-star ratings, three-column title page
- Admin-managed promo carousel, **WordPress (Fictioneer) migration toolkit**, JSON-LD SEO

**[Full specification →](platforms/nineheavens.md)**

---

### Solomonster · $499
**Web-novel publishing platform with PLUS subscription and translation teams**

`Next.js 16` `React 19` `TypeScript` `Prisma` `PostgreSQL 16` `shadcn/ui`

- **PLUS reader subscription**: 83% of revenue goes to authors, calculated automatically
- **Translation teams** with revenue shares, payouts, invites and recruitment
- Coins, paid chapters, early access, promo codes; RoboKassa ready
- Reader with focus mode, auto-scroll, read-aloud, **character dialogue bubbles**
- Author studio: version history, scheduled publishing, bulk pricing, DOCX / ZIP import, Rulate importer
- ~300 achievements, events, daily check-in, **encrypted private messages**, live activity feed

**[Full specification →](platforms/solomonster.md)**

---

### Weba · $599
**Flagship Next.js platform with 4 payment gateways and 5 social logins**

`Next.js 16` `React 19` `TypeScript` `Prisma` `PostgreSQL 16` `TipTap 3` `sharp`

- **Payments:** RoboKassa, YooKassa, CloudPayments, PayAnyWay + manual methods
- **Sign-in:** Google, Yandex, VK ID, Mail.ru, Discord (+ Telegram linking)
- Two reader layouts, read-aloud, **EPUB / FB2 / TXT** export, live activity feed
- Author studio with version history and edit-conflict protection, scheduled publishing, Rulate importer
- **~50 admin pages**, ~150 settings, events and ~300 achievements
- Security-hardened (internal audit, September 2026); Kakao Page-inspired light / dark design

**[Full specification →](platforms/weba.md)**

---

### Baxilib · $939
**Russian platform with teams, passes and payouts, on a private engine**

`🔒 Secret engine` `PostgreSQL 17` `Docker` `PWA` `204 test files`

- **Translation teams** with 3 nested access levels; **takeover of abandoned translations**, with the right to object
- **Monthly pass per novel**, early access, promo codes, paid promotion, author payouts
- Full-text search, **offline reading**, read-aloud, EPUB / FB2 / TXT
- Support tickets, beta readers, typo reports, copyright claims with counter-notices, appeals
- **OPDS catalogue**, IndexNow, JSON-LD, Atom feed
- Only PostgreSQL on the server: jobs, search and counters run inside it

**[Full specification →](platforms/baxilib.md)**

---

### Dragons Heaven · $939
**English web-novel platform on a private high-performance engine**

`🔒 Secret engine` `PostgreSQL 17` `Docker` `PWA + Web Push` `~3,100 tests`

- **6 payment gateways:** Robokassa, PayAnyWay, **PayPal**, **NOWPayments (crypto)**, Crypto Bot, Tribute
- **Real-time** notifications, messages, comments and new chapters; live admin monitoring
- **Community Boost pool**, referral programme, paid placement slots, early access
- Reader with paragraph highlights and notes, offline reading, EPUB / FB2 / TXT
- Passwordless sign-in, **Content-Security-Policy**, HMAC-verified payment callbacks, data export
- Copyright takedowns, appeals, JSON-LD, sectioned sitemap, per-novel RSS

**[Full specification →](platforms/dragons-heaven.md)**

---

## Compare platforms

✅ included and on · ⚙️ included, off by default or needs your API keys · — not included

| | erIIIba | NineHeavens | Solomonster | Weba | Baxilib | Dragons Heaven |
|---|:---:|:---:|:---:|:---:|:---:|:---:|
| **Price** | **$299** | **$399** | **$499** | **$599** | **$939** | **$939** |
| Stack | Laravel 12 | Yii 1.1 | Next.js 16 | Next.js 16 | 🔒 | 🔒 |
| Database | MySQL | PostgreSQL | PostgreSQL | PostgreSQL | PostgreSQL | PostgreSQL |
| UI language | RU | EN | RU | RU | RU (+EN) | EN |
| Deployment | Nginx + PHP-FPM | Nginx + PHP-FPM | Node + PM2 | Node + PM2 | Docker | Docker |
| Automated tests | — | — | route crawler | QA scripts | 204 files | ~3,100 tests |
| **Reading** | | | | | | |
| Reader themes & typography | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Read aloud (TTS) | — | ✅ | ✅ | ✅ | ✅ | ✅ |
| Progress synced to server | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Offline reading | — | — | — | — | ✅ | ✅ |
| E-book download | EPUB / FB2 / TXT | chapter text | EPUB / FB2 / TXT | EPUB / FB2 / TXT | EPUB / FB2 / TXT | EPUB / FB2 / TXT |
| Full-text search | — | — | — | — | ✅ | ✅ |
| **Publishing** | | | | | | |
| Rich-text editor | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Scheduled publishing | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Bulk import formats | TXT FB2 DOCX ZIP | TXT MD HTML DOCX EPUB ZIP | TXT MD DOCX ZIP | TXT MD DOCX ZIP | TXT MD ZIP | TXT MD ZIP |
| Rulate importer | ✅ | — | ✅ | ✅ | ⚙️ | ⚙️ |
| WordPress migration | — | ✅ | — | — | — | — |
| Collaborative segment translation | — | ✅ | — | — | — | — |
| Translation teams | — | ✅ | ✅ | ⚙️ | ⚙️ | — |
| **Money** | | | | | | |
| Coins & paid chapters | ✅ | ⚙️ | ✅ | ✅ | ✅ | ✅ |
| Early access | — | ✅ | ✅ | ✅ | ✅ | ✅ |
| Subscription / pass | manual | — | ✅ PLUS | ⚙️ | ✅ per novel | — |
| Online payment gateways | — | Ko-fi | ⚙️ 1 | ✅ 4 | ⚙️ 3 | ✅ 6 |
| Promo codes | — | — | ✅ | ✅ | ✅ | — |
| Cash-out requests | ✅ | — | ✅ | ✅ | ⚙️ | — |
| Paid promotion of titles | ✅ | — | — | — | ✅ | ✅ |
| **Community** | | | | | | |
| Comments & ratings | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Reviews | — | ✅ | ✅ | ✅ | ✅ | ✅ |
| Private messages | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| XP / achievements | — | ✅ | ✅ | ✅ | ✅ | ✅ |
| Real-time updates | — | — | ✅ | ✅ | ✅ | ✅ |
| Social login | — | — | ⚙️ | ✅ | ⚙️ | ⚙️ |
| **Admin & SEO** | | | | | | |
| Admin panel | Filament | ✅ | ✅ | ✅ | ✅ | ✅ |
| Sitemap | — | ✅ | ✅ | ✅ | ✅ | ✅ |
| JSON-LD structured data | — | ✅ | — | — | ✅ | ✅ |

Each platform's page has the full feature list and a **"Good to know"** section with its limits.

---

## What's included

Every purchase includes:

- **Full source code** of the chosen platform
- **Database schema and migrations**
- **Deployment guide** for your server: aaPanel / Nginx, or Docker for the secret-engine platforms
- **Commercial license** for your project
- No production data: user data from live sites is never included

Not included by default (see [services](#add-on-services)): hosting, installation, design changes, translation of the UI, new features.

---

## Add-on services

Quoted per project:

| Area | Examples |
|---|---|
| **Launch** | Server setup, installation, domain and SSL, Cloudflare / CDN, S3 storage, backups |
| **Branding** | Logo, colours, fonts, custom home page and reader design |
| **Language** | Translating the interface (RU ↔ EN) or adding a new language |
| **Migration** | Import from WordPress, Rulate or another CMS; moving an existing database |
| **Payments** | Connecting a payment gateway, switching on subscriptions or payouts |
| **Features** | Custom modules, integrations (Discord, Telegram), API work |
| **Performance** | Database tuning, caching, load testing |

---

## How to buy

1. **Message us** on Telegram, Discord or email, naming the platform you are interested in.
2. **See a demo.** A demonstration can be arranged before purchase: home page, catalogue, title page, reader, profile, admin panel, mobile version.
3. **Agree the terms.** One-time payment; add-on services are quoted separately.
4. **Receive the code** with the deployment guide.
5. **Launch it yourself** or order installation from us.

---

## FAQ

**Why is the stack of Baxilib and Dragons Heaven secret?**
Both run on the private XI engine, whose technology is not disclosed publicly. The buyer receives the full source code and the stack details under an NDA. What we can say publicly:
- the database is PostgreSQL 17
- nothing else is required on the server (no Redis, no search server, no message broker)
- it ships as a Docker image
- it comes with an automated test suite

**Are the platforms the same product in different frameworks?**
No. Each is a separate working product with its own strengths. Use the [comparison table](#compare-platforms) and each platform's "Good to know" section.

**Can I change the interface language?**
- NineHeavens and Dragons Heaven are in English.
- Baxilib is in Russian with a built-in English switch (about 80% of strings translated).
- Weba, Solomonster and erIIIba are in Russian with hard-coded strings.

Translation is available as an add-on service.

**Is hosting included?**
No. All platforms are self-hosted on your own server. Requirements are listed on each platform's page.

**Are there monthly fees?**
No. The license is a one-time payment. Support and updates can be agreed separately.

**Can I resell the code?**
No, unless your contract explicitly allows it. See [License](#license).

---

## License

All platforms are commercial proprietary software. A purchased license grants usage rights according to the agreement made with the buyer.

Unless explicitly permitted by contract, the following are prohibited:

- Redistribution
- Resale of the source code
- Public source publication
- Unauthorized sublicensing
- Removal of licensing restrictions

Custom commercial agreements can be discussed separately.

---

## Contacts

```text
Telegram: @licht_re
Discord:  exseiba
Email:    rumisaca@gmail.com
```

---

<div align="center">

# XI PROJECTS

### Pick the platform. Launch the library. Own the business.

**Commercial infrastructure for modern web fiction.**

</div>
