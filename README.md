# protfolio
# Puneeth Kumar V — Portfolio Website

A modern, responsive personal portfolio built with plain HTML5, CSS3, and JavaScript. No frameworks, no build step — open the file and it works.

## Files

```
puneeth-portfolio/
├── index.html   All content and page structure
├── style.css    Theme tokens, layout, animations
├── script.js    Theme toggle, nav, scroll reveals, contact form
└── README.md    This file
```

## Running it

No installation needed.

- **Quickest:** double-click `index.html` to open it in your browser.
- **Recommended (for correct font/asset loading):** serve it locally instead of opening the file directly:
  ```bash
  cd puneeth-portfolio
  python3 -m http.server 8000
  ```
  Then visit `http://localhost:8000`.

## Deploying it

Any static host works, since there's no backend:

- **GitHub Pages** — push this folder to a repo, enable Pages in repo Settings, point it at the branch/root.
- **Netlify / Vercel** — drag-and-drop the folder onto their dashboard, or connect the GitHub repo for auto-deploys.

## What to customize before publishing

| Location | What to update |
|---|---|
| `#profilePhoto` in `index.html` | Replace the placeholder avatar `src` with your real photo (or a path like `images/photo.jpg`) |
| Education section | Fill in college name, university name, and graduation year (three placeholder timeline entries included) |
| Projects section | Swap each project's GitHub link (currently all point to your profile) for the actual repo URL; add new `<article class="project-card">` blocks for future projects |
| Certifications section | Replace the dashed placeholder cards with real certification cards as you earn them |
| Skills section | Adjust the `--fill` percentages in the skill bars, or add/remove tags in the tag cloud |

## Notes on the contact form

The form has no backend — submitting it opens the visitor's email client with a pre-filled message addressed to `puneeth360720@gmail.com`. If you'd rather have messages land silently (no email client popup), wire the form up to a service like Formspree or Getform, or build a small backend endpoint and swap the `submit` handler in `script.js`.

## Browser support

Uses standard modern CSS (`backdrop-filter`, CSS custom properties, `IntersectionObserver`) — works in all current versions of Chrome, Firefox, Safari, and Edge. Reduced-motion preference is respected automatically.
