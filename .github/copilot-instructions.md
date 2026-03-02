# Copilotception — Repository Instructions

## Project Purpose

This project is a **Reveal.js presentation** that pitches **GitHub Copilot** to a customer audience. The presenter is **Samuel Tauil** from Microsoft.

When asked to generate, create, or fill in the presentation, you MUST produce a complete set of Reveal.js slides inside `src/index.html` by replacing the placeholder comment block with `<section>` elements.

---

## Presenter Information

- **Name**: Samuel Tauil
- **Email**: samuel.tauil@microsoft.com
- **GitHub**: @samueltauil
- **Role**: Microsoft

Use this information on the title slide and call-to-action slide. Do NOT use placeholder text like "Your Name" — always use Samuel Tauil's real details.

---

## Presentation Topic

**GitHub Copilot** — the AI-powered developer tool by GitHub (Microsoft). The pitch should cover what it is, the problems it solves, why it matters, why Microsoft/GitHub wins against competitors, and proof points that build credibility. The audience is a technical decision-maker at a company evaluating AI coding assistants.

---

## Evaluation Criteria (MUST satisfy ALL)

The presentation is scored on these 6 criteria. Every slide must serve at least one criterion. Design the narrative to maximize every score.

### 1. Problem Clarity
The customer's problem must be **clear, relevant, and compelling**.
- Lead with the pain: developer productivity bottleneck, talent shortage, slow onboarding, context-switching overhead, technical debt accumulation.
- Use concrete scenarios the audience will recognize.

### 2. Value Articulation
Clearly explain **why GitHub Copilot matters** to the customer.
- Translate features into business outcomes: faster delivery, reduced costs, happier developers, lower attrition.
- Use the "So what?" test — every claim must connect to customer value.

### 3. Microsoft Differentiation
Make it **crystal clear why Microsoft/GitHub wins** vs. alternatives (Cursor, Tabnine, Amazon CodeWhisperer/Q, JetBrains AI, Codeium/Windsurf).
- Deepest IDE integration (VS Code, Visual Studio, JetBrains, Neovim, Xcode).
- Enterprise-grade: SSO, IP indemnity, content exclusions, audit logs, policy controls.
- Copilot ecosystem: Chat, CLI, PR summaries, code review, workspace agents, MCP, extensions, coding agent.
- Backed by OpenAI partnership + Azure AI infrastructure.
- Multi-model: can use Claude, Gemini, OpenAI models — the customer chooses.
- Largest training signal: GitHub hosts 100M+ developers, 420M+ repos.
- GitHub Copilot coding agent (autonomous issue-to-PR agent).

### 4. Storytelling & Flow
The pitch must be **easy to follow and well structured**.
- Narrative arc: Problem → Impact → Solution → Differentiation → Proof → Call to Action.
- Each slide should transition naturally to the next.
- Use short, punchy text on slides. NO walls of text. Bullet points max 5 per slide.
- Visual aids: stat callouts, comparison tables, CSS-styled elements. Use emojis sparingly — at most 1-2 per slide and only when they add clarity, not decoration.

### 5. Proof / Credibility
**Examples or outcomes that build confidence**.
- Customer case studies: Accenture (developer happiness up 30%), Mercado Libre (shipping 2x faster), Duolingo, Shopify, Dow.
- Stats: 55% faster task completion (GitHub research), 46% of new code written by Copilot (across users), 1.3M+ paying businesses.
- Testimonials or quotes if possible.
- Mention Fortune 500 adoption and enterprise traction.

### 6. Pitch Readiness
The presentation must **sound ready for a real customer conversation**.
- Professional, confident tone. Not salesy — consultative.
- Presenter notes must include talking points, transition phrases, and objection-handling tips.
- End with a clear call to action (trial, POC, next meeting).

---

## Slide Structure (MANDATORY)

Generate exactly these slides in this order. Each slide is a `<section>` element. Use the CSS classes defined in the template (`center-slide`, `stat-number`, `highlight-box`, `two-column`, `competitor-table`, `github-icon`).

