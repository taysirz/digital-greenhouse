# AUREVA — Roadmap and implementation status

This roadmap separates what is present in the 0.1.4 source snapshot from the intended product direction. A planned feature is not automatically implemented.

## Current snapshot: 0.1.4

### Included in source snapshot

- Chrome extension popup, mini-app, dashboard, widget and blocked-page surfaces.
- Local tracking, point/growth engine and related tests.
- Focus and website-protection components.
- AI integration components and backend routes.
- Manual-city real-world weather card using Open-Meteo.
- Warm editable palette and plant-first visual hierarchy.
- CSP-safe popup initialisation.
- Single document viewport as the mini-app's vertical scroll owner.
- Automated test suite; see `AUREVA_0.1.4_TEST_RESULTS.md`.

### Verification still required

- Manual Chrome acceptance of CSP behaviour, single-scrollbar behaviour and colour placement.
- Live weather lookup/refresh in the user's Chrome profile.
- Real deployment, production environment, provider configuration and backend security review.
- End-to-end confirmation of AI consent and runtime behaviour.

## Priority 1 — Browsing points clarity

The user reported using AUREVA for around eight hours and seeing zero points. The interface must never leave the user unable to distinguish:
- time observed in an active foreground tab;
- time confidently classified as useful;
- time that remains neutral or uncertain;
- points actually awarded;
- the reason no points were awarded.

Improve classification and feedback without inventing points. Consider review/correction flows that can appropriately re-evaluate a time segment, with clear safeguards against point farming. The 0.1.4 scoring engine is unchanged.

## Priority 2 — Plant as the centre

Make the plant the main visual and emotional anchor. Give it expressive growth states and meaningful responses to care. It represents the person, not a disposable productivity score.

## Priority 3 — Whole-life care features

Develop real interactions for the wellbeing areas that can affect a person's life, such as:
- hydration;
- rest and sleep routines;
- movement and physical activity;
- time outdoors;
- learning and reading;
- creativity and hobbies;
- connection and relationships;
- reflection and emotional wellbeing.

These are candidate product areas, not a claim that every one is currently implemented. Use supportive language and avoid health diagnosis or guilt mechanics.

## Priority 4 — Real outside conditions

Expand the real-weather card only with reliable, appropriately licensed data. Show local conditions and practical guidance. Weather tips must remain informational and should not be represented as official emergency warnings.

## Priority 5 — Visual and interaction polish

Keep AUREVA colourful, playful and energetic, with minimal words, one obvious scroll surface and clear colour roles. Preserve the plant-first layout across extension surfaces.

## Priority 6 — Release and operations readiness

- Complete manual Chrome testing.
- Verify supported Chrome version and permissions.
- Review backend secrets, authentication and deployment configuration.
- Confirm data minimisation, consent, export and deletion behaviour.
- Confirm commercial weather-data terms.
- Create a release checklist and publish only what is verified.
