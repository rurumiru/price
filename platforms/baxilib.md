<div align="center">

# Baxilib

### Russian web-novel platform with teams, passes and payouts, on a private engine

**$939** · one-time license · Russian UI (+ English switch) · 🔒 secret stack

[← Back to the price list](../README.md)

</div>

---

## In one paragraph

Baxilib is a platform for reading and publishing light novels, web novels and original stories for Russian-speaking readers. It is the sister of [Dragons Heaven](dragons-heaven.md) on the same **private XI engine**, and it adds what Dragons Heaven leaves out:
- **translation teams** with three access levels
- **monthly passes** for a novel
- **author payouts**
- **handover of abandoned translations** to people who will finish them

Like Dragons Heaven, it needs nothing besides PostgreSQL: background jobs, full-text search and counters all run inside the database. It ships with 204 automated test files.

---

## Stack

| Layer | Technology |
|---|---|
| Application engine | 🔒 **Classified**: private XI engine, disclosed to the buyer under NDA |
| Database | **PostgreSQL 17**: balances and counters enforced by triggers and CHECK constraints; keyset pagination everywhere |
| Search | Built into PostgreSQL: full-text index (Russian + simple), so English titles are found too |
| Background jobs | Built in, stored in PostgreSQL (21 workers) |
| External services | **None required**: no Redis, no search server, no message broker |
| Storage | Local disk or any S3-compatible bucket |
| Frontend | Tailwind CSS 4, own design system |
| PWA | Installable app, offline page, chapters saved for offline reading |
| Mail | SMTP or Mailgun |
| Deployment | **Docker** image + Docker Compose, health-check endpoints, aaPanel / Nginx guide |
| Minimum server | 2 vCPU / 4 GB RAM / 20 GB disk |

---

## Features

### Reader
- 5 surfaces (Night, Sepia, Paper, Grey, OLED), font, size, line spacing, width, justify, hyphenation
- Reader settings stored in the account; server-side reading progress
- **Read aloud** with adjustable speed
- Bookmarks that keep the quote, the paragraph and your note
- **Offline reading**: save chapters to the device
- **Download as EPUB / FB2 / TXT**

### Catalogue and discovery
- Catalogue filters, genre pages, instant search suggestions
- **Full-text search**
- Top lists by period with time decay, all-time score
- Reader-made lists, "similar novels", followers

### Title page and community
- Comments with reactions; reviews with likes; 1–10 ratings, shown after 5 votes
- Private messages with user blocking
- **XP ledger, levels and badges**
- Blog, **support tickets** with staff replies and internal notes
- Weekly email digest, live in-app notifications, **web push**

### Translator studio
- Visual editor plus a markup mode, live preview, pasted images
- **Scheduled publishing**
- Chapter import from TXT / MD, or ZIP with images (UTF-8 and CP1251), saved as drafts
- **Beta readers** for drafts; typo reports that quote the exact text
- Author statistics

### Teams and handover
- **Translation teams** with three nested access levels per title: proofreader → translator → editor. Money, deletion and transfer stay with the owner.
- **Abandoned-translation takeover**:
  1. After a long silence, an established reader can claim the title.
  2. The owner has a window to object; objections go to moderators.
  3. Earnings from chapters that were already published stay with the original translator.

### Monetization
- Coin wallet on a ledger, with overdraft blocked by the database; paid chapters with an author share (70% by default)
- **Early access**: a chapter price plus a "free after" date
- **Monthly pass per novel**: the owner sets the price, with auto-renew
- **Promo codes** that grant coins, chapters, pass days or a badge
- Donations, **paid novel promotion**, refunds
- **Author payouts**: coins are held when a request is made, then an admin approves it
- Payment gateways: Robokassa, PayAnyWay, Tribute (card, SBP, Telegram Stars). Manual top-up with admin approval works out of the box.

### Admin and moderation
- About 30 admin screens, including background jobs, monitoring and imports
- Reports, sanctions and **appeals**, audit log
- **Copyright claims with counter-notices**
- Three registration modes: open, closed or **by application** (the default)
- 18+ gate, per-country blocking, maintenance mode

### SEO
- Sitemap index, OpenGraph / Twitter cards, **JSON-LD**
- Atom feed, **IndexNow** (instant search-engine pings)
- **OPDS catalogue** for e-reader apps

### Security and privacy
- Visible session list, one-time recovery codes
- Copy protection on paid text
- Personal data export and account deletion

---

## Size

| Metric | Value |
|---|---|
| Migrations | 133 |
| Database tables | ~74 |
| Routes | ~140 |
| Background workers | 21 |
| Automated tests | **204 test files** |

---

## Good to know

- **UI language:** Russian. An English switch is built in, with about 80% of interface strings translated.
- **Off by default, switch on when ready:**
  - translation teams and title takeover
  - author payouts
  - payment gateways: real integrations that ship in test mode, so add your merchant keys
- **Needs your keys:**
  - social login (VK, Google, Yandex, Telegram)
  - email (SMTP / Mailgun)
  - web push (VAPID)
  - Telegram / VK channel digests
- **Imports:**
  - The Rulate importer needs a logged-in Rulate session.
  - The legacy database importer was written for one previous site, so it is adapted per project.
- WordPress import is not included.

---

<div align="center">

**Baxilib · $939**

[Order / ask for a demo](../README.md#how-to-buy) · [Compare platforms](../README.md#compare-platforms)

</div>
