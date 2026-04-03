# PlanetCorps AI Academy

A multi-program learning platform for AI certification study. Each program is a self-contained course with curriculum modules, assessments, glossary, exercises, and progress tracking.

## Programs

### Claude University
**Claude Certified Architect – Foundations** certification prep.

| Domain | Name | Weight |
|--------|------|--------|
| 1 | Agentic Architecture & Orchestration | 27% |
| 2 | Tool Design & MCP Integration | 18% |
| 3 | Claude Code Configuration & Workflows | 20% |
| 4 | Prompt Engineering & Structured Output | 20% |
| 5 | Context Management & Reliability | 15% |

- 5 curriculum modules covering all 27 task statements
- 57 practice questions (39 domain + 18 scenario-based)
- 4 hands-on exercises
- 4-phase study plan with checkpoints
- Searchable glossary (44 terms)

Content lives in `programs/claude-university/`.

## Adding a New Program

1. Create a folder under `programs/` (e.g., `programs/prompt-engineering-mastery/`)
2. Add a `program.json` manifest defining modules, assessments, and resources
3. Add content files in `curriculum/`, `assessments/`, and `docs/` subdirectories
4. Restart the server — the program is auto-discovered

See `programs/claude-university/program.json` for the manifest format.

## Running

```bash
npm install
npm start        # http://localhost:3009
```

## Tech Stack
- Express.js on port 3009
- Vanilla JavaScript SPA
- JSON file-based persistence (per-user, per-program)
- Marked.js for markdown rendering
- Quicksand font, PlanetCorps light theme
