# D. Jones Catering

A responsive, single-page marketing website for D. Jones Catering — a full-service catering business for weddings, corporate events, and private parties.

Built with plain HTML, CSS, and JavaScript (no build step, no dependencies).

## Structure

```
.
├── index.html        Page markup (Home, About, Services, Menu, Gallery, Testimonials, Contact)
├── css/style.css      All styling, responsive breakpoints, animations
├── js/script.js       Nav toggle, scroll effects, menu tabs, form validation
└── images/            Favicon and any real photos you add later
```

## Running locally

No build tools required — just serve the folder statically, e.g.:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

Or open `index.html` directly in a browser.

## Customizing

- **Business details** — phone, email, address, and hours are in the Contact and Footer sections of `index.html`. Search for `(312) 852-8499` and `hello@djonescatering.com` to replace with real info.
- **Photos** — the hero, About, and Gallery sections currently use CSS gradient placeholders (`.media-block`, `.gallery-item`, `.hero-bg`) instead of real photography. Drop real images into `images/` and swap the relevant CSS `background` declarations (or add `<img>` tags) once photos are available.
- **Menu items** — edit the `.menu-panel` sections in `index.html` to reflect actual dishes and pricing.
- **Social links** — update the `href="#"` placeholders in the `.social-links` block with real profile URLs.
- **Contact form** — the form currently validates client-side and shows a success message, but is not wired to a backend. Connect it to a service like Formspree, Netlify Forms, or a custom API endpoint inside the `submit` handler in `js/script.js` (see the comment marking where to add the request).

## Deployment

This is a static site, so it can be deployed as-is to GitHub Pages, Netlify, Vercel, Cloudflare Pages, or any static host — no build command needed.
