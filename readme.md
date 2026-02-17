# Glasshouse Landing Page

Landing page for Glasshouse.

## Stack

- **Astro** — static site generator, zero client JS by default
- **Tailwind CSS v4** — utility-first styling via Vite plugin
- **GitHub Pages** — hosting via GitHub Actions

## Project structure

```
src/
├── layouts/Layout.astro       # Base HTML shell (dark theme, fonts, meta)
├── components/
│   ├── Navbar.astro            # Fixed nav with mobile toggle
│   ├── Hero.astro              # Tagline + CTAs
│   ├── Architecture.astro      # Core component cards
│   ├── Features.astro          # Product feature grid (supports image/video)
│   ├── CtaBanner.astro         # Mid-page callout
│   ├── TechStack.astro         # Tech badge pills
│   ├── DataProviders.astro     # Integration logos
│   ├── Faq.astro               # Native <details>/<summary>
│   └── Footer.astro
├── pages/index.astro           # Composes all sections
└── styles/global.css           # Tailwind directives + theme tokens
```

## Development

```sh
npm install
npm run dev        # localhost:4321
npm run build      # static output to dist/
```

## Deployment

Pushes to `main` trigger a GitHub Actions workflow that builds and deploys to GitHub Pages.
