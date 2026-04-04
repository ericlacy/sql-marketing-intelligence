# SQL for Marketing Intelligence

**MSMI 698** · University of San Francisco · McLaren School of Management

Two self-contained SQL learning environments for graduate marketing students. No server, no installation, no accounts — open the HTML file in any modern browser and start writing SQL.

## Environments

| Environment | File | Database | Purpose |
|---|---|---|---|
| **SQL Lab** | `SQL_Lab_USF.html` | E-commerce Marketing (6 tables, ~75K rows) | Graded exercises with auto-grading and diagnostic feedback |
| **SQL Lecture** | `SQL_Lecture_Environment.html` | Bay Area Coffee Chain (7 tables, ~60K rows) | In-class instruction with clause-by-clause step cards |

## Quick Start

1. Open either HTML file in Chrome, Firefox, or Safari
2. The database loads in-memory on page open (~2 seconds)
3. Write SQL, press **Ctrl+Enter** to run

Or visit the [live site](https://ericlacy.github.io/sql-marketing-intelligence/) to run both environments directly in your browser.

## Features

- **Tiered mastery**: 19 exercises across 3 tiers (Foundations → AI-Assisted → Full Autonomy)
- **Auto-grading**: Diagnostic feedback on each check — not just pass/fail
- **SQL linter**: Pre-execution warnings for missing GROUP BY, HAVING without GROUP BY, aggregate in WHERE
- **ER diagrams**: Interactive crow's foot notation diagrams embedded in both environments
- **Light/dark mode**: Theme toggle with persistence
- **Zero infrastructure**: Everything runs client-side via sql.js (SQLite compiled to WebAssembly)

## Deliberate Data Quality Issues

Both databases contain seeded data quality issues used as teaching instruments:

| Issue | SQL Lab | Lecture |
|---|---|---|
| Orphan records | 50 orders | 40 transactions |
| NULL values | ~30% discount_applied | ~25% tip_amount |
| Duplicate entries | ~20 customers | ~14 members |
| Date anomaly | Campaign 13 | Promotion 8 |
| Orphan touches | 100 campaign_touches | 80 promo_touches |

## Course Structure

7 weeks · 3 tiers · 7 CLOs · 5 weekly quizzes

- **Tier 1 (Weeks 1–2):** No AI. Hand-write SELECT, WHERE, JOIN queries.
- **Tier 2 (Weeks 3–4):** AI generates SQL. Students diagnose and fix.
- **Tier 3 (Weeks 5–6):** Full AI access with mandatory annotation.
- **Week 7:** Marketing Intelligence Challenge — individual CMO briefing presentations.

## Technology

- [sql.js](https://github.com/sql-js/sql.js/) — SQLite compiled to WebAssembly
- All data generated deterministically in-memory on page load
- localStorage for progress persistence (SQL Lab) and theme preference (both)
- No external dependencies beyond the sql.js CDN

## License

Course materials © 2026 Eric Lacy, University of San Francisco. All rights reserved.
