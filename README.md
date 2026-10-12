# JJG Development Group

One-page site for JJG Development Group, owner's representative, Long Island and the New York region.
Live at **jjgdevelopmentgroup.com** (domain still to be pointed).

## Important: how this deploys

This site is deployed **directly to the Vercel project `jjg-site`**, not from this
repository. Vercel is not watching this repo, so **pushing here does not update the
live site.**

This repo exists as a backup and as the record of the current code. Keep it in sync
after any deploy.

A previous version of this repo held an older, simpler build of the site that did not
match what was live, which caused real confusion. The contents here now match the
deployed site.

## Files

- `index.html` — the whole site, styles and scripts inline
- `headshot.webp` — John Guido, cut out, transparent background
- `favicon.svg`

## Known work outstanding

- **The contact form does not send.** `FORM_ENDPOINT` is still the placeholder
  `https://formspree.io/f/FORM_ID`. It falls back to opening the visitor's own mail
  client and shows a success message either way, so enquiries can be lost silently.
  This is the most important thing to fix.
- No privacy policy or terms page, though the form collects personal data.
- No `og:image`, so shared links show no preview image.
- No robots.txt, sitemap.xml, canonical URL or custom 404.
- No analytics.
- Page title is just "JJG Development Group", with no description of the service or location.
- John's photo is an older picture and is due to be replaced.
