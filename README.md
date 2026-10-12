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
  This is the most important thing to fix, and it needs a real form service key.
- No analytics, by choice so far. Adding any would mean revisiting the cookies
  section of the privacy policy, which currently states plainly that the site sets
  none.
- John's photo is an older picture and is due to be replaced. When the new one
  arrives, check its cut-out edge before use. The current one had a pale halo from
  being cut off a light background, which had to be repaired.

## Legal pages

`privacy.html` and `terms.html` are built from the Dee Nick Media templates
(DRAFT 12.19.24), with placeholders filled in and **clauses removed that do not
apply to this site**: payment processing, email subscriptions, advertising and
analytics cookies, and social media tracking. The site does none of those. The
privacy policy states that no cookies are set, which is true today and must be
revisited if analytics is ever added.

Effective date on both is October 12, 2026. Neither has been reviewed by a lawyer.
