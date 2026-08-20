# Silk Vision — Navigation

Mega-menu navigation for [silkvision.net](https://www.silkvision.net/), rebuilt in the
production design language. The published page is the menu and the logo, nothing else.

**Live:** https://imageworksc.github.io/silk-vision/

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
- All CSS is scoped to `#sv-header-wrap` / `.sv-*`, so the block can be dropped into the live
  theme without colliding with it

## Files

- `index.html` — the whole component: markup, scoped CSS and script in one file
- `assets/logo.png` — the site logo
