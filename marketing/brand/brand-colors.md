# Brand Colors — Ember Horizon Studios

*Reference before any design, marketing, or web task. These values are canonical.*

---

## Primary Palette

| Name          | Hex       | RGB                | Usage                                      |
| ------------- | --------- | ------------------ | ------------------------------------------ |
| **Ember**     | `#e07a3a` | rgb(224, 122, 58)  | Primary accent — logo ring, CTA buttons, tagline text, highlights |
| **Deep Night** | `#0c0c12` | rgb(12, 12, 18)    | Primary background — dark surfaces, logo base, body bg |
| **Warm White** | `#f0ede6` | rgb(240, 237, 230) | Primary text on dark — headings, body copy, mono-light logo |

## Secondary Palette

| Name          | Hex       | RGB                | Usage                                      |
| ------------- | --------- | ------------------ | ------------------------------------------ |
| **Ash**       | `#7a7690` | rgb(122, 118, 144) | Muted text, placeholders, secondary copy   |
| **Ember Dim** | `#8a4a1f` | rgb(138, 74, 31)   | Ember hover states, depth accents          |
| **Ember Border** | `rgba(224, 122, 58, 0.2)` | —    | Subtle borders and dividers on dark bg     |

---

## Logo Files

All files are in `marketing/brand/`. Open in Inkscape to convert text to paths before production use.

| File                   | Use                                              |
| ---------------------- | ------------------------------------------------ |
| `logo-primary.svg`     | Default — dark bg, full logo with text           |
| `logo-reversed.svg`    | Light bg (press kit, print, light websites)      |
| `logo-mono-dark.svg`   | Single dark color, transparent bg (emboss, print)|
| `logo-mono-light.svg`  | Single light color, transparent bg (over photos) |
| `logo-mark.svg`        | Icon only, square, dark bg — social media avatars|

---

## Typography (Brand Reference)

| Role           | Font                   | Weight | Notes                          |
| -------------- | ---------------------- | ------ | ------------------------------ |
| Display / Name | DM Serif Display       | 400    | Used on holding page, headings |
| Body / UI      | Inter                  | 300–500| Used on holding page, forms    |
| Logo wordmark  | Arial Black / Impact   | 900    | In SVG files; convert to paths in Inkscape before production |

---

## Web Implementation

```css
:root {
  --bg:          #0c0c12;
  --text:        #f0ede6;
  --muted:       #7a7690;
  --accent:      #e07a3a;
  --accent-dim:  #8a4a1f;
  --border:      rgba(224, 122, 58, 0.2);
}
```

These CSS variables are already implemented in `holding-page/index.html`.
