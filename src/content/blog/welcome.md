---
title: 'Welcome to the Fieldwork blog'
description: 'Astro blog for firmware benchmark updates and engineering notes.'
pubDate: 'May 17 2026'
heroImage: '../../assets/blog-placeholder-1.jpg'
---

This site is built with [Astro](https://astro.build) and deploys to [Vercel](https://vercel.com) as a static site from the `blog/` directory in the fieldwork-firmware monorepo.

## Adding a post

Create a new `.md` or `.mdx` file in `blog/src/content/blog/` with frontmatter:

```yaml
---
title: 'Your title'
description: 'One-line summary'
pubDate: 'May 17 2026'
---
```

Run `npm run dev` inside `blog/` to preview locally.

## Deploying

In Vercel, set the project **Root Directory** to `blog`, then connect the repo. After the first deploy, update `site` in `astro.config.mjs` to your production URL so the sitemap and RSS feed use the correct domain.
