# TOLEVU × AUREVA

**ŦØŁĒṼŪ ✦ — Illuminate the Everyday.**

This repository preserves the TOLEVU parent-brand foundation and the AUREVA product project, including the current extension and backend source snapshot, product philosophy, brand system, engineering notes, test evidence, release instructions and Digital Greenhouse project history.

## Current snapshot

- **Product:** AUREVA
- **Release snapshot:** 0.1.4
- **Parent brand:** TOLEVU
- **Current source bundle:** [AUREVA 0.1.4 Developer Preview](releases/AUREVA_0.1.4_Developer_Preview.zip)
- **Chrome package:** [AUREVA 0.1.4 Chrome Ready](releases/AUREVA_0.1.4_Chrome_Ready.zip)
- **Status:** Development snapshot. Automated tests passed; manual acceptance in a real Chrome profile remains outstanding.

The developer preview archive contains the editable extension source, Node.js backend source, tests, documentation and configuration examples. It is the complete source snapshot for this release, not a claim that every planned product capability is already implemented.

## Start here

1. Read [TOLEVU brand foundation](TOLEVU.md).
2. Read the [AUREVA product brief](AUREVA/PRODUCT_BRIEF.md).
3. Review the [product roadmap and implementation status](AUREVA/ROADMAP.md).
4. Read the [technical architecture](docs/TECHNICAL_ARCHITECTURE.md).
5. Download the [developer source bundle](releases/AUREVA_0.1.4_Developer_Preview.zip) and follow its `AUREVA_0.1.4_START_HERE.md`.
6. Check [security and privacy guidance](SECURITY.md) before running or deploying the backend.

## Brand architecture

- **TOLEVU** is the parent brand. Its identity brings together technology, nature, luxury, light and enlightenment.
- **AUREVA** is TOLEVU's digital-wellbeing companion: the reimagined Digital Greenhouse, centred on a plant that represents the person behind the screen.

These are related identities, not the same visual system. Do not assume a final TOLEVU colour palette has been approved. AUREVA's editable palette and current colour-role mapping are documented separately.

## Repository map

- `TOLEVU.md` — parent-brand foundation and known decisions.
- `AUREVA/` — product brief, design system and roadmap.
- `docs/` — technical architecture, history and brand architecture.
- `releases/` — versioned source and installable package archives.
- `archive/` — historical Digital Greenhouse material where retained.
- Existing legacy files from the original Digital Greenhouse repository are preserved until their archive migration is completed.

## Honest status

AUREVA inherits substantial design and engineering work from Digital Greenhouse. The original Digital Greenhouse project did not reach its intended dependable product outcome; it should not be represented as a successful finished product. AUREVA 0.1.4 is a new, editable development snapshot and still requires hands-on Chrome acceptance and follow-up work on browsing-point attribution.

## Security and licensing

Never commit API keys, signing secrets, owner credentials, generated access tokens, production environment files, or real user data. See [SECURITY.md](SECURITY.md).

No open-source licence has been selected. Public visibility is not permission to reuse, redistribute, or commercialise this code. See [LICENCE STATUS](LICENCE_STATUS.md).
