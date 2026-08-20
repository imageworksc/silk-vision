# Silk Vision — Navigation Redesign

Mega-menu navigation for [silkvision.net](https://www.silkvision.net/), rebuilt in the
production design language and published with GitHub Pages.

| Page | What it shows |
| --- | --- |
| [`index.html`](./index.html) | The live homepage with the redesigned navigation dropped in, replacing the legacy Drupal header. |
| [`menu.html`](./menu.html) | The navigation on its own, with the design tokens it was built from. |
| [`nav-prototype.html`](./nav-prototype.html) | The original `silk vision menu 08-19` comp, kept for reference. |

## Design tokens (pulled from the production stylesheet)

| Token | Value | Used for |
| --- | --- | --- |
| Brand blue | `#005894` / `#005895` | Nav links, panel headings, outlined Contact button |
| Utility blue | `#106096` | Top bar text |
| Purple gradient | `#800080` → `#5f005f` | Top-bar CTA, panel CTAs |
| Body | `#45575b` | Panel copy, panel border |
| Rules | `#ccc`, `#bcc4c6` | Header rule, column dividers, utility separators |
| Type | Montserrat (nav + headings), Poppins (body) | |
| Container | `1400px` / `max-width: 93%` | Matches the site grid |

## Structure

Four dropdowns, all wired to live silkvision.net URLs:

- **Vision Correction** — two columns (LASIK & Laser / Lens Options) plus a Self-Test CTA
- **Eye Care** — two columns (Cataract & Lens Care / Conditions We Treat) plus an Ask Our Team CTA
- **About** — single column, practice and doctor pages
- **Patients** — single column, right-aligned panel, plus a Book a Consultation CTA

## Behaviour

- Opens on hover at ≥1024px, with an invisible bridge so the pointer survives the gap to the panel
- Click also toggles, `Escape` and outside-click close, `aria-expanded` tracked on every trigger
- Below 1024px the bar collapses to a hamburger and the panels become accordions
- Header is sticky; honours `prefers-reduced-motion`
- All CSS is scoped to `#sv-header-wrap` / `.sv-*` so it never collides with the legacy theme

`assets/` holds the mirrored homepage files (images, CSS, JS) needed by `index.html`.
