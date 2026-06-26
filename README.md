# Deepansh Dubey — Portfolio

A single-file, dependency-light personal portfolio. Dark-mode, motion-driven,
built around a pharma/computational-science visual language (cerulean accent,
molecular-node hero canvas). No build step — just `index.html`.

## Stack
- Hand-authored HTML + CSS (design tokens, 8-layer depth system)
- **GSAP + ScrollTrigger** (scroll choreography, timeline growth, counters)
- **Lenis** (smooth scroll, GSAP-ticker integrated)
- **VanillaTilt** (3D card tilt)
- Fonts: **Cabinet Grotesk** (Fontshare) · **DM Sans** + **IBM Plex Mono** (Google Fonts)
- All animation respects `prefers-reduced-motion`.

## Contact info — already set
Your real handles are baked into `index.html`:

| What | Value |
|------|-------|
| Email | `drx.deepanshdubey@gmail.com` |
| LinkedIn | `https://www.linkedin.com/in/deepanshdubey1` |
| GitHub | `https://github.com/drdeepanshdubey` |
| YouTube | `https://www.youtube.com/@RxPlained` *(verify this is your channel URL; update if not)* |

All other content (roles, projects, credentials) is populated from your CV.
The site is ready to deploy as-is.

## Deploy on GitHub Pages (free)

1. **Create a repo and push**
   ```bash
   git init
   git add index.html README.md
   git commit -m "Portfolio"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
   > Tip: name the repo `<your-username>.github.io` to get a clean root URL
   > (`https://<your-username>.github.io`). Any other name deploys to
   > `https://<your-username>.github.io/<repo-name>/`.

2. **Turn on Pages**
   - Repo -> **Settings** -> **Pages**
   - **Source:** *Deploy from a branch* -> Branch **main** -> folder **/ (root)** -> **Save**

3. Wait ~1 minute. Your site is live at the URL shown on that Pages screen.

### Alternative: drag-and-drop (no Git)
Go to https://app.netlify.com/drop and drag the `01-portfolio` folder in. Live instantly with a random subdomain you can rename.

## Updating content later
Everything lives in `index.html`:
- **Hero** — lines under `<header class="hero">` (name, role chips, tagline, metrics).
- **About / stats** — `<section id="about">`.
- **Expertise cards** — `<section id="expertise">`.
- **Work bento** — `<section id="work">` (each `<article class="work-card">`).
- **Experience timeline** — `<section id="experience">`.
- **Education** — `<section id="education">`.
- **Contact / footer** — `<section id="contact">`.

## Browser support
Modern evergreen browsers (Chrome, Edge, Firefox, Safari). Uses
`backdrop-filter`, CSS Grid, and Canvas 2D — all broadly supported. The page
degrades gracefully with JavaScript disabled (content remains readable; the
reveal animations simply show their final state).
