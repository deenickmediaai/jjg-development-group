# JJG Development Group website

Single static page. No build step.

## Deploy
Push this folder to GitHub and import it in Vercel (framework: Other). `index.html` is the site.

## Contact form
The form posts to Formspree. To connect it:
1. Create a free form at formspree.io with john@jjgdevelopmentgroup.com as the recipient.
2. Copy the form ID from the endpoint it gives you (https://formspree.io/f/XXXXXXXX).
3. In `index.html`, replace `FORM_ID` in the line `var FORM_ENDPOINT='https://formspree.io/f/FORM_ID';`.

Each submission arrives as an email with the subject "Website Contact Form: <name>" and every field listed, with reply-to set to the visitor.
Until the ID is set, the form falls back to opening the visitor's email app.

## Domain
Point jjgdevelopmentgroup.com at Vercel from GoDaddy when ready (A record 76.76.21.21 or CNAME to cname.vercel-dns.com for www).