### Slide 1 — Title Slide
- Class: `center-slide`
- Include the official GitHub Invertocat (Octocat mark) as an inline SVG using the `.copilot-logo` class, filled with the Copilot purple-blue gradient. Use the real GitHub Invertocat SVG path — do NOT use an approximation or placeholder shape.
- Title: "GitHub Copilot" with a subtitle about AI-powered development
- Presenter: "Samuel Tauil | Microsoft"
- Notes: Quick intro, set the stage, mention what you'll cover

### Slide 2 — The Problem
- Title: a provocative question or bold statement about developer productivity challenges
- 3-4 bullet points describing the pain (talent gap, slow onboarding, context switching, technical debt)
- Use CSS-styled bullet markers (the `github-icon` class) instead of heavy emoji usage
- Notes: Expand on each pain point, ask rhetorical questions, connect to audience

### Slide 3 — The Cost of Inaction
- Use `stat-number` class for 2-3 impactful statistics (e.g., "60% of dev time isn't coding", "$85B lost to bad DX annually")
- Brief framing text around each stat
- Notes: Let the numbers sink in, pause after each stat, connect to their specific context

### Slide 4 — Introducing GitHub Copilot
- What it is in one sentence
- 3-4 key capabilities as `highlight-box` items (code completion, chat, CLI, PR reviews)
- Notes: Demo-style talking points — describe what it feels like to use it

### Slide 5 — How It Works (30-second version)
- Simple 3-step flow: Context → AI Model → Suggestion
- Mention multi-model (GPT-4o, Claude, Gemini)
- Keep it visual and simple — not overly technical
- Notes: Adjust depth to audience tech-savviness

### Slide 6 — Business Impact / Value
- Use `two-column` layout
- Left: developer outcomes (speed, quality, satisfaction)
- Right: business outcomes (delivery velocity, cost savings, retention)
- Each item backed by a specific number or case study reference
- Notes: Bridge from "cool tech" to "business case" — this is where you win the exec

### Slide 7 — Why GitHub Copilot Wins (Differentiation)
- Use `competitor-table` for a comparison matrix: GitHub Copilot vs. Cursor vs. Amazon Q vs. Tabnine
- Dimensions: IDE coverage, Enterprise security, Ecosystem breadth, Model choice, IP indemnity, Autonomous agents
- GitHub Copilot should clearly lead in most dimensions
- Notes: Don't trash competitors, but highlight unique strengths. Mention multi-model and coding agent.

### Slide 8 — Enterprise Ready
- 4-5 enterprise features as bullet points (use `github-icon` styled markers, not emojis)
- SSO/SCIM, IP indemnity, content exclusions, audit logs, policy controls, admin dashboard
- A brief mention of FedRAMP / compliance readiness
- Notes: This slide closes security/compliance objections. Emphasize IP indemnity.

### Slide 9 — Customer Proof Points
- 2-3 mini case studies with company name, metric, and outcome
- Use `highlight-box` for each
- Mention broad adoption: 1.3M+ businesses, Fortune 500 companies
- Notes: Name-drop relevant customers. Adapt to audience's industry if possible.

### Slide 10 — The Copilot Ecosystem
- Show breadth: Copilot in IDE, Chat, CLI, PR Reviews, Code Review, Workspace, Extensions, MCP, Coding Agent
- Brief one-liner for each
- Notes: Emphasize this is a platform, not a point tool. Mention extensibility.

### Slide 11 — Call to Action
- Class: `center-slide`
- Clear next step: "Start a free trial" / "Let's set up a POC" / "Book a deeper dive"
- Contact: Samuel Tauil — samuel.tauil@microsoft.com — github.com/samueltauil
- A memorable closing line
- Notes: Be direct. Suggest specific next steps. Offer to set up a pilot.

### Slide 12 — Thank You / Q&A
- Class: `center-slide`
- "Thank You" + invite questions
- Notes: Transition phrases for Q&A, common questions and answers to prepare for

---

## Reveal.js Technical Rules

