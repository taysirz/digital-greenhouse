# AUREVA — Design system

**Status:** Editable working system; not a final brand lock.

## Personality

Colourful, playful, energetic and deeply human. The plant should be the visual protagonist. The interface should be visually rich but not wordy or cluttered.

## Current editable palette

The active tokens are defined in `extension/aureva-refresh.css` inside the developer preview archive.

| Token | Hex | Current role |
|---|---|---|
| `--ar-bg` | `#F4EBDD` | Warm light canvas |
| `--ar-card` | `#FFF7EA` | Primary card |
| `--ar-card-2` | `#EDE0CC` | Secondary surface |
| `--ar-ink` | `#302547` | Main text |
| `--ar-plum` | `#302447` | Plant hero depth |
| `--ar-violet` | `#7556CF` | Actions and active UI |
| `--ar-lavender` | `#C4B3F0` | Growth and soft accents |
| `--ar-coral` | `#FF8878` | Warm energy accent |
| `--ar-sun` | `#FFD06C` | Light and achievement |
| `--ar-sky` | `#A9DDE6` | Outside-weather accent |
| `--ar-mint` | `#9ED7C3` | Care and vitality |

## Surface roles

- Plant hero: plum/violet depth, with lavender light and champagne-style highlights.
- Outside weather: sky/mint and soft lavender.
- Digital life and browsing status: warm cream with lavender/periwinkle signals.
- Care actions: restrained individual pastel cues.
- Page and card surfaces: warm ivory and beige.

The 0.1.4 visual refinement keeps the established token values and changes their placement/hierarchy. See `extension/aureva-polish.css` in the source archive.

## Layout rules

- Make the plant dominant on the home screen.
- Keep labels short and minimise paragraphs.
- Make the primary status and next action visible without scrolling where practical.
- Use one vertical scrolling surface in the full-tab mini-app.
- Avoid nested scroll containers.
- Keep popup, mini-app, dashboard, widget and blocked page visually coherent.
- Preserve accessible contrast, keyboard focus and reduced-motion support.
- Never communicate status through colour alone.

## Current limitations

The visual direction remains editable. Live Chrome visual acceptance of 0.1.4 has not yet been recorded in the included test report.
