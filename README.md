| [banner.html](https://imageworksc.github.io/silk-vision/banner.html) | Same bands, but the block on the right bleeds off the edge of the window and reads as a banner |# Silk Vision — Navigation

Three versions of a mega-menu navigation for [silkvision.net](https://www.silkvision.net/),
built from the practice's own colours, type and photography.

| Page | Panels |
| --- | --- |
| [index.html](https://imageworksc.github.io/silk-vision/) | Panels hang under their trigger as cards |
| [full-width.html](https://imageworksc.github.io/silk-vision/full-width.html) | Panels are bands across the window; contents held to the header column; the promo is a block beside the items |
| [banner.html](https://imageworksc.github.io/silk-vision/banner.html) | Same bands, but the promo breaks out of the column and runs as a full-bleed banner under the items |

## Shared design

| Token | Value | Used for |
| --- | --- | --- |
| Brand blue | `#005894` / `#00365d` | Nav, item names, icons |
| Purple | `#800080` | Actions only, never decoration |
| Mist / hairline | `#f2f7fb` / `#dbe7f1` | Hover wash, rules |
| Type | Montserrat (nav, headings), Poppins (body) | |
| Container | `1400px` / `max-width: 93%` | Matches the site grid |

Every procedure row carries the one fact that separates it from the row above, and each
row has an outline icon drawn from the anatomy or object involved. All CSS is scoped to
`#sv-header-wrap` / `.sv-*`, so any of the three can be dropped into the live theme.

## Files

- `index.html`, `full-width.html`, `banner.html` — one self-contained page each
- `assets/` — logo and the photographs used in the panels
