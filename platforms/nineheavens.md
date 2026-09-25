<div align="center">

# NineHeavens

### Collaborative translation platform for web novels

**$399** · one-time license · English UI

[← Back to the price list](../README.md)

</div>

---

## In one paragraph

NineHeavens is a platform where a team translates a novel **together**: the source text is split into segments, translators submit their versions, the team votes, and the best versions are assembled into the published chapter. Readers get a modern reader, a catalogue, comments and ratings. The team gets bulk chapter import, scheduled releases, paid chapters and a full admin panel. It is the only platform in this catalogue built around a real translation workflow, not just publishing finished text.

---

## Stack

| Layer | Technology |
|---|---|
| Backend | **Yii 1.1.32** (Composer) |
| Language | **PHP 8.3 / 8.4** |
| Database | **PostgreSQL 13–18** (plain SQL, no extensions required) |
| Cache | File cache or Memcached |
| Frontend | Server-rendered pages, own design system (dark / light tokens), jQuery |
| Images | Every stored image is converted to **WebP** (covers, avatars, banners, editor uploads) |
| JSON API | `/api/v1/*`: catalogue, updates, rankings, library, progress, chapters, comments, wallet |
| Web server | Nginx + PHP-FPM |
| Mail | Sendmail / msmtp (any SMTP relay) |
| Deployment | aaPanel guide (Ubuntu 22/24, Debian 12), cron jobs, Let's Encrypt |

**Required PHP extensions:** `pdo_pgsql`, `gd` (with WebP), `mbstring`, `iconv`, `curl`, `dom`, and `zip` for archive import.

---

## Features

### Collaborative translation
- Source text split into segments; translators submit versions; the team votes; the best versions become the chapter
- Translation versions are visible only to admins by default (switchable to team or everyone)
- Source text visible only to the team
- Rich segment editor: bold, italic, underline, strike, sup / sub, links, **translator's-note popovers**, inline images (auto-WebP)
- "Suggest a fix": readers send corrections, the team reviews them in a queue

### Teams and access rights
- Team roles: lead, translator, editor, proofreader, beta reader, typesetter, QC
- Invitations
- Per-title access matrix for reading, translating, downloading, rating, commenting and blog posting: everyone / group / moderators / owner
- Beta readers can read unreleased chapters
- Admin-defined default access for new titles and per-title overrides

### Reader
- 5 themes (paper, sepia, graphite, night, ink), font, size, line spacing, width, alignment
- Saved reading position, arrow-key navigation, chapter reactions
- Per-paragraph menu: pin, 4 colour marks, copy link, quote, suggest a fix, **read aloud** (Text-to-Speech)
- Foreword / afterword blocks, support-the-translator call-to-action

### Catalogue and title page
- Category tree, genres, tags, filters, "Updates by day", Top lists (popular, rating, activity, new), RSS
- Translation requests with voting; people directory with a follow feed
- **Three-column title page**: cover and facts on the left; description, table of contents and comments in the centre; team and similar titles on the right
- **5-star ratings**, reviews
- Table of contents with search, sort and All / Free / Premium filters
- One comment feed across all chapters: threads, spoilers, quotes, likes, **GIFs** (via a server-side proxy)

### Publishing and import
- **Bulk chapter import:**
  - many files at once, or a ZIP archive
  - one big TXT / MD / HTML / **DOCX / EPUB** file split into chapters by headings. Recognises "Chapter N", 第N章, N화, Word / Markdown / EPUB headings or a custom regex
- Preview before saving (rename, reorder, merge), resumable background jobs
- Import hardened against zip bombs, XXE and path traversal
- Scheduled chapter releases (cron)
- **WordPress migration toolkit**: users (password hashes kept), content, comments, media, legacy 301 redirects. Built for the Fictioneer theme; adapted to your site as a service.

### Monetization
- Coin wallet on a database ledger (protected by triggers, idempotent operations)
- Paid chapters, **early access** (free after a date), unlock schedules, "unlock all"
- Owner revenue share (70% by default), top-up packages
- Admin grants, refunds and chargebacks
- Payment intake: manual top-up (admin approves) and Ko-fi webhook matching

### Community
- **XP "cultivation realms"**: 8 levels from Mortal to Immortal Emperor, shown as a badge next to every commenter
- Reputation levels; bronze / silver / gold badges, some of them secret
- Blogs per title and site-wide, announcements, home-page news ticker
- Private support requests (visible only to the author and staff)
- Private messages, notifications, online / last-seen status
- Profile activity timeline with a 12-month heat map

### Home page
- Card carousel with **admin-managed promo banners**: schedule, impressions and click tracking
- Continue reading, new chapters, top lists, latest comments, genres, announcement cards

### Admin and moderation
- `/admin`: users (roles, bans, password reset), titles (owner, access, hide, copyright ban, delete), action log
- Site settings:
  - registration: open, invite-only or closed
  - site-wide banner
  - GIF provider
  - default access rules
  - translation-version visibility
- Reports and a moderation queue

### SEO
- Meta description, canonical, OpenGraph / Twitter cards, **JSON-LD**, rel prev / next
- Sitemap index with parts, robots.txt, noindex rules

### Design
- Dark / light theme (dark by default), glass cards, Golos Text + Literata / Roboto Serif
- Mobile-first pass: no horizontal overflow from 360 px, 36–40 px touch targets

---

## Size

| Metric | Value |
|---|---|
| Controllers | 42 |
| Models | 50 |
| Console commands | 17 |
| Migrations | 29 |
| View templates | ~280 |
| Database tables | ~74 |

---

## Good to know

- **UI language:** English. Interface strings go through the Yii translation layer (message files), so another language can be added by translating those files.
- **Payments:** coins ship switched off. Only manual top-ups and Ko-fi work out of the box. Card or crypto gateways are available as custom integration work.
- **Search** is simple PostgreSQL pattern matching over titles, alternative titles, authors and users. There is no external search engine.
- **Cache:** file or Memcached. Redis is not supported.
- **Tests:** no automated test suite.

---

<div align="center">

**NineHeavens · $399**

[Order / ask for a demo](../README.md#how-to-buy) · [Compare platforms](../README.md#compare-platforms)

</div>
