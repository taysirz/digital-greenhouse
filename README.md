Digital Greenhouse 
Grow beyond the screen. Digital Greenhouse is a Chrome extension designed to help people build healthier browsing habits, protect focus time, and make progress on goals through a plant-centred growth system.
> \*\*Release:\*\* 3.3.1 — publisher-configurable beta  
> \*\*Repository scope:\*\* Chrome extension source and client-side tests. The backend source, live service, and private deployment configuration are maintained separately.
What it does
Plant and progress: a persistent growth model, adaptive points, activity goals, safeguards against reward farming, and non-punitive plant health.
Browsing awareness: uses foreground-tab activity and page signals to estimate useful, neutral, or distracting browsing. Page-level corrections can improve future classification; automatic classifications can be wrong.
Focus and protection: strict Focus/Garden Guard access rules, user-defined site rules, ad/tracker filtering rules, and in-page reminders.
In-page experience: popup, mini-app, dashboard, floating plant widget, and extension-styled notifications.
Unified hosted AI: when the publisher has configured a secure backend and the user accepts the disclosed data-sharing consent, one configured hosted model powers the public AI features. Users do not supply provider keys or choose the server's model.
Local-first defaults: local extension features can run without the hosted AI service. Hosted syncing and AI fail closed while the publisher endpoint is blank.
Before you install or share this source
This GitHub source is deliberately not preconfigured with a hosted service URL or provider credentials. `service-config.js` has an empty URL, so it will not upload to localhost or send data to an unknown server. A maintainer must configure the HTTPS service origin and verify the backend before distributing a build that enables hosted AI/data sync.
The backend source and its deployment instructions are not included in this extension-only repository. Do not add backend `.env` files, provider API keys, signing secrets, owner tokens, user data exports, or personal browsing records to GitHub.
Install for local browsing
Download the repository ZIP from GitHub and extract it, or clone the repository.
Open `chrome://extensions` in Chrome.
Turn on Developer mode.
Choose Load unpacked and select this repository folder — the one containing `manifest.json`.
Refresh already-open pages if needed.
The local browsing, growth, and extension UI features can be explored. Hosted AI and remote syncing will not connect until a valid HTTPS service origin is configured.
Publisher configuration
Only configure a backend that you own or are authorized to use, and only after reviewing what its server stores.
From the repository root, use Node.js 20 or later:
```bash
node configure-publisher.cjs https://YOUR-REAL-SERVICE-ORIGIN
```
Use the HTTPS origin only (no path, query, token, or trailing endpoint). The helper rejects plain HTTP and placeholder hosts. The service URL is public configuration, not a secret; provider credentials, signing secrets, and owner-admin tokens must remain in the backend hosting provider's private environment. Re-test the configured build before sharing it.
Important data and AI behavior
Please read this before accepting the in-extension setup consent:
Sharing is all-or-nothing, not a per-category selection. After clear Setup disclosure and explicit consent, the extension automatically enrolls and syncs the complete supported local dataset. That can include routines, progress, settings, feedback, and recorded browser-use signals.
The hosted AI uses the same consent in the public build. Relevant context, which can include page information when page understanding runs, is sent to the configured AI service/provider for processing.
The service operator can access and export the data stored by the backend. Treat collected data and owner exports as private.
Turning consent off stops future syncing and hosted AI once revocation reaches the server. It does not automatically delete data already stored by the server. Existing records require a separate deletion request/process.
The backend bundled with the wider project is beta scaffolding, not an audited, production-grade multi-user data platform. Before broad public use, review access isolation, persistent storage, backups, retention, deletion, abuse limits, privacy disclosures, and applicable rules — especially if minors may use the product.
Never commit personal data exports, API keys, access tokens, signing secrets, or owner credentials.
See `VISION-MAP.md`, `RELEASE-NOTES.md`, and `FINAL-ACCEPTANCE.md` for scope and status.
Development and tests
Requirements: Node.js 20 or later. No external npm dependencies are required for the included tests.
```bash
npm test
```
The included suite covers selected extension/client behavior: AI-content disclosure detection, domain parsing, filter-list validation, growth rewards, browsing reminders/page corrections, core growth UI wiring, AI runtime guards, and publisher URL validation. Backend authentication/data-store tests are maintained with the separate backend source and are not included here.
Passing tests do not establish that every feature works on every website, that the deployed AI provider is reachable, or that the backend is production-ready. This source package does not claim to have completed independent live-browser acceptance.
Permissions
The manifest requests Chrome permissions for storage, tabs/navigation, alarms, idle detection, script injection, network-request rules, and access to HTTP/HTTPS pages. These powers support browsing-awareness, blocking, page-context features, and the in-page UI. Review the source and the in-extension disclosure before use.
Project status
Publisher-configurable beta, not a finished production service. The extension source and selected automated tests are public-ready for review; hosted AI/data syncing requires separately configured backend infrastructure and careful real-environment verification.
License
No license is included yet. Public visibility on GitHub does not automatically grant permission to reuse, modify, or redistribute this code. Add a license before inviting reuse or outside contributions under specific
