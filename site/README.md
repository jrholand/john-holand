# John R. Holand — portfolio site (static)

Single-file static site rebuilt from john-r-holand.onhercules.app. No build step, no framework.

```
index.html
assets/portrait.jpg
assets/John_Holand_Resume.pdf
assets/John_Holand_Executive_Summary.pdf
```

To update the resume or summary later, replace the PDF with the same filename.

## Host it
Any static host works: GitHub Pages, Netlify, Cloudflare Pages, or nginx/Apache/Caddy
(point the web root at this folder). Local preview: `python3 -m http.server 8080`.

## Notes
- Content lives in the JS data arrays near the bottom of index.html (METRICS, CASES, ROLES, etc.).
- Contact form opens the visitor's email client (mailto). For a real form backend, set the
  form's `action` to Formspree / Netlify Forms and delete the submit handler.
- Fonts load from Google Fonts. To fully self-host, download Hanken Grotesk, IBM Plex Mono
  and Instrument Serif and swap the <link> for @font-face rules.
