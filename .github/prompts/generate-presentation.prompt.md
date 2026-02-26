Generate the full GitHub Copilot pitch presentation by filling in the slides in `src/index.html`.

## What to do

Open `src/index.html` and replace the placeholder comment block inside `<div class="slides">` with the complete set of 12 presentation slides as defined in the repository instructions.

Follow the slide structure, content guidelines, evaluation criteria, CSS classes, and speaker notes requirements specified in `.github/copilot-instructions.md` exactly.

## Key requirements

1. Generate all 12 slides (Title → Problem → Cost → Intro → How it Works → Value → Differentiation → Enterprise → Proof → Ecosystem → CTA → Thank You)
2. Every slide MUST have `<aside class="notes">` with detailed presenter talking points (3-6 sentences)
3. Use the CSS utility classes: `center-slide`, `stat-number`, `highlight-box`, `two-column`, `competitor-table`, `emoji-icon`
4. Keep slide text concise (max 5 bullets, max 10 words each)
5. Include real stats, real customer names, real competitive comparisons
6. Presenter notes must include transition phrases and objection-handling tips
7. Use Samuel Tauil's name and contact info (samueltauil@microsoft.com, github.com/samueltauil) — never use placeholders
8. Use emojis sparingly (1-2 per slide max). Prefer CSS classes (`gradient-text`, `tag`, `check-green`, `cross-dim`) for visual polish
9. Do NOT modify anything outside the `<div class="slides">` container
8. Do NOT add external images or dependencies
9. Ensure ALL 6 evaluation criteria from `requirements/criterias.txt` are thoroughly addressed

## After generation

Tell me to:
- Run `npm start` to serve the presentation
- Open http://localhost:8000 in a browser
- Press **S** to open speaker/presenter view with notes
