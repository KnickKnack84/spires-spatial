# Spires Spatial — project Claude Code config

## WHY
Marketing website for Spires Spatial (Hal Spires, Nicholas's brother) — 3D property tour / measurement services for real-estate listings in Middle Georgia. Goal: replace the placeholder Google Sites page with a polished site that helps Hal land residential and commercial clients. **Status: under development** — being shown to a potential client; iterating on content, name confirmation, real photos, and hosting.

## WHAT — the build
- Single self-contained static page: `index.html` (inline CSS/JS, CDN fonts + imagery). No build step, no deps.
- Deployed via GitHub Pages (repo `KnickKnack84/spires-spatial`).
- Aesthetic: editorial/architectural — Fraunces (display) + Instrument Sans (body) + JetBrains Mono (labels); ink `#14110F` / warm bone `#F4EFE6` / bronze `#A87B4F` / aged-gold `#C9A961`.
- Hero = 3-mode interactive viewer (Photo · Dollhouse · Floor Plan) mirroring Matterport/Asteroom UI; View Transitions API; one-time auto-tour on first load.
- "How it works" steps = hand-coded SVG line illustrations (not photos).

## HOW — working on it
- Edit `index.html` directly. To preview: open the file in a browser, OR `python -m http.server 8000 --bind 127.0.0.1` from this folder and visit http://127.0.0.1:8000/.
- After UI changes, verify in a real browser (golden path + the hero mode toggle + hover states).
- `index.html` lives at the repo root — required by GitHub Pages. (This is the deliverable, not a "working file" — the root-folder rule doesn't apply to it.)
- Keep it dependency-free and single-file unless there's a strong reason to split.

## File organization
`index.html` at root (Pages requirement). `README.md`, `.gitignore`, `.nojekyll`, `CLAUDE.md` at root. Project docs in `development/`. Per-project rules in `.claude/rules/`.

## Pointers
- Single source of truth: `development/MASTER_DEVELOPMENT.md` (read first every session, update at end).
- Cross-session context + open questions: `~/.claude/projects/C--Users-Nicholas/memory/project_hal_spires_3d.md`.
- Tier / language / policy: `.claude/rules/project-meta.md`.

## important-instruction-reminders
Do what has been asked; nothing more, nothing less. Prefer editing the existing file over creating new ones. Don't add build tooling/frameworks unless asked — this is intentionally a single static file.
