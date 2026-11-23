# tvt logo

The mark is four bars under a dashed threshold. Only the orange bar went past
it, and its cut-off top is shown as an outline: tvt finds what nobody reads and
trims it, while everything that's used stays. The wordmark is drawn as shapes,
not set in a font, so it renders the same everywhere.

| File | Use |
| --- | --- |
| `tvt-logo-dark.svg` | Horizontal logo on dark backgrounds (the default) |
| `tvt-logo-light.svg` | Horizontal logo on light backgrounds |
| `tvt-logo-stacked-dark.svg`, `tvt-logo-stacked-light.svg` | Square spaces: social avatars, slides, stickers |
| `tvt-mark.svg`, `tvt-mark-light.svg` | The mark alone, when "tvt" is already written nearby |
| `tvt-logo-mono-black.svg`, `tvt-logo-mono-white.svg` | One-color print, engraving, embroidery |
| `favicon.svg` | Browser tabs and app icons; a heavier line and outline so the cut still reads at 16 px |

## Colors

| Role | On dark | On light |
| --- | --- | --- |
| Kept bars | `#5794F2` blue, `#A352CC` purple | `#3D71D9`, `#8F3BB8` |
| The trimmed bar | `#FF9830` orange | `#E0752D` |
| The threshold | `#73BF69` green | `#37872D` |
| Wordmark | `#FFFFFF` | `#111217` |
| Background | `#111217` | `#F4F5F5` |

## Use

- Keep clear space around the logo of at least the height of one bar's width (about 15% of the mark's height).
- Minimum size: the horizontal logo 24 px tall on screen, 10 mm in print; below that, use `favicon.svg` or the mark.
- Don't recolor the bars, stretch the logo, add effects, or rearrange the mark and the wordmark.
- For a PNG, export from the SVG at the size you need, for example:
  `rsvg-convert -h 512 tvt-logo-stacked-dark.svg > tvt-512.png`
