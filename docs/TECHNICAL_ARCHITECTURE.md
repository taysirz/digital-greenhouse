# Technical architecture — AUREVA 0.1.4

## Source package

The current editable source snapshot is included at `releases/AUREVA_0.1.4_Developer_Preview.zip`. Its archive structure contains:
- `extension/` — Manifest V3 Chrome extension.
- `backend/` — Node.js service and dashboards.
- automated tests for both components;
- release notes, security notes and configuration documentation.

The Chrome-installable source package is `releases/AUREVA_0.1.4_Chrome_Ready.zip`.

## Extension

The extension uses Manifest V3 and JavaScript, HTML, CSS and JSON. Main areas include:
- background/service worker and browser event handling;
- popup and mini-app;
- full dashboard and persistent widget;
- activity collection and domain utilities;
- growth/points engine;
- Focus and site protection;
- AI/provider client components;
- local settings and privacy/consent handling;
- automated tests.

The 0.1.4 patch moves dashboard query-mode setup into external `view-mode.js` to comply with extension Content Security Policy. The full-tab mini-app uses the document viewport as its single vertical scrolling surface.

## Backend

The source archive contains a Node.js backend, storage layer, user and owner dashboards, analytics/progress modules, AI-provider routes and tests. Read `backend/README.md` and `backend/RENDER-SETTINGS.txt` inside the archive before running it.

Do not assume that a source package means a hosted deployment is current or operational. Deployment, database migration/restore, real provider calls and production security require separate verification.

## Weather integration

The current weather prototype uses Open-Meteo geocoding and forecast endpoints. The user manually enters a city; the extension does not request precise GPS location for this feature. An internet connection is required. The provider attribution is shown in the interface. The free API offering is non-commercial, so commercial launch requires suitable commercial access or a different provider.

## Trust boundaries

- AI classification is probabilistic; it must not silently override deterministic user-configured protection rules.
- Unknown/low-confidence browsing should remain visibly unclassified or neutral.
- Avoid publishing credentials, generated access tokens, live environment files, database exports or user data.
- Keep backend secrets in hosting environment configuration.
- Treat automated tests as evidence for tested code paths, not as proof of production readiness.
