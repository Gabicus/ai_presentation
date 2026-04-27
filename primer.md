# AI Art Class Presentation · primer

Updated: 2026-04-27

## Current status

Reveal.js 6.0.1 presentation for Fairmont State AI & Art class. **Due Monday April 28, 2026.**
Runs locally: `python3 -m http.server 8080` from `ai_art_class/` dir.
Pushed to GitHub: `git@github.com:Gabicus/ai_presentation.git` (main branch).

## What changed (this session)

- Deleted 3 slide groups: "Then AI Happened", "The Real Question", "The Takeaway"
- Deleted "Career Intelligence System" and "Three.js Cosmos Hero" slides
- Added devil's advocate section (foundation matters, Marcy Bridge, Skynet/Terminator, environmental cost/ManBearPig, blank page is gone)
- Added citation tree slide to "Work I've Done with AI" section
- Added standalone Three.js cosmos scene (`cosmos-standalone/index.html`) — vanilla, no React
- Moved "Deeper Dives" and "Design Resources" into DejaViewed section
- "My Creative Portfolio" moved to vertical sub-slide under final "What Will You Build?" slide
- Cosmos graph slide URL corrected to `https://dejaviewed.dev/graph-cosmos`
- Iframes for ASE and Cosmos use `data-src` for lazy loading (GPU was hitting 100%)
- Fixed slide 0/1 images: global CSS `max-height: 55vh` was overriding, added `max-height: 95vh` inline
- Fixed ASE Evolution grid: `grid-template-rows: 1fr 1fr`, `object-fit: cover`, `max-height: 72vh`
- Fixed terminator image container: `flex: 0` → `flex: 1`
- RAM cleanup: 13GB stale DuckDB temps from `/tmp`, 6GB chroma-mcp from swap
- Git initialized, committed, pushed to GitHub

## Section structure (horizontal groups)

1. Title + Intro (name, PE, images)
2. AI Today (what it can do)
3. But We've Seen This Before (photography → 3D printing → AI, South Park meme)
4. The Pattern (Photoshop 1990s, Digital Photography 2000s, 3D Printing 2010s, AI 2020s)
5. What Changes (what AI adds to creative workflow)
6. Work I've Done with AI (NETL portfolio, brownbag slides, citation tree)
7. DejaViewed (site, deeper dives, design resources, cosmos graph)
8. All-Seeing Eye (evolution grid, ASE live iframe, 3D Cosmos live iframe)
9. Devil's Advocate (foundation matters, Marcy Bridge, Skynet, environmental cost, blank page gone)
10. Live Build (prompt demo, webcam energy conductor)
11. What Will You Build? + My Creative Portfolio (vertical sub-slides)

## Key files

- `index.html` — main presentation (~950 lines)
- `cosmos-standalone/index.html` — standalone Three.js cosmos (942 lines)
- `all-seeing-eye/` — Next.js static export of ASE
- `webcam-energy.html` — hand-tracking visualizer for live demo
- `editor.html` — slide authoring tool
- `img/` — all presentation images

## Deploy notes

- GitHub: `git@github.com:Gabicus/ai_presentation.git`
- Cloudflare (dejaviewed.dev/ai_presentation): possible but needs reveal.js dist copied — index.html refs `node_modules/reveal.js/dist/`. Not set up yet.
- After clone: `npm install` to get reveal.js

## Next up

- Verify all slides in browser before Monday
- Consider CDN for reveal.js if deploying to Cloudflare
- Practice run-through with webcam demo

## Don't forget

- reveal.js 6.0.1 plugin paths: `dist/plugin/` not `plugin/`
- Audience: mixed students + skeptical art faculty — tone matters
- Webcam demo needs good lighting, two hands visible
