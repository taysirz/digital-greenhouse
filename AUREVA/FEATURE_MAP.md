# AUREVA — feature map and evidence boundaries

This document distinguishes the current 0.1.4 source snapshot from the broader product vision.

| Area | In 0.1.4 source snapshot | Remaining verification / work |
|---|---|---|
| Plant-centred home | Plant-first visual hierarchy and growth components are present | Manual Chrome visual acceptance |
| Browsing activity | Foreground activity and useful-page credit are distinguished | Improve classification transparency and point attribution |
| Zero-points experience | UI explains tracked time versus credited time | The scoring engine is unchanged; eight-hour / zero-points complaint remains open |
| Outside weather | Manual city input and Open-Meteo weather card | Live Chrome lookup and commercial data licensing |
| Care check-ins | Quick care actions are present in source | Validate persistence and refine into meaningful whole-life features |
| Focus / protection | Existing extension components and tests are included | Manual end-to-end Chrome acceptance |
| AI | Provider/client and backend components are present | Verify actual provider config, consent gates and live calls |
| Single-scroll mini-app | 0.1.4 changes to one document-level vertical scroll owner | Manual Chrome check on the user's device |
| Popup CSP | Inline startup removed in favour of external local script | Manual Chrome confirmation |

## How to describe status

Use precise wording:
- **In source:** files and implementation exist in the package.
- **Automated-test passed:** test report covers the relevant path.
- **Manual-tested:** verified in real Chrome.
- **Unverified:** source/test evidence does not establish runtime behaviour.
- **Planned:** product direction only.

Do not describe a roadmap item as an implemented feature.
