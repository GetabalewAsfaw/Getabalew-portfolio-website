# Portfolio website

Static personal portfolio for Getabalew Asfaw: plain HTML, CSS and JavaScript, no build step and no package manager.

- Live site: https://getabalew-asfaw.vercel.app/ (Vercel deploys `main` automatically). `.github/workflows/pages.yml` is a leftover that runs an npm build this repo doesn't have, so it fails; ignore it or delete it.
- `index.html` holds every page (About, Resume, Portfolio, Certificates, Contact); `assets/js/script.js` switches between them via `data-nav-link` buttons and `data-page` articles.
- Styles: `assets/css/style.css`. Icons come from Ionicons 5.5.2 via unpkg.
- Images live in `assets/`. Use forward slashes in paths; keep project thumbnails about 900px and certificates about 1400px on the long side.
- The contact form posts to SubmitForm and redirects to `thank-you.html`. Don't change the form endpoint.

## Adding a portfolio project
Copy an existing `<li class="project-item active" data-category="..." data-filter-item="">` block in the Portfolio section of `index.html`, use a category that matches the filter buttons, and put the image in `assets/`.

## Checking changes
- Preview locally: `python3 -m http.server 8000`, then open http://localhost:8000.
