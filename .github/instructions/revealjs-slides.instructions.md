---
applyTo: "src/**/*.html"
---

# Reveal.js Slide Authoring Instructions

When editing HTML files in `src/`, you are working with Reveal.js presentation files.

## Slide Structure

- Each top-level `<section>` inside `<div class="slides">` is a horizontal slide.
- Nested `<section>` elements create vertical slide stacks.
- Speaker notes go inside `<aside class="notes">` within each `<section>`.

## Speaker Notes Format

Every slide MUST have speaker notes. Format:

```html
<aside class="notes">
  <p>Main talking point for this slide.</p>
  <p>Transition: "Now let's look at..."</p>
  <p>If asked about X, respond with Y.</p>
</aside>
```

Notes should include:
- What to say (3-6 sentences of talking points)
- How to transition to the next slide
- Objection-handling tips where relevant
- Timing cues (e.g., "Pause here for effect")

## Available CSS Classes

Use these classes defined in the template's `<style>` block:

| Class | Purpose | Usage |
|-------|---------|-------|
| `center-slide` | Centers all text (title/closing slides) | `<section class="center-slide">` |
| `stat-number` | Large gradient number for statistics | `<span class="stat-number">55%</span>` |
| `gradient-text` | Copilot purple-blue gradient text for emphasis | `<span class="gradient-text">key phrase</span>` |
| `highlight-box` | Subtle bordered box for key points | `<div class="highlight-box">...</div>` |
| `two-column` | Side-by-side grid layout | `<div class="two-column"><div>Left</div><div>Right</div></div>` |
| `competitor-table` | GitHub-styled comparison table | `<table class="competitor-table">...</table>` |
| `tag` | Pill-shaped label (purple) | `<span class="tag">Enterprise</span>` |
| `check-green` | Green checkmark text | `<span class="check-green">✓</span>` |
| `cross-dim` | Dimmed cross for competitor gaps | `<span class="cross-dim">✗</span>` |
| `copilot-logo` | Centered logo container | `<div class="copilot-logo">...</div>` |

## Content Rules

- **CRITICAL: All slide content must fit within 960×700px without scrolling**
- Max 4 bullet points per slide (5 only in two-column, per column)
- Max 8 words per bullet point
- Max 4 highlight-box elements per slide, each limited to 1 line of text
- Max 3 stat blocks on stat slides
- Competitor table: max 6 rows, 3-4 words per cell
- Use `<h2>` for slide titles (not `<h1>` except the title slide)
- No external images — use inline SVG, Unicode, or CSS for visuals
- Use emojis sparingly — max 1-2 per slide, only when they add meaning
- Prefer CSS classes (`gradient-text`, `tag`, `check-green`) over emojis for visual polish
- Write real content, never placeholders
- HTML only — no Markdown plugin usage
- Use `check-green` / `cross-dim` in competitor tables instead of emoji ✅/❌
