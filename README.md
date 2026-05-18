# Fieldwork Blog

Astro blog for Fieldwork firmware updates, benchmark notes, and engineering write-ups. Deploys as a static site on [Vercel](https://vercel.com).

## Local development

```sh
cd blog
npm install
npm run dev
```

Open [http://localhost:4321](http://localhost:4321).

## Writing posts

Add Markdown or MDX files under `src/content/blog/`:

```md
---
title: 'My post'
description: 'Short summary for SEO and listings'
pubDate: 'May 17 2026'
heroImage: '../../assets/blog-placeholder-1.jpg'
---

Your content here.
```

## Deploy to Vercel

1. Import this repository in the [Vercel dashboard](https://vercel.com/new).
2. Set **Root Directory** to `blog`.
3. Leave the framework preset as **Astro** (build: `npm run build`, output: `dist`).
4. After the first deploy, set `site` in `astro.config.mjs` to your production URL (for sitemap and canonical links).

Or from the CLI:

```sh
cd blog
npx vercel
```

## Project structure

```text
blog/
├── public/           # static assets (favicon, etc.)
├── src/
│   ├── assets/       # images and fonts
│   ├── components/
│   ├── content/blog/ # blog posts (Markdown / MDX)
│   ├── layouts/
│   └── pages/
├── astro.config.mjs
└── package.json
```
