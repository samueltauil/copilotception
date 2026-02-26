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
| `stat-number` | Large blue number for statistics | `<span class="stat-number">55%</span>` |
| `highlight-box` | Blue-bordered box for key points | `<div class="highlight-box">...</div>` |
| `two-column` | Side-by-side grid layout | `<div class="two-column"><div>Left</div><div>Right</div></div>` |
| `competitor-table` | Styled comparison table | `<table class="competitor-table">...</table>` |
| `emoji-icon` | Slightly enlarged emoji | `<span class="emoji-icon">🚀</span>` |

## Content Rules

- Max 5 bullet points per slide
- Max 10 words per bullet point
- Use `<h2>` for slide titles (not `<h1>` except the title slide)
- No external images — use emoji and CSS for visual interest
- Write real content, never placeholders
- HTML only — no Markdown plugin usage
