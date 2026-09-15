# Architecture

- `src/main.js`: application state, calculations, natural-language parsing, UI rendering, backup/restore, sharing, and rate lookup.
- `src/styles.css`: responsive Apple-inspired dark interface and iOS safe-area handling.
- `public/manifest.webmanifest`: installable PWA metadata.
- `public/sw.js`: app-shell caching and offline fallback.
- `.github/workflows/deploy-pages.yml`: repeatable GitHub Pages deployment.

## Data model
Each trip contains a base currency, members, exchange rates, rate metadata, and expenses. Each expense identifies the payer and included members. Settlement minimization nets each member's amount paid against their allocated share, then matches debtors with creditors.

## Privacy
All application data is browser-local. There is no account system or backend. The exchange-rate lookup sends only currency codes and a date to the public rate endpoint.
