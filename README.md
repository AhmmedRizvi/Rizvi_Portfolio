# Rizvi Ahmmed — Portfolio (Static HTML/CSS/JS)

No build tools, no server, no framework. Just open `index.html`, or serve the folder with any static file server.

## Run it

Double-click `index.html`, or for the best experience (so relative links and the resume download work cleanly), serve it locally:

```bash
# any of these work
npx serve .
python3 -m http.server 8000
```

## Where everything lives

```
index.html      → page structure only (sections are empty containers)
css/style.css   → all styling and animations
js/data.js      → ALL CONTENT: projects, skills, experience, journey, social links — edit this file to update the site
js/script.js    → renders data.js into the page + all interactivity
assets/         → put Rizvi-Ahmmed-Resume.pdf here
```

**To update content, you only ever need to edit `js/data.js`.** Nothing else needs to change — the page renders itself from that file.

## Before you go live

| What | Where |
|---|---|
| Resume PDF | Add `assets/Rizvi-Ahmmed-Resume.pdf` |
| GitHub / LinkedIn / email | `js/data.js` → `SOCIAL_LINKS` |
| Your domain (SEO tags) | `index.html` (`YOUR_DOMAIN.example`) and `robots.txt` / `sitemap.xml` |
| Contact form | Currently opens the visitor's email client with the message pre-filled (no backend needed). To collect submissions instead, point the form at a service like Formspree or Netlify Forms — swap the `submit` handler in `js/script.js` for a `fetch()` call to your form endpoint |
| Project GitHub/Live links | `js/data.js` → `githubUrl` / `liveUrl` per project (left `null` until real links exist, which hides the buttons) |

## Features

- Single HTML file, hash-based routing for project case studies (`#/projects/slug-name`) — shareable, deep-linkable, no server needed
- **Ctrl/Cmd + K** — command palette
- **Ctrl + `` ` ``** or the terminal icon — Easter-egg terminal (`help`, `about`, `skills`, `projects`, `experience`, `contact`, `clear`)
- Scroll-reveal, magnetic buttons, custom cursor, mouse-reactive hero background — all respect `prefers-reduced-motion`
- Dark theme by default with a theme-toggle icon (palette itself is dark-only per the design brief; add `dark:` Tailwind variants if you want a full light mode)
- No fabricated content — GitHub stats and unknown project links are shown as clear placeholders, never invented

## Deploying

Since it's fully static, this works as-is on GitHub Pages, Netlify, Vercel, or Cloudflare Pages — just push the folder, no build step configured or required.
