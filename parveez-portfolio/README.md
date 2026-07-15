# Parveez M — Portfolio Website

A premium, interactive one-page portfolio built with vanilla HTML/CSS/JS,
GSAP + ScrollTrigger for motion, and no build step required.

## Structure
```
portfolio/
├── index.html          # everything lives here (markup, styles, scripts)
├── images/
│   └── photo.jpg        # your professional photo
├── resume/
│   └── Parveez_M_Resume.pdf
└── README.md
```

## Run locally
Just open `index.html` in a browser — or, for the smoothest experience
(so relative paths and any future fetch calls behave correctly), serve it:

```bash
npx serve .
# or
python3 -m http.server 8000
```

## Deploy on Vercel
1. Push this folder to a GitHub repo (or drag-and-drop it into vercel.com/new).
2. Framework preset: **Other** (static site) — no build command needed.
3. Output directory: `/` (root).
4. Deploy. Done.

You can also deploy instantly with the Vercel CLI:
```bash
npm i -g vercel
vercel
```

## Content notes
- Every real project, internship, and credential is pulled directly from
  your résumé and rewritten for clarity.
- The "Concept Case Studies" section is clearly labeled as self-initiated
  design exploration, not client work — this is intentional, per your brief.
- Testimonials are clearly labeled as sample/placeholder content.
- The contact form is front-end only; wire it to Formspree, EmailJS, or a
  serverless function to actually receive messages.
- Swap the placeholder `#` links for your real LinkedIn/GitHub URLs in
  `index.html` (search for `href="#"`).

## Customizing
- Colors: CSS variables at the top of `index.html` under `:root` and
  `[data-theme="light"]`.
- Fonts: Space Grotesk (display), Inter (body), JetBrains Mono (labels/data).
- Sections are clearly commented (`<!-- ============ SECTION ============ -->`)
  for easy editing.
