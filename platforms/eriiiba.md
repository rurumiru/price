<div align="center">

# erIIIba

### Laravel web-novel library with a Filament admin panel

**$299** · one-time license · Russian UI

[← Back to the price list](../README.md)

</div>

---

## In one paragraph

erIIIba is the entry-level platform in this catalogue. It is a clean Laravel 12 web-novel library that runs on ordinary PHP + MySQL hosting. It has:
- a **Filament** admin panel and a separate moderator panel with pre-moderation
- a Livewire catalogue and a reader
- paid chapters, beta readers, paid title promotion
- EPUB / FB2 / TXT downloads and a read-only REST API

Pick it if your team already works with Laravel and wants a solid base to extend.

---

## Stack

| Layer | Technology |
|---|---|
| Framework | **Laravel 12** |
| Language | **PHP 8.2+** |
| Admin panel | **Filament 3** (20 resources + site settings) |
| UI | **Livewire 3** + Blade, Tailwind CSS 4 (typography), Vite 7 |
| Database | **MySQL 5.7 / 8.0 or MariaDB** |
| Roles | spatie/laravel-permission |
| Images | Intervention Image: uploads auto-converted to WebP |
| Documents | PhpWord (DOC / DOCX import), HTML → Markdown conversion |
| Storage | Local or S3-compatible disk, with a migrate-to-S3 command |
| Queue / cache / sessions | Database driver (no extra services) |
| Deployment | Nginx + PHP-FPM (aaPanel guide and Nginx configs included), HTML minification |

---

## Features

### Reader
- Dark / warm modes, font size, 3 font families
- Per-chapter progress saved to the server
- Chapter image gallery with lightbox; scroll position restored between chapters
- **Download as EPUB / FB2 / TXT** (with images and table of contents), with each format switchable by admins

### Catalogue and home page
- Live catalogue filtered by search, tags, status, year, author and country, with sorting and filters kept in the URL
- Updates feed
- **Home-page layout builder**:
  - blocks ranked by views, rating or newest
  - time windows: day, month, all time
  - grid, list or swiper layouts
  - custom HTML banners

### Title page
- Volumes, chapters and release schedule
- Alternative names, original author and source, release year
- Star ratings, favourites, chapter likes, threaded comments

### Author tools
- Author dashboard, novel and chapter editors (rich text or Markdown), per-novel statistics
- **Import:** authors upload TXT / FB2 / DOC / DOCX. Admins can import a ZIP of TXT / MD files, where folders become volumes.
- **Rulate parser** (admin panel and command line)
- **Beta readers**: invite them, collect their notes; they can read locked chapters
- Error / typo reports notify the author and admins
- Scheduled chapters (future publish date set in admin)

### Monetization
- User balance and **paid chapters** (verified email required)
- Per-novel and author-bundle subscriptions (bundle discount 15% by default), approved by an admin
- **Paid promotion packages** (e.g. featured on the home page for a limited time)
- Withdrawal requests, moderated donation links, ad banners
- Top-up by request, confirmed by an admin

### Community
- Threaded comments with likes, commenter badges and backgrounds, spam flags
- Private chat with spam reports
- In-app notifications
- Blog, moderator-recruitment board with applications
- Profiles with banners

### Admin and moderation
- **Filament admin panel**: 20 resources, site settings, roles (super admin, moderator, author), per-user novel limits
- **Separate moderator panel** behind an extra password:
  - pre-moderation of new novels, covers and descriptions
  - publish / unpublish, delete comments
  - spam queue
  - moderated profile edits

### Security and API
- **Scraper blocking** by user-agent fingerprint blocklist
- Per-novel geo-block; 18+ gate (logged-in users only)
- Email verification for paid and 18+ content; signed verification links
- **Public read-only REST API** `/api/v1` (8 endpoints) with a docs page for staff

---

## Size

| Metric | Value |
|---|---|
| Models | 31 |
| Migrations | 60 |
| Controllers | 16 |
| Livewire components | 29 |
| Filament resources | 20 |
| Blade views | ~80 |

---

## Good to know

- **UI language:** Russian, hard-coded in the templates.
- **Payments are manual:** top-ups and subscriptions are confirmed by an admin. A RoboKassa module is in the code but not connected; connecting a gateway is available as custom work.
- **SEO is basic:** meta description and robots.txt. A sitemap, OpenGraph tags and RSS can be added as custom work.
- No read-aloud, PWA, real-time updates, promo codes or early access. For those, look at the higher tiers.
- Search uses simple SQL pattern matching.
- **Tests:** none beyond framework stubs.

---

<div align="center">

**erIIIba · $299**

[Order / ask for a demo](../README.md#how-to-buy) · [Compare platforms](../README.md#compare-platforms)

</div>
