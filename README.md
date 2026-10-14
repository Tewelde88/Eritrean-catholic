# Catholic Church in Eritrea: official website

The official digital home of the Catholic Church in Eritrea and the platform of the Eritrean Catholic Bishops' Conference.

## Design system

Before building the pages, the site's visual rules are defined in [`design-system/`](design-system/):

| File | What it holds |
|---|---|
| `tokens.css` | The named values: colors (light and dark mode), fonts and text sizes, spacing, corner shapes |
| `base.css` | How plain text, headings and links look, plus layout helpers (`.container`, `.section`) |
| `components.css` | Buttons, cards, the top navigation bar and the footer |
| `styleguide.html` | A page that shows everything above. Open it in a browser to see the design system. |

### The choices

- **Feel:** dignified and traditional
- **Colors:** Marian Blue and Gold (gold is for lines and ornaments, never for reading text)
- **Fonts:** EB Garamond for headings, Source Sans 3 for reading text, Noto Ethiopic for Tigrinya
- **Spacing:** Comfortable (4, 8, 16, 24, 32, 48, 64 px)
- **Components:** Classic: blue menu bar with a gold line, gently squared corners, cards topped with gold

### Using it on a page

Add these lines inside `<head>`:

```html
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=EB+Garamond:wght@500;600&family=Source+Sans+3:wght@400;600&family=Noto+Serif+Ethiopic:wght@500;600&family=Noto+Sans+Ethiopic:wght@400;600&display=swap">
<link rel="stylesheet" href="design-system/tokens.css">
<link rel="stylesheet" href="design-system/base.css">
<link rel="stylesheet" href="design-system/components.css">
```

Then use the tokens instead of typing raw values, for example `color: var(--color-primary-text)` or `gap: var(--space-4)`. Copy the navigation, button and card markup from `styleguide.html`.
