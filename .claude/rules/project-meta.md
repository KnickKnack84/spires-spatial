# Project meta — Spires Spatial

| Field | Value |
|---|---|
| **Name** | Spires Spatial (website) |
| **Tier** | build |
| **Language** | HTML / CSS / vanilla JS (single static file) |
| **Build system** | none — `index.html` is the artifact |
| **Serena** | not used (single file, no symbol intelligence needed) |
| **Codex policy** | advisory only / not required (build-tier, no merge gate) |
| **Review policy** | CodeRabbit on PRs is enough; `/ultrareview` optional for big changes; no Codex Stage-3 gate (not kernel-tier) |
| **Default TDD skill** | n/a (static marketing site — no test suite) |
| **Hosting** | GitHub Pages (repo `KnickKnack84/spires-spatial`); long-term may move to Cloudflare Pages to match the SPP/Websites pattern + allow a private repo |
| **GitHub repo** | `KnickKnack84/spires-spatial` |
| **Worktrees** | not needed (single file); if ever needed → `C:\Users\Nicholas\dev\spires-spatial-worktrees\` (outside OneDrive) |
| **Status** | under development — client demo in progress |

## Notes
- This is a deliberately dependency-free single-file static site. Don't introduce frameworks, bundlers, or a `src/` split unless there's a real need.
- `index.html` MUST stay at the repo root (GitHub Pages requirement) — the "no working files in root" rule doesn't apply; this file IS the deliverable.
- Public repo currently (so free-tier GitHub Pages works). Switch to private + Cloudflare Pages if/when this stops being a throwaway prospect demo.
