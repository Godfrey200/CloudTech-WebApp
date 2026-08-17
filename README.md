# TechCrush — CloudTech-WebApp

Learn cloud the way it's actually run in production. This repository contains the TechCrush marketing/homepage: a small, responsive static site demonstrating the program, curriculum, pipeline metaphor, and a simple cohort signup form. The site is authored with plain HTML, CSS and vanilla JavaScript and is designed to be deployed as a static site (example: Azure Static Web Apps).

## Quick demo
Open index.html in your browser or run a simple static server (see How to run).

## Features
- Responsive marketing homepage (hero, curriculum, pipeline, instructors, cohort CTA)
- Terminal type-on animation in the hero (script.js)
- Smooth progress rail showing scroll position
- Simple client-side cohort signup placeholder (form handled in script.js)
- Built and intended to be deployed as an Azure Static Web App (terminal demo in the hero)

### Stack
- Language(s): HTML, CSS, JavaScript
- Framework / runtime: None — plain static site
- Notable libraries/services: Google Fonts; intended for Azure Static Web Apps deployment

## Repository layout

How it fits together:
- index.html is the single-page markup. styles.css contains the full visual system (tokens, layout, components). script.js wires the hero terminal animation, the scroll progress rail and the cohort signup placeholder. The site is static — no server-side code — and can be hosted on any static host or CDN.

## How to run (local)
Minimal steps to preview locally after cloning:

1. Clone the repo
   git clone https://github.com/Godfrey200/CloudTech-WebApp.git
   cd CloudTech-WebApp

2. Open directly
   - Open index.html in your browser (double-click or File → Open).

3. Run a simple static server (recommended)
   - Python 3:
     python3 -m http.server 8000
     Open http://localhost:8000
   - Node (serve):
     npx serve -s . 5000
     Open http://localhost:5000

No build step is required.

## Deploy
This project is ready for static hosting. Example options:
- Azure Static Web Apps — the site’s hero shows an example az CLI flow (az staticwebapp create ...).
- GitHub Pages — push the repository and enable Pages for the main branch.
- Any static host / CDN (Netlify, Vercel, S3 + CloudFront, etc.)

If you want an example Azure CLI command copied from the site’s terminal animation:

(Adjust parameters to match your Azure subscription, resource group and repository.)

## Contributing
Contributions are welcome:
- Open an issue to discuss changes or feature requests.
- Create a branch, make changes, and open a pull request.
- Keep changes focused (styling, accessibility improvements, small JS fixes).

Notes:
- The cohort form is a placeholder; production deployments should replace the client-side handler with a secure backend or serverless endpoint for storing or emailing requests.

## License
Add your preferred license here (e.g., MIT). If you want, I can add a LICENSE file.

## Contact
Repo owner: Godfrey200 — open issues or PRs on this repository for questions or suggested updates.
