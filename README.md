# Copilotception

A **GitHub Copilot pitch presentation** built with [Reveal.js](https://revealjs.com/) — generated entirely by GitHub Copilot itself.

## What Is This?

This repo contains a Reveal.js presentation template that pitches GitHub Copilot to customer audiences. The slides are **not stored in the repo** — they are generated on-the-fly by GitHub Copilot using the instructions and evaluation criteria defined in this project.

The concept: **GitHub Copilot generates a presentation about GitHub Copilot.** Hence the name — *Copilotception*.

## How It Works

1. Open this repo in an IDE with GitHub Copilot (e.g., VS Code).
2. Ask Copilot to generate the presentation (e.g., *"generate my presentation"*).
3. Copilot reads the instructions in `.github/copilot-instructions.md`, the evaluation criteria in `requirements/`, and the slide authoring rules in `.github/instructions/` — then fills in `src/index.html` with a complete set of slides.
4. A local server starts automatically and you get a URL to view the presentation.
5. Press **S** in the browser to open the speaker/presenter view with talking-point notes.

## Project Structure

```
.github/
  copilot-instructions.md          # Main instructions for slide generation
  instructions/
    revealjs-slides.instructions.md  # Reveal.js authoring rules & CSS classes
    requirements.instructions.md     # Maps evaluation criteria to slides
  prompts/                           # Reusable prompt files
requirements/
  criterias.txt                      # Evaluation criteria for the pitch
src/
  index.html                         # Reveal.js template (slides generated here)
package.json                         # npm scripts (start, dev)
```

## Quick Start

```bash
# Clone the repo
git clone https://github.com/samueltauil/copilotception.git
cd copilotception

# Ask GitHub Copilot to generate the presentation
# (in your IDE or Copilot CLI, just say "generate my presentation")

# Or manually serve the template
npm start
# → http://localhost:8000
```

## Presenter

**Samuel Tauil** — Microsoft  
📧 samuel.tauil@microsoft.com  
🐙 [github.com/samueltauil](https://github.com/samueltauil)

## Notes

- Generated slides in `src/index.html` are **ephemeral** — they are not committed to the repo. The template stays clean for re-generation.
- The presentation is scored on 6 criteria: Problem Clarity, Value Articulation, Microsoft Differentiation, Storytelling & Flow, Proof/Credibility, and Pitch Readiness.
- Every slide includes speaker notes with talking points, transitions, and objection-handling tips.

## License

Internal use — Microsoft.