1. **File to edit**: `src/index.html` — replace the placeholder comment block with slide `<section>` elements. Do NOT touch anything outside the `<div class="slides">` container (head, scripts, styles are already set up).
2. **Speaker notes**: Every slide MUST have `<aside class="notes">` with 3-5 sentences of talking points written as natural, readable prose — the presenter will read through them during the pitch. Notes should describe what to say about the slide content. Always end with a `Transition:` line. Do NOT include meta-instructions or coaching cues like "Let these numbers sink in", "Pause here", "Adjust depth", "This is the slide that wins", "Bridge from X to Y", or "Name-drop customers relevant to...". Do NOT mention specific time durations for the pitch (e.g., "15-minute conversation", "this will take 10 minutes") — the presenter decides the pacing live. Only include content the presenter would actually say out loud.
3. **Press S** to open speaker/presenter view — remind user of this.
4. **No external images** — use inline SVG, Unicode symbols, or CSS-styled elements for visual interest. Use emojis sparingly (1-2 per slide max, only for clarity).
5. **GitHub Logo** — Use the official GitHub Invertocat (Octocat mark) as an inline SVG on the title slide and wherever GitHub branding is needed. The logo should use the Copilot purple-blue gradient fill (`url(#copilot-grad)`). Use the official SVG path for the Invertocat mark (`M12 .297c-6.63...`) sourced from GitHub's brand assets — do NOT use a placeholder or approximation shape.
5. **Keep slide text concise** — max 5 bullet points per slide, max 8 words per bullet.
6. **Use the CSS utility classes** already defined in the `<style>` block: `center-slide`, `stat-number`, `highlight-box`, `two-column`, `competitor-table`, `github-icon`, `copilot-logo`, `gradient-text`.
7. **HTML only** — do not use the Markdown plugin for slides. Write raw HTML `<section>` elements.
8. **GitHub branding** — the presentation uses GitHub's dark theme colors. Use the Copilot purple-blue gradient (`gradient-text` class) for emphasis text. Use `github-icon` class for styled bullet markers instead of emojis.
9. **CRITICAL — Slide content MUST fit on screen without scrolling.** The slide viewport is 960×700px. Follow these hard limits to prevent overflow:
   - Max 4 `highlight-box` elements per slide (keep text inside each to 1 line)
   - Max 4 bullet points per slide for regular slides, max 5 only for `two-column` layouts (per column)
   - Max 3 stat blocks on stat slides (one `stat-number` + one short line each)
   - Competitor table: max 6 rows, keep cell text to 3-4 words
   - No extra `<p>` or `<div>` wrappers that add vertical space — keep markup flat
   - Prefer short, punchy text. If a slide feels dense, move content to speaker notes instead
   - Do NOT add `margin-top` greater than `1em` on any element

---

## Tone & Language

- **Professional and consultative**, not aggressive sales.
- **Confident** — speak as someone who knows the product deeply.
- **Customer-centric** — frame everything around their outcomes, not Microsoft features.
- Use "you" and "your team" in slide text. Avoid "we" (Microsoft) dominating.
- Presenter notes should be conversational — as if coaching someone to deliver the pitch.

---

## What NOT to Do

- Do NOT create additional files — only modify `src/index.html`.
- Do NOT add npm dependencies or change package.json.
- Do NOT change the Reveal.js theme, plugins, or configuration.
- Do NOT use Markdown slides — use HTML `<section>` elements.
- Do NOT use external images or assets.
- Do NOT generate more than 12 slides (keep it tight for a ~15 minute pitch).
- Do NOT add generic placeholder text like "Lorem ipsum" — every word must be real content.
- Do NOT commit or push the generated slides to git. The generated content in `src/index.html` is ephemeral — it should remain an uncommitted local change so the template stays clean for re-generation.
- Do NOT ask the user to commit or push.

---

## After Generating Slides

After filling in the slides, you MUST launch the server **idempotently** — every run must succeed regardless of prior state. Follow these steps exactly:

1. **Kill any existing process on port 8000** before starting a new server. Run: `lsof -ti:8000 | xargs kill -9 2>/dev/null; sleep 1` (this is safe even if nothing is running).
2. **Start the local server** by running `npx serve src -l 8000 --no-clipboard` (or `npm start`).
3. **Verify the server is running** by checking the process started and port 8000 is responding (e.g., `curl -s -o /dev/null -w "%{http_code}" http://localhost:8000`). The HTTP status must be `200`. If it is not, diagnose and retry.
4. **Only after verification succeeds**, present the URL to the user: `http://localhost:8000`
5. **Remind the user** to press **S** to open the speaker/presenter view with notes.

Do this automatically — do not ask for permission or confirmation. The user expects to see a working URL immediately after generation. Never present the URL without first confirming the server is responding.
