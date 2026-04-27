# hosq curator workspace — UX prototype

Interactive UX prototype for the HOSQ foundation curator tool. Lets a curator upload a project essay or PDF, see it parsed into the v7 schema (18 phases, 86 fields), and improve the application with AI feedback scored against the 10-vector / 39-subindex HOSQ rubric.

**Two modes**, switchable at any time via the top-bar toggle:

- **Writing mode** — quiet AI: top-3 weak spots + contextual coach for the selected paragraph.
- **Scoring mode** — cockpit AI: all 10 vectors visible, click to drill into 39 sub-indices and highlight the paragraphs driving each score.

Single static HTML file — no build, no backend. All "scoring" and "AI" interactions are mocked for UX testing only.

## Stack
- Plain HTML / CSS / JS — one file (`index.html`)
- Cera Pro woff fonts (HOSQ brand, self-hosted in `fonts/`)
- HOSQ design tokens (cream / coral / violet / dark) per brand spec

## Local
Open `index.html` in any browser, or:
```bash
python3 -m http.server 8000
# → http://localhost:8000/
```
