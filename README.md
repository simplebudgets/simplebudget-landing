<p align="center">
  <img width="250" height="250" alt="simpleSuite logo" src="https://github.com/user-attachments/assets/753aa8a3-3b44-41e4-af7a-e3dc8cd33e7f" />
</p>

<h1 align="center">simpleSuite Landing</h1>

<p align="center">
  The marketing and documentation site for simpleSuite — an open-source suite of personal productivity apps.
</p>

<p align="center">
  <a href="https://github.com/simplesuite/simplesuite-landing/blob/main/LICENSE"><img src="https://img.shields.io/github/license/simplesuite/simplesuite-landing" alt="License" /></a>
  <a href="https://github.com/simplesuite/simplesuite-landing/stargazers"><img src="https://img.shields.io/github/stars/simplesuite/simplesuite-landing" alt="Stars" /></a>
  <a href="https://github.com/simplesuite/simplesuite-landing/issues"><img src="https://img.shields.io/github/issues/simplesuite/simplesuite-landing" alt="Issues" /></a>
</p>

---

## What is this?

This is the source for [simplesuite.dev](https://simplesuite.dev) — the landing site, pricing page, guides, and legal pages for the simpleSuite ecosystem.

## simpleSuite Apps

| App | Description | Repo |
|-----|-------------|------|
| simpleBudget | Personal budgeting & expense tracking | [simplesuite/simplebudget](https://github.com/simplesuite/simplebudget) |
| simpleTracker | Notes, tasks & project management | [simplesuite/simpletracker](https://github.com/simplesuite/simpletracker) |
| Self-Host | Deploy the full stack on your own server | [simplesuite/simplesuite-selfhost](https://github.com/simplesuite/simplesuite-selfhost) |

## Pages

| Route | Description |
|-------|-------------|
| `/` | Landing page |
| `/simplebudget` | simpleBudget product page |
| `/simpletracker` | simpleTracker product page |
| `/pricing` | Pricing & FAQ |
| `/about` | About page |
| `/guides` | User guides |
| `/privacy` | Privacy policy |
| `/terms` | Terms of service |

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Astro 5 |
| Sitemap | @astrojs/sitemap |
| Hosting | Vercel |

## Getting Started

```bash
# Clone the repo
git clone https://github.com/simplesuite/simplesuite-landing.git
cd simplesuite-landing

# Install dependencies
npm install

# Start dev server
npm run dev
```

## Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Production build (outputs to `dist/`) |
| `npm run preview` | Preview production build locally |

## Project Structure

```
src/
├── assets/          # Images and SVGs
├── content/
│   └── guides/      # Markdown guide articles
├── layouts/
│   └── Base.astro   # Shared page layout
├── pages/
│   ├── index.astro
│   ├── simplebudget.astro
│   ├── simpletracker.astro
│   ├── pricing.astro
│   ├── about.astro
│   ├── guides/
│   ├── privacy.astro
│   └── terms.astro
└── content.config.ts
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the [GNU AGPL v3](LICENSE).
