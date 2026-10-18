# Krushang Prajapati — Portfolio

Personal portfolio of an Electronics & Communication Engineering student at SCET, Surat, focused on FPGA/VLSI design and embedded systems, with full-stack and AI side projects.

**Live site:** https://krushang004.runs-on.dev

## What's on the site

- **Hero** — photo, short intro and a terminal-style `profile.json` card with key stats and a Resume download.
- **About** — background, the FPGA Design Challenge 2.0 win, and achievement badges.
- **Skills** — grouped as HDL & FPGA, Embedded & Hardware, Programming, Web & Cloud, AI & Vision, and Tools.
- **Projects** — FPGA image processing (flagship), cache controller, digital design lab, smart classroom IoT dashboard, offline AI assistant, HTTP honeypot, and Mindscape.
- **Experience & Education** — freelance work, Google Student Ambassador, FPGA Design Challenge 2.0, IEEE/T&P volunteering, and the B.Tech at SCET.
- **Contact** — email, GitHub and LinkedIn links.

## Highlights

- 🏆 1st place among 22 teams at FPGA Design Challenge 2.0 (SCET) — real-time image processing on a Basys 3 (Artix-7) board with 8 hardware filters, written in Verilog.
- Direct-mapped, write-back cache controller in Verilog with a 5-state FSM, verified with a testbench.
- ESP32-CAM AI motion detection with a Firebase dashboard, plus Python security and offline-AI tools.

## Tech

- Single static page: HTML, CSS and JavaScript are all inside `index.html`. `styles.css` and `script.js` are intentionally near-empty placeholders kept for GitHub Pages compatibility.
- **Three.js** (loaded from a CDN via an import map) draws the starfield background and shooting stars.
- **Fonts:** Space Grotesk, Orbitron and Inter from Google Fonts.
- Responsive layout with a hamburger menu on small screens, and scroll-triggered reveals using `IntersectionObserver`.
- Colour tokens are CSS variables at the top of `index.html` (dark background `#0f1419`, cyan accent `#00d4ff`).

## Project structure

```
.
├── index.html          # Markup, styles and scripts (everything lives here)
├── avatar.png          # Hero photo
├── resume.pdf          # Linked from the Resume button
├── styles.css          # Placeholder (styles are embedded in index.html)
├── script.js           # Placeholder (scripts are embedded in index.html)
├── package-lock.json   # Empty lockfile; there are no npm dependencies
└── README.md
```

## Run locally

There is no build step. Because the page loads Three.js as an ES module, serve it over HTTP instead of opening the file directly:

```bash
# Python
python -m http.server 8000

# or Node.js
npx http-server
```

Then open http://localhost:8000.

## Updating the content

- **Projects, skills, timeline:** edit the matching sections in `index.html` (`#projects`, `#skills`, `#experience`).
- **Resume:** replace `resume.pdf` with the new file under the same name.
- **Photo:** replace `avatar.png`.
- **Link preview:** the canonical URL and Open Graph tags are in the `<head>` of `index.html`; update them if the domain changes.

## Contact

- Email: krushangrprajapati@gmail.com
- GitHub: [@Krushang004](https://github.com/Krushang004)
- LinkedIn: [Krushang Prajapati](https://www.linkedin.com/in/krushang-prajapati-5b4a97324/)
- X: [@Krushang300506](https://x.com/Krushang300506)
