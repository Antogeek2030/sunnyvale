# Drain Cleaning Sunnyvale CA

Professional drain cleaning, hydro jetting, and sewer line services website built with Astro and deployed on Cloudflare Pages / Workers.

**Live site:** https://draincleaningsunnyvaleca.com

## Features

- Fully responsive, mobile-friendly design
- Service pages: Drain Cleaning, Hydro Jetting, Sewer Line Cleaning, Camera Inspection, Emergency Services
- Service Areas page with embedded Google Map
- Contact page with form and map pinpointing 1095 W Evelyn Ave #104, Sunnyvale, CA 94086
- SEO-ready (sitemap, robots.txt, meta tags, canonical URLs)
- Cloudflare adapter for Pages / Workers deployment

## Commands

| Command | Action |
| --- | --- |
| `npm install` | Install dependencies |
| `npm run dev` | Start local dev server |
| `npm run build` | Build production site to `./dist/` |
| `npm run deploy` | Build + deploy to Cloudflare |
| `npm run preview` | Preview production build locally |

## Deploy to Cloudflare Pages

### Recommended settings in Cloudflare Pages dashboard

| Setting | Value |
| --- | --- |
| **Framework preset** | Astro (or None) |
| **Build command** | `npm run build` |
| **Build output directory** | `dist` |
| **Root directory** | `/` (or leave blank) |
| **Deploy command** | leave empty (or remove any custom deploy command) |

Do **not** set the deploy command to `npx wrangler deploy` or `npm run deploy` unless you also set the build command to run first. Cloudflare Pages already uploads the contents of the build output directory after a successful build.

### Alternative: deploy via Wrangler CLI

```bash
npm install
npm run deploy   # runs astro build && wrangler deploy
```

## Customize

- Update phone, email, and address in `src/consts.ts`
- Replace Formspree form ID in `src/pages/contact.astro` with your own endpoint
- Colors and styling are in `src/styles/global.css`

## Location

1095 W Evelyn Ave #104  
Sunnyvale, CA 94086  
USA
