<div align="center">

# XI PROJECTS

### Commercial CMS for Web Novels, Light Novels & Translation Platforms

**A production-ready platform for launching modern web novel and light novel services.**

Catalog • Reader • Releases • Teams • SEO • Admin Panel • API • PostgreSQL

<br>

![License](https://img.shields.io/badge/license-commercial-111111?style=for-the-badge)
![Database](https://img.shields.io/badge/database-PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Type](https://img.shields.io/badge/product-Web%20Novel%20CMS-7c3aed?style=for-the-badge)
![Status](https://img.shields.io/badge/status-available-16a34a?style=for-the-badge)

<br>

[Overview](#overview) •
[Packages](#packages) •
[Features](#features) •
[Architecture](#architecture) •
[Pricing](#pricing) •
[License](#license)

</div>

---

# Overview

**XI Projects** is a commercial CMS ecosystem designed specifically for:

- Web novels
- Light novels
- Original fiction
- Translation teams
- Publishing groups
- Multi-author platforms
- Private novel communities
- Commercial reading platforms

Unlike generic blogging engines, XI Projects is built around the actual structure of serialized fiction.

```text
Novel
  ↓
Volumes
  ↓
Chapters
  ↓
Releases
  ↓
Readers
```

Every package uses **PostgreSQL** as the primary database.

The main CMS functionality is the same across all packages.

You are choosing the **technology stack and architecture**, not unlocking features through artificial pricing tiers.

---

# Packages

| Package | Stack | Database | Price |
|---|---|---|---:|
| **Started Pack** | Yii 1 / Yii 2 | PostgreSQL | **$399** |
| **Medium Pack** | Next.js stack | PostgreSQL | **$499** |
| **Large Pack** | Laravel stack | PostgreSQL | **$599** |
| **Boost Pack** | Private Engine | PostgreSQL | **$939** |

> All packages include the same core CMS functionality.

---

## Started Pack

### `$399`

A reliable and lightweight implementation built around the Yii ecosystem.

**Stack**

```text
Yii 1 / Yii 2
PHP
PostgreSQL
Redis-ready architecture
Nginx / Caddy
```

Suitable for:

- Translation teams
- Private libraries
- Smaller commercial projects
- Low-cost VPS deployments
- Projects where resource efficiency matters

The Started Pack provides the full XI Projects CMS feature set without requiring an unnecessarily heavy infrastructure stack.

---

## Medium Pack

### `$499`

A modern implementation focused on frontend performance, API integrations and scalable web architecture.

**Stack**

```text
Next.js
React
API Layer
SSR / ISR
PostgreSQL
Redis-ready architecture
```

Suitable for:

- Modern novel platforms
- Commercial projects
- API-oriented systems
- Projects focused on frontend performance
- Platforms planning future scaling

The Medium Pack is intended for teams that prefer a modern JavaScript frontend stack while retaining the full XI Projects publishing ecosystem.

---

## Large Pack

### `$599`

A flexible commercial implementation built around the Laravel ecosystem.

**Stack**

```text
Laravel
PHP
API
Queue Workers
Background Jobs
PostgreSQL
Redis-ready architecture
```

Suitable for:

- Commercial platforms
- Projects requiring external integrations
- Advanced backend workflows
- Background processing
- Automation
- Custom business logic

The Large Pack is designed for projects that expect deeper backend customization and extensive integrations.

---

## Boost Pack

### `$939`

The highest-tier XI Projects implementation, based on a private proprietary engine.

**Stack**

```text
Private XI Engine
High-performance backend
API-first architecture
PostgreSQL
Advanced caching
Queue processing
Custom infrastructure options
```

Suitable for:

- Large platforms
- High-load projects
- Custom infrastructure
- Advanced deployment scenarios
- Projects requiring deeper architectural flexibility

The Boost Pack uses a private XI Projects engine that is not distributed publicly.

---

# Same Functionality Across All Packs

XI Projects does **not** split basic functionality into artificial feature tiers.

Every package includes the same core platform functionality.

| Feature | Started | Medium | Large | Boost |
|---|:---:|:---:|:---:|:---:|
| Novel Catalog | ✅ | ✅ | ✅ | ✅ |
| Reader | ✅ | ✅ | ✅ | ✅ |
| Admin Panel | ✅ | ✅ | ✅ | ✅ |
| PostgreSQL | ✅ | ✅ | ✅ | ✅ |
| User Accounts | ✅ | ✅ | ✅ | ✅ |
| Roles & Permissions | ✅ | ✅ | ✅ | ✅ |
| Translation Teams | ✅ | ✅ | ✅ | ✅ |
| Volume Management | ✅ | ✅ | ✅ | ✅ |
| Chapter Management | ✅ | ✅ | ✅ | ✅ |
| Release System | ✅ | ✅ | ✅ | ✅ |
| Genres & Tags | ✅ | ✅ | ✅ | ✅ |
| Ratings | ✅ | ✅ | ✅ | ✅ |
| Reading History | ✅ | ✅ | ✅ | ✅ |
| Bookmarks | ✅ | ✅ | ✅ | ✅ |
| Responsive UI | ✅ | ✅ | ✅ | ✅ |
| SEO | ✅ | ✅ | ✅ | ✅ |
| API Support | ✅ | ✅ | ✅ | ✅ |
| Media Management | ✅ | ✅ | ✅ | ✅ |
| Moderation Tools | ✅ | ✅ | ✅ | ✅ |

The difference between packages is primarily:

- Framework
- Runtime architecture
- Deployment approach
- Customization flexibility
- Scaling strategy

---

# Features

## Novel Management

Create and manage complete serialized fiction projects.

Supported entities include:

- Novels
- Light novels
- Web novels
- Volumes
- Chapters
- Side stories
- Alternative titles
- Authors
- Artists
- Translators
- Editors
- Genres
- Tags
- Publication statuses
- Age ratings
- Covers
- Descriptions
- Metadata

Example structure:

```text
Novel
├── Volume 1
│   ├── Chapter 1
│   ├── Chapter 2
│   └── Chapter 3
│
├── Volume 2
│   ├── Chapter 4
│   └── Chapter 5
│
└── Side Stories
    ├── Side Story 1
    └── Side Story 2
```

---

## Modern Reader

The built-in reader is designed specifically for long-form fiction.

Available functionality can include:

- Typography customization
- Font size settings
- Reading width settings
- Light theme
- Dark theme
- Chapter navigation
- Reading history
- Reading progress
- Bookmarks
- Mobile reading
- Keyboard navigation
- Responsive layout
- Reader preferences

The reader is optimized for both desktop and mobile usage.

---

## Advanced Catalog

Readers can discover titles through a structured catalog.

Supported discovery tools include:

- Genres
- Tags
- Publication status
- Popularity
- Recently updated
- New releases
- Ratings
- Alphabetical sorting
- Advanced filters
- Full-text search

---

## Translation Teams

XI Projects can be used by multi-user translation and publishing teams.

Typical roles include:

```text
Administrator
Project Manager
Translator
Editor
Proofreader
Author
Publisher
Moderator
```

Projects can be assigned to:

- Teams
- Individual translators
- Editors
- Proofreaders
- Project managers

This allows a publishing workflow to be organized directly inside the CMS.

---

## Administration Panel

The administration panel provides centralized control over the entire platform.

Administrators can manage:

- Users
- Novels
- Volumes
- Chapters
- Teams
- Releases
- Reports
- Comments
- Moderation
- Media
- Permissions
- Roles
- SEO
- Platform settings
- System configuration

---

## SEO

XI Projects is designed for search-friendly publishing.

Supported SEO architecture may include:

- SEO-friendly URLs
- Meta titles
- Meta descriptions
- OpenGraph metadata
- Canonical URLs
- Structured metadata
- Sitemap generation
- robots.txt configuration
- Server-side rendering where supported

Example URLs:

```text
/novel/shadow-slave
/novel/shadow-slave/volume-3
/novel/shadow-slave/chapter-184
```

---

## Responsive Design

XI Projects is designed for:

```text
Desktop
Laptop
Tablet
Mobile
```

Reader pages are optimized for long reading sessions and small screens.

---

# PostgreSQL

Every XI Projects package uses **PostgreSQL**.

```text
Started Pack  → PostgreSQL
Medium Pack   → PostgreSQL
Large Pack    → PostgreSQL
Boost Pack    → PostgreSQL
```

PostgreSQL is used as the primary relational database for:

- User accounts
- Titles
- Volumes
- Chapters
- Teams
- Roles
- Permissions
- Reader progress
- Bookmarks
- Ratings
- Metadata
- Releases
- Platform configuration

Depending on the project, PostgreSQL can be combined with:

- Redis
- S3-compatible object storage
- CDN
- Queue workers
- Search services
- Backup infrastructure

---

# Architecture

XI Projects can be deployed using different application architectures while retaining PostgreSQL as the central database layer.

```text
┌───────────────────────────────┐
│           FRONTEND            │
│                               │
│ Catalog / Reader / Profiles   │
└───────────────┬───────────────┘
                │
                ▼
┌───────────────────────────────┐
│             API               │
├───────────────────────────────┤
│ Novels                        │
│ Chapters                      │
│ Users                         │
│ Teams                         │
│ Search                        │
│ Administration                │
│ Releases                      │
└───────────────┬───────────────┘
                │
                ▼
┌───────────────────────────────┐
│          PostgreSQL           │
├───────────────────────────────┤
│ Users                         │
│ Novels                        │
│ Chapters                      │
│ Teams                         │
│ Metadata                      │
│ Reader Data                   │
└───────────────┬───────────────┘
                │
                ▼
        Cache / Storage / CDN
```

---

# Built for Novels, Not Blogs

XI Projects is not a generic blog CMS with a novel theme added on top.

The data model, administration interface and reader workflow are designed around serialized fiction from the beginning.

Typical publishing workflow:

```text
Create Novel
     ↓
Create Volume
     ↓
Upload Chapters
     ↓
Assign Team
     ↓
Edit / Proofread
     ↓
Publish Release
     ↓
Reader receives update
```

---

# Deployment

Depending on the selected package and project requirements, XI Projects can be deployed with:

- Linux VPS
- Dedicated server
- Docker
- Nginx
- Caddy
- Cloudflare
- PostgreSQL
- Redis
- S3-compatible storage
- CDN infrastructure
- Reverse proxy architecture
- Queue workers
- Backup infrastructure

---

# Pricing

<div align="center">

| Package | Technology | Price |
|---|---|---:|
| **Started Pack** | Yii 1 / Yii 2 + PostgreSQL | **$399** |
| **Medium Pack** | Next.js + PostgreSQL | **$499** |
| **Large Pack** | Laravel + PostgreSQL | **$599** |
| **Boost Pack** | Private Engine + PostgreSQL | **$939** |

### One-time commercial license

**No mandatory monthly CMS subscription.**

</div>

---

# Optional Services

Additional services can be ordered separately.

Examples:

- Custom UI / UX
- Custom frontend
- Custom reader design
- Migration from another CMS
- Infrastructure setup
- API development
- External integrations
- Discord integration
- Payment integration
- CDN configuration
- Cloudflare configuration
- PostgreSQL migration
- Database optimization
- Backup configuration
- Branding
- Deployment
- Server configuration
- Performance optimization
- Custom feature development

---

# Who Is XI Projects For?

## Translation Teams

Manage multiple titles, translators, editors and releases from one centralized platform.

## Publishers

Launch a branded publishing platform using your own domain and infrastructure.

## Authors

Publish serialized fiction through a platform specifically designed for chapters, volumes and releases.

## Communities

Create a centralized platform for readers, translators, editors and contributors.

## Startups

Launch a web novel service without spending months rebuilding basic publishing infrastructure from zero.

---

# Demo

A demonstration environment can be provided before purchase.

The demo may include access to:

```text
✓ Homepage
✓ Catalog
✓ Novel Page
✓ Reader
✓ User Profile
✓ Admin Panel
✓ Mobile Version
```

The internal source code and architecture of the **Boost Pack** private engine are not publicly exposed.

---

# License

XI Projects is commercial proprietary software.

A purchased license grants usage rights according to the selected agreement.

Unless explicitly permitted by contract, the following are prohibited:

- Redistribution
- Resale of source code
- Public source publication
- Unauthorized sublicensing
- Removal of licensing restrictions

Custom commercial agreements may be discussed separately.

---

# Purchase

For licensing, demonstrations, custom development or integration requests:

```text
Email:    rumisaca@gmail.com
Discord:  exseiba
Telegram: @licht_re
```

---

<div align="center">

# XI PROJECTS

### Build the library.  
### Publish the story.  
### Own the platform.

**Commercial infrastructure for modern web fiction.**

</div>
