# SupportNow · Family Advocacy (Phase 1 prototype)

Landing page and intake forms for **Family Advocacy**, the part of **SupportNow, the Official Family Support Platform** that connects families raising children with disabilities to advocates who have been there.

**Live preview:** https://supportnow-org.github.io/family-advocacy/

## Pages
- `index.html` — landing page (value prop, how it works, areas of support, for advocates)
- `family-intake.html` — "Find an Advocate" intake for families *(brand blue)*
- `advocate-intake.html` — "Signup as Advocate" intake for advocates, existing + prospective *(green)*

## Notes
- Static prototype: HTML + Bootstrap 5.3 + DM Sans + Font Awesome, all via CDN. Open `index.html` directly or serve the folder.
- Color system: family-facing = SupportNow blue, advocate-facing = green.
- Both intake forms submit to [Formspree](https://formspree.io) via `fetch` (AJAX), so the in-page success panel is preserved instead of redirecting. Endpoints: family → `mkolqapa`, advocate → `mgojnbpd`. Contact fields carry `autocomplete` attributes for browser autofill, plus a hidden `_subject` and a `_gotcha` honeypot for spam.
- Next step: add the "while you wait" confirmation pages.
