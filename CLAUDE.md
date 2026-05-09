# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
pnpm dev        # Start dev server
pnpm build      # Production build
pnpm preview    # Preview production build
```

Use `pnpm` (not npm). No lint or test scripts are configured.

## Architecture

Personal site at ethleb.com built with **Astro 5** + **React 19**. Deployed to Netlify.

**Stack:**
- Astro for static generation and file-based routing
- React (`.jsx`) only for client-side interactive components — everything else uses `.astro`
- Catppuccin Mocha color palette via CSS custom properties (`--ctp-*`) defined globally in `src/layouts/Layout.astro`
- Astro Content Collections for blog posts (`src/content/posts/`)

**Routing:**
- `src/pages/index.astro` — home page, composes section components
- `src/pages/posts/[...slug].astro` — dynamic blog post routes, pre-rendered via `getStaticPaths()`
- Blog post schema defined in `src/content/config.ts` (fields: `title`, `description`, `date`, `tags?`, `draft?`)

**Components split:**
- `.astro` components: static structure with scoped `<style>` blocks — Intro, Posts, Projects, Socials, WaveDivider, Layout
- `.jsx` components: client-interactive only (e.g., `SoundWave.jsx` with React state)
- Projects accordion uses vanilla JS with ARIA attributes inside `Projects.astro`

**Styling:**
- No CSS framework — scoped component styles with Catppuccin CSS variables
- Responsive breakpoints at 600px and 768px
- Per-component color overrides via local CSS vars (e.g., `--post-color`, `--project-color`)

**Formatting:** Prettier with `prettier-plugin-astro` and `@trivago/prettier-plugin-sort-imports`. Import order: third-party → internal → models → utils → components.
