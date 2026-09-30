# shahzaibjavedportfolio

Static personal portfolio website for Shahzaib Javed, with a homepage, about page, projects page, and blog article pages.

## Tech stack

- HTML5
- Tailwind CSS (CDN)
- Vanilla JavaScript
- Lucide icons (CDN)
- Google Fonts (Inter, JetBrains Mono)

## Current site content

- `index.html`: main landing page with sections for About, Experience, Tech Stack, Featured Projects, FAQ, and Contact
- `about/index.html`: short about page
- `projects/index.html`: short projects overview page
- `blog/*/index.html`: blog pages and article pages
- SEO/support files: `robots.txt`, `sitemap.xml`, verification HTML file

## Project structure

```text
.
├── index.html
├── about/
│   └── index.html
├── projects/
│   └── index.html
├── blog/
│   ├── async-microservices-fastapi-redis/
│   ├── fastapi-performance-optimization/
│   ├── python-memory-optimization/
│   ├── rest-api-security-best-practices/
│   └── technical-seo-for-developers/
├── robots.txt
├── sitemap.xml
└── google03284386b208d7d3.html
```

## Local preview

No build step is required.

From the repository root:

```bash
python3 -m http.server 8000
```

Then open:

- Home: `http://localhost:8000/`
- About: `http://localhost:8000/about/`
- Projects: `http://localhost:8000/projects/`
- Example blog page: `http://localhost:8000/blog/fastapi-performance-optimization/`

## Customization guide

- **Profile content:** edit text in `index.html` (hero, experience, skills, FAQ, contact).
- **Social/contact links:** update links in `index.html` (`mailto:`, LinkedIn, GitHub, WhatsApp).
- **Styling/theme:** update the CSS variables and classes in `index.html` (the page uses Tailwind utilities + inline style block).
- **Icons:** icon names are set with `data-lucide` attributes in HTML.
- **SEO metadata:** update title/description/canonical/Open Graph/JSON-LD in each page file.
- **Sitemap/robots:** keep `sitemap.xml` and `robots.txt` aligned with your final production domain.
- **Blog pages:** each article is a static HTML file under `blog/<slug>/index.html`.

## Deployment / hosting details (from repository evidence)

- GitHub Actions shows `pages build and deployment` workflow runs for this repository.
- Repository SEO files currently reference more than one domain:
  - `index.html` canonical/Open Graph values reference `https://shahzaibjaved.dev/`
  - `about/`, `projects/`, `sitemap.xml`, and `robots.txt` reference `https://shahzaibjaved-portfolio.netlify.app/`

Because domain references are mixed, this README does **not** claim a single confirmed live URL.
