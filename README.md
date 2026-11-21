# Jamafriq Global Consultancy — website

Static site for [jamafriqglobal.com](https://www.jamafriqglobal.com): IELTS coaching and global placement consultancy, Nairobi, Kenya.

## Structure
- `index.html`, `courses.html`, `mentorship.html`, `reviews.html`, `contact.html` — main pages
- `terms.html`, `privacy.html`, `cookies.html`, `404.html` — legal and error pages
- `css/site.css` — single stylesheet
- `assets/` — logo, IELTS mark and partner logos
- `sitemap.xml`, `robots.txt`, `llms.txt`, `site.webmanifest` — SEO
- `vercel.json` / `_redirects` — redirects from the old URLs (`/enroll`, `/partners`, …) plus caching and security headers

## Deploy
No build step. Deploy the repository root to Vercel, Netlify or any static host.

## Notes
- Time-limited announcements carry a `data-until` ISO date and remove themselves automatically.
- All forms compose a WhatsApp message to +254 721 776 745; no backend required.
- Add `assets/og-image.jpg` (1200×630) for social previews.

## Compliance notes (Kenya DPA 2019 checklist)
- Fonts are self-hosted (`assets/fonts`, SIL Open Font Licence); nothing loads from Google.
- No analytics, pixels, maps or embeds. If analytics is added, load it only when `document.documentElement.dataset.consent === 'all'`.
- Every form has a required privacy tick box, a separate unticked marketing box, a warning not to enter ID/passport/medical details, length limits and a double-tap guard.
- Still to do outside the code: ODPC registration check, advocate review of Terms/Privacy, real office address in the policies, evidence on file for the 98% pass rate and 500+ placed figures, partner permission for logos, Search Console and Google Business Profile.
