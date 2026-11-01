# Meridian Data website

Static site. No build step, no server code.

## Contents
- `index.html` – the whole site. Pages are switched by URL hash:
  `#home`, `#who-we-work-with`, `#our-approach`, `#responsible-data`, `#contact`
- `assets/london-skyline.jpg` – hero and page-header image
- `favicon.svg`, `robots.txt`

## Deploy
Upload the folder contents to the web root of any static host
(Netlify, Vercel, Cloudflare Pages, GitHub Pages, S3 + CloudFront, or a standard web server).
Netlify: drag the folder onto app.netlify.com/drop.

Fonts load from Google Fonts; everything else is local.

## Before going live
1. **Contact form** – currently validates input but does not send anything.
   Point it at a form service or your own endpoint: in `index.html`, find the
   `// Enquiry form` script block and replace the "not yet connected" message with a
   `fetch()` POST to your endpoint (e.g. Formspree, Netlify Forms, or your CRM).
2. **Contact details** – add email, phone and registered address in the Contact page aside
   and the footer.
3. **Legal pages** – add a privacy notice and cookie statement if required, and your
   company registration details in the footer.
4. **Image** – `assets/london-skyline.jpg` is the hero and header photo. Replace it, keeping the filename, to change it.
