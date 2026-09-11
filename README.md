# DJones Catering

A responsive, single-page marketing website for DJones Catering LLC — customized catering (buffet style and four-course plated meals) for weddings, corporate events, and private parties.

Built with plain HTML, CSS, and JavaScript (no build step, no dependencies).

## Structure

```
.
├── index.html        Page markup (Home, About, Services, Menu, Gallery, Testimonials, Contact)
├── css/style.css      All styling, responsive breakpoints, animations
├── js/script.js       Nav toggle, scroll effects, menu tabs, form validation
└── images/            Favicon and real event/food photography
```

## Running locally

No build tools required — just serve the folder statically, e.g.:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

Or open `index.html` directly in a browser.

## Customizing

- **Business details** — phone `(312) 852-8499` and email `JonesD74@icloud.com` are live in the Contact and Footer sections of `index.html`. Address/service area is still a placeholder ("Greater Metro Area & Surrounding Counties") — update it once you have a specific service radius to publish.
- **Photos** — the hero, About, and Gallery sections use real event photography (in `images/`). Add more by dropping new files into `images/` and adding `<img>` tags following the existing pattern in the Gallery section.
- **Menu items** — edit the `.menu-panel` sections in `index.html` to reflect actual dishes and pricing.
- **Social links** — update the `href="#"` placeholders in the `.social-links` block with real profile URLs.
- **Contact form** — the form currently validates client-side and shows a success message, but is not wired to a backend. Connect it to a service like Formspree, Netlify Forms, or a custom API endpoint inside the `submit` handler in `js/script.js` (see the comment marking where to add the request).

## Deployment

This is a static site, so it can be deployed as-is to GitHub Pages, Netlify, Vercel, Cloudflare Pages, or any static host — no build command needed.
