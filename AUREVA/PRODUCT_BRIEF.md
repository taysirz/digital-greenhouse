# AUREVA — Product brief

**Parent brand:** TOLEVU (`ŦØŁĒṼŪ ✦`)  
**Product:** AUREVA  
**Product origin:** Digital Greenhouse  
**Current packaged snapshot:** 0.1.4  
**Positioning direction:** A living digital companion.

## Core idea

AUREVA is a digital-wellbeing companion designed around the idea that the plant represents the person behind the screen — their inner life, wellbeing and growth. The plant is not merely a productivity mascot, score widget or punishment meter.

The experience should help people care for the whole of life, including both digital behaviour and life away from the screen.

## Product principles

1. The plant is the emotional and visual centre of the product.
2. Real-life wellbeing matters alongside digital habits.
3. Browsing activity should affect points transparently and contextually.
4. Weather refers to the actual outside world, never a person's browsing mood.
5. Supportive prompts should guide users without shame or punishment.
6. Uncertain AI classification must not be presented as fact.
7. Progress should be resilient: a difficult day or a mistaken classification must not erase accumulated growth.

## Product systems

### The plant and care

The plant should be prominent, expressive and visibly responsive to care. The product vision includes care features for areas that can affect a person's wellbeing. Candidate areas include hydration, sleep and rest, movement, outdoor time, learning, creativity, relationships and reflection. Each should have a useful interaction or feature rather than being decorative labels.

### Outside world

The weather card is about real local outdoor conditions. The current prototype uses manually entered city location and Open-Meteo data. It can show current conditions and practical informational cues. It is not an official emergency-alert service and should not replace local authority guidance.

The current Open-Meteo free API offering is non-commercial. A commercial licence/API arrangement or a provider with suitable commercial terms is required before commercial deployment.

### Digital life and points

Browsing should have a visible, explainable relationship with points. Useful/productive browsing may earn points under the existing scoring model; neutral or uncertain browsing should not automatically be rewarded; distracting browsing may trigger supportive interventions. Browsing must not directly injure the plant or erase its progress.

The current 0.1.4 patch does **not** change the scoring engine. In the current implementation, foreground browsing time and time credited as useful are distinct. Only confidently classified useful pages are credited automatically. The manual “Mark useful” control is feedback, not an instant points award or retrospective correction. This is a known usability gap and a priority for future work.

### Digital protection and focus

The source bundle includes Focus and site-protection systems, with settings and deterministic user-configured rules taking priority over uncertain AI inference. Review the implementation and tests before claiming specific behaviour as production-ready.

### AI companion

AI-related components are present in the codebase. AI features must explain what they do and should be described as implemented only when the relevant provider, consent, and runtime behaviour have been verified.

## Product experience

AUREVA's intended feeling is colourful, playful, energetic and deeply human. The home experience should be compact, visually led and easy to understand. Minimise explanatory paragraphs. Use short labels, useful icons, clear status and progressive disclosure.

## Current release boundary

AUREVA 0.1.4 is a development snapshot. The developer preview includes the current extension and backend source, tests, and documentation. Automated checks passed according to the included test report. Manual Chrome acceptance remains required. The 0.1.4 patch fixes CSP-safe popup startup, single-viewport mini-app scrolling and colour-role placement; it does not implement the next-generation points redesign.
