# Spires Spatial — Master Development

> Single source of truth. Read first every session; update at the end of every session.

## What this is
Marketing website for **Spires Spatial** (Hal Spires) — 3D property tours / dollhouse views / measured floor plans / digital twins for real-estate listings in Middle Georgia. Single self-contained static `index.html` (inline CSS/JS, CDN fonts + imagery, no build step). Deployed via GitHub Pages.

## Current state (2026-05-11)
- ✅ Hero: 3-mode interactive viewer — **Photo · Dollhouse · Floor Plan** — mirroring the Matterport/Asteroom product UI. Pill toggle; one-time auto-tour on first load (Photo → Dollhouse → Floor Plan → Photo, then hands control back); View Transitions API cross-fade; keyboard-navigable; respects `prefers-reduced-motion`.
  - Photo mode: bright living-room interior; on hover, Matterport-style measurement annotation pins (ceiling/window/door) + a "Will my sofa fit through the door?" callout with a mini SVG door+sofa diagram.
  - Dollhouse mode: detailed hand-coded axonometric cutaway (floor slab, walls, 9 interior partitions, 7 furniture pieces, roof outline, 2 dimension callouts, 10 room labels) — on warm paper, ink+bronze line art. "Sketches itself" element-by-element on entering the mode.
  - Floor Plan mode: detailed top-down 2D plan matching the dollhouse (7 swing doors, 8 windows, fixtures/furniture, segmented dimension lines, north arrow, scale bar, room labels w/ sq ft). Also sketches itself in.
- ✅ Hero kicker: "Middle Georgia · Real Estate 3D Photography & Measurement Services" (12.5px, ink — more prominent than the section kickers).
- ✅ "How it works" steps: hand-coded SVG line illustrations (no photos): (1) top-down capture-route map w/ 6 numbered scan dots + dashed route + 360° camera glyph; (2) "from one scan" → three panels (photo → isometric measured 3D wireframe → 2D floor plan) w/ flow arrows; (3) "one link, everywhere" → central 3D-tour card w/ dashed connectors to a browser/MLS window, a phone, an envelope, a social glyph. Groups fade+lift in on scroll.
- ✅ "Why agents call back" — 4-card dark section. ✅ Showcase — twilight-home photo + "Walk through" play button w/ pulsing rings. ✅ Pricing — 3 tiers ($125 residential / $175 commercial single / $100/suite multi); featured card has a gold underglow. ✅ Contact — phone, email, service area.
- ✅ Branding "Spires Spatial" throughout (wordmark, title, footer). Footer: "Spires Spatial · Macon, GA · Owner: Hal Spires".
- ✅ Verified: zero console errors, all 16 anchor links resolve, all images load.

## Open / next
1. **Confirm the business name "Spires Spatial"** with Hal. (Alternatives considered: Verisite, Vantage 3D.)
2. Logo / wordmark — currently a text mark "*Spires* Spatial"; does he want a graphic mark?
3. Swap placeholder stock photos (hero living-room, showcase twilight house) → Hal's real listing photos.
4. "View sample tour" CTA → point at a real Asteroom embed URL.
5. Hosting decision — currently GitHub Pages (public repo). Long-term: Cloudflare Pages (matches the SPP/Websites pattern, allows a private repo) + a custom domain (`spiresspatial.com`?). Get a domain email too (`hal@spiresspatial.com`).
6. Possible: a 4th "Measurements" hero mode if Hal wants to spotlight that; an "About Hal" blurb; testimonials once he has them.

## Deploy / preview
- Repo: `KnickKnack84/spires-spatial` (public — required for free GitHub Pages).
- Live URL: see GitHub Pages settings / the repo's Environments. (Form `https://knickknack84.github.io/spires-spatial/`.)
- Local preview: open `index.html`, or `python -m http.server 8000 --bind 127.0.0.1` from this folder → http://127.0.0.1:8000/.
- To push updates: edit `index.html`, commit, `git push` → Pages auto-rebuilds in ~1 min.

## Session log
- **2026-05-11** — Formalized into this project folder under `OneDrive\Desktop\Spires Spatial\`; created repo `KnickKnack84/spires-spatial`; deployed via GitHub Pages for a client-shareable link. (Prior iteration history lived in the scratch folder `Desktop\HalSpires3D\`, now superseded.)
