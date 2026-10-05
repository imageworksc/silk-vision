# Silk Vision — Navigation

Four versions of a mega-menu navigation for [silkvision.net](https://www.silkvision.net/),
built from the practice's own colours, type and photography.

| Page | Panels |
| --- | --- |
| [index.html](https://imageworksc.github.io/silk-vision/) | Panels hang under their trigger as cards; each row has a one-line description |
| [simple.html](https://imageworksc.github.io/silk-vision/simple.html) | Same as index, with the descriptions removed |
| [full-width.html](https://imageworksc.github.io/silk-vision/full-width.html) | Floating panels up to 1500px wide; items in the header's column, photo block on the right set off by a hairline |
| [banner.html](https://imageworksc.github.io/silk-vision/banner.html) | Floating panels; the photo block runs flush to the panel's edges on a soft tint |

## Shared design

| Token | Value | Used for |
| --- | --- | --- |
| Brand blue | `#005894` / `#00365d` | Nav, item names |
| Purple | `#800080` | Actions only, never decoration |
| Mist / hairline | `#f2f7fb` / `#dbe7f1` | Hover wash, rules |
| Type | Montserrat (nav, headings), Poppins (body) | |
| Container | `1400px` / `max-width: 93%` | Matches the site grid |

All CSS is scoped to `#sv-header-wrap` / `.sv-*`, so any version can be dropped into the
live theme. Each file starts with the same shared rules; full-width and banner add one
section of their own at the end.

## Breakpoints

| Width | Behaviour |
| --- | --- |
| up to 1023px | Burger menu, panels open inline as an accordion |
| 1024px and up | Desktop menu, panels open on hover or click |
| 2400px and up | The whole header scales up in steps (1.25× to 2.67× at 5120px), so 4K and 5K screens at 100% scaling see it at its 1920px proportions |

## Files

- `index.html`, `simple.html`, `full-width.html`, `banner.html` — one self-contained page each
- `assets/` — logo and the photographs used in the panels
