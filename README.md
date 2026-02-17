# riverbraun.com

Travel content strategy and writing — personal site for River Braun.

## Stack

- Static HTML/CSS/JS (single page)
- Hosted on [Vercel](https://vercel.com)
- Domain: [riverbraun.com](https://riverbraun.com)

## Local Development

```bash
npm run dev
```

Opens at `http://localhost:3000`

## Deployment

This repo is connected to Vercel for automatic deployments. Every push to `main` triggers a production deploy.

### First-time setup

1. Push this repo to GitHub
2. Go to [vercel.com/new](https://vercel.com/new) and import the repo
3. Vercel auto-detects the config from `vercel.json`
4. Add custom domain `riverbraun.com` in **Settings → Domains**
5. Update DNS at your registrar:
   - **A record:** `76.76.21.21`
   - **CNAME for www:** `cname.vercel-dns.com`

## Before Launch Checklist

- [x] Replace scheduling URL with TidyCal link
- [x] Replace LinkedIn URL with actual profile
- [x] Add Substack link (onawander.substack.com)
- [x] Set email to beawesome@riverbraun.com
- [ ] Verify beawesome@riverbraun.com email is receiving
- [ ] Add favicon (`public/favicon.ico`)
- [ ] Add OG image (`public/og-image.jpg`) and update meta tags
- [ ] Verify/update statistics (87%, 3×) with your own data
- [ ] Set up Google Search Console and submit sitemap
- [ ] Set up Google Analytics or Plausible

## Future: Migration to Next.js + Sanity

When ready to add a blog and CMS:

1. `npx create-next-app@latest` in a new branch
2. Install `next-sanity` and configure Sanity studio
3. Migrate HTML to Next.js pages/components
4. Vercel deployment stays the same — just auto-detects Next.js
