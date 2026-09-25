<div align="center">

# Dragons Heaven

### English web-novel platform on a private high-performance engine

**$939** · one-time license · English UI · 🔒 secret stack

[← Back to the price list](../README.md)

</div>

---

## In one paragraph

Dragons Heaven is a reading and publishing platform for translated light novels, web novels and original fiction, aimed at English-speaking readers. It runs on the **private XI engine**.
- Notifications, messages, comments and new chapters update live without reloading the page.
- It covers about 72 database tables with roughly **3,100 automated tests**.
- It needs nothing besides PostgreSQL: background jobs, full-text search and counters all run inside the database.

It includes six payment gateways (PayPal and crypto among them), a community Boost pool, copyright handling and a real-time admin monitor.

---

## Stack

| Layer | Technology |
|---|---|
| Application engine | 🔒 **Classified**: private XI engine, disclosed to the buyer under NDA |
| Database | **PostgreSQL 17**: ledger integrity and counters enforced by triggers and CHECK constraints |
| Search | Built into PostgreSQL: full-text + trigram similarity |
| Background jobs | Built in, stored in PostgreSQL (4 queues, 9 scheduled tasks) |
| External services | **None required**: no Redis, no search server, no message broker |
| Storage | Local disk or any S3-compatible bucket behind a CDN (private bucket, content-addressed files) |
| Images | WebP with responsive `srcset` variants |
| Frontend | Tailwind CSS v4, own design system (dark by default) |
| PWA | Manifest, offline service worker, **Web Push** |
| Mail | SMTP or Mailgun |
| Deployment | **Docker** multi-stage image + Docker Compose (memory limits, health checks), Nginx reverse proxy, Let's Encrypt, CI pipeline |
| Minimum server | 2 vCPU / 4 GB RAM |

---

## Features

### Reader
- 5 backgrounds (Night, OLED, Sepia, Paper, Grey), serif / sans, size, line height, width, justify, hyphenation, drop cap
- Settings and reading position **synced across devices**
- Read aloud with speed control, keep-screen-on, table of contents with search, arrow keys, mobile dock
- **Paragraph bookmarks and colour highlights with notes**
- Typo reports sent straight to the translator
- Chapter discussion, reactions, "what to read next"
- **Offline reading** of already-opened pages
- **Download as EPUB / FB2 / TXT**

### Catalogue and discovery
- Filters:
  - genres and tags, each included or excluded
  - type, country, language, status, age rating
  - year range, minimum chapters, minimum rating
- Grid or list view; filters are kept in the URL
- Instant search suggestions
- Charts by score, activity, views and length, weighted with time decay
- Updates feed, reader-made collections, series, similar titles, "readers also read"
- Home page: showcase, continue reading, weekly rating, per-genre picks, latest comments

### Title page
- Continue / read button; chapter list opens at your bookmark and is searchable
- Reviews with "helpful" votes; 1–10 ratings, shown after 5 votes
- Discussion, translator credit, 18+ gate, "unlock all paid chapters", download

### Translator studio
- Author dashboard, visual editor with a markup mode, drafts
- **Scheduled publishing** that keeps chapter order; decimal chapter numbers (12.5, prologue 0); volumes
- **Bulk import from TXT / MD / ZIP with images**, previewed before anything is saved
- "Workshop" screen for editing a whole novel at once, unlocked after 50 published chapters
- Per-chapter translator assignment
- **Rulate importer** with re-sync (needs a logged-in Rulate session)
- Metadata lookup from AniList, NovelUpdates and NovelList

### Monetization
- Coin wallet on a ledger that records every movement
- Paid chapters with a "free after" date (**early access**)
- Purchases are permanent; the translator's share is credited in the same transaction
- Coin packs, **paid placement slots** (showcase, catalogue), refund claims
- **Referral programme**: rewards for reading done by invited users
- **Community Boost pool**: readers vote, and the pool buys chapters that then open for everyone
- **Payment gateways:** Robokassa, PayAnyWay, PayPal, NOWPayments (crypto), Crypto Bot, Tribute. Also manual top-up requests with proof of payment.

### Community
- Threaded comments with spoilers, @mentions and 6 reactions
- Reviews, ratings, follows, profiles, member directory
- Private messages with blocking
- XP levels and badges, personal reading statistics
- Notification inbox with 10 per-type switches, plus **push notifications**
- Translation-request board with voting, site blog
- Discord webhook announcements; links to Telegram, VK and Boosty

### Real-time
- The notification badge, inbox, private messages, latest comments, new chapters and the Boost pool update live
- Navigation and the editor work without full page reloads

### Admin and moderation
- 8 roles (user, author, moderator, copyright, support, editor, finance, admin); 22 admin sections; separate "may move money" permission
- Dashboard with week-over-week analytics
- **Live monitoring**: 2 hours of per-minute metrics, slow requests, errors
- Reports and sanctions (warning, mute, ban) with **appeals**; audit journal
- **Copyright takedowns and counter-notices**: 3 strikes remove publishing rights
- Registration: open, closed or by application
- Novel pre-moderation
- Also managed from admin:
  - genres, tags, media, blog
  - versioned legal documents
  - commerce queue, jobs, imports, settings

### SEO
- Sectioned sitemap index with XSL styling
- RSS for the whole site and for each novel
- Generated robots.txt, canonical links, OpenGraph, **JSON-LD**
- Permanent numeric URLs, 301 redirects from old URLs, bot blocklist

### Security and privacy
- **Passwordless magic-link sign-in** with an optional password (12+ characters)
- Session list with IP and device, one-time recovery codes, re-authentication before sensitive changes
- **Content-Security-Policy with script hashes**, CSRF protection, rate limits, anti-scraper throttling, XSS-safe markup
- Signed, HMAC-verified payment callbacks that also check the amount
- Copy protection on paid text; private storage bucket behind the CDN
- Users can export their data as JSON; account deletion with a 7-day grace period; limited retention of payment data

### Migration
- Importer for a legacy site database: tested on 3,500 chapters in about a minute
- Server-migration guide, media transfer to S3, WebP backfill

---

## Size

| Metric | Value |
|---|---|
| Migrations | 129 |
| Database tables | ~72 |
| Routes | 123 |
| Screens | ~60 (23 admin) |
| Background workers | 16 |
| Automated tests | **~3,100** in 257 test files |

---

## Good to know

- **UI language:** English. The interface was built from a Russian original, so a Russian UI can be restored as an add-on.
- **Social login** (Telegram, VK, Google, Yandex) is built but switched off until you add your own app keys.
- The Boost pool ships switched off; set your own rates before enabling it.
- Payment gateways need your own merchant accounts. Test them in sandbox mode before launch (Tribute has no sandbox).
- No team entity (translator credit is free text), no subscriptions, no forum.
- File import accepts TXT / MD / ZIP. DOCX and EPUB are not supported.
- Why is the stack secret? See the [FAQ](../README.md#faq).

---

<div align="center">

**Dragons Heaven · $939**

[Order / ask for a demo](../README.md#how-to-buy) · [Compare platforms](../README.md#compare-platforms)

</div>
