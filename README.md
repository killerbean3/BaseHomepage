# Base Homepage

Reusable landing-page template. Dark purple palette, pinned Header & Footer components, and full responsiveness.

## Theme

- **Palette**: dark `#0b0f19` / `#0f0f1e` backgrounds with `#a78bfa` (violet-purple) accent
- **Toolbar**: glassmorphic header with `backdrop-filter: blur(6px)` and purple border accents
- **Footer**: subtle divider line, copyright + legal links
- All design tokens are CSS custom properties in [`src/index.css`](src/index.css)

## Structure

```
src/
  index.css          ← global CSS variables + page layout styles
  components/
    Header.tsx       ← reusable toolbar/header
    Footer.tsx       ← reusable copyright/legal footer
    index.ts         ← barrel export
  App.tsx            ← demo landing page using the theme
```

## How to customise

1. **Brand & nav** — edit `NAV_ITEMS` in [App.tsx](src/App.tsx) and pass `brandName` to `<Header />` / `<Footer />`.
2. **Colors** — change any variable in [`:root`](src/index.css). All components consume them automatically.
3. **Content** — replace the hero, feature blocks, and stats with your own text / images.

## Dev

```bash
npm install
npm run dev    # http://localhost:5173
```
