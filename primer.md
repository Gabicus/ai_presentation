# AI Art Class Presentation · primer

Updated: 2026-04-27 (afternoon)

## Current status

Reveal.js 6.0.1 presentation for Fairmont State AI & Art class. **Due Monday April 28, 2026.**
Runs locally: `python3 -m http.server 8080` from `ai_art_class/` dir.
Live online: `https://dejaviewed.dev/ai_presentation/`
GitHub: `git@github.com:Gabicus/ai_presentation.git` (main branch).

Reveal.js loads from `reveal-dist/` (committed) — works offline and online, no npm install needed.

## What changed (this session)

- Deleted slide groups: "Then AI Happened", "The Real Question", "The Takeaway"
- Deleted "Career Intelligence System" and "Three.js Cosmos Hero" slides
- Added devil's advocate section (foundation matters, Marcy Bridge, Skynet/Terminator, environmental cost/ManBearPig, blank page is gone)
- Added citation tree slide to "Work I've Done with AI" section
- Added standalone Three.js cosmos scene (`cosmos-standalone/index.html`)
- Moved "Deeper Dives" and "Design Resources" into DejaViewed section
- "My Creative Portfolio" → vertical sub-slide under final "What Will You Build?"
- Cosmos graph slide URL → `https://dejaviewed.dev/graph-cosmos`
- Iframes use `data-src` for lazy loading (GPU was 100%)
- Intro slide images: 82vh (fit fullscreen with name text)
- Fixed ASE Evolution grid, terminator image container
- RAM cleanup: 13GB DuckDB temps from `/tmp`, 6GB chroma-mcp from swap
- Switched reveal.js refs from `node_modules/` to `reveal-dist/` for portability
- Deployed to dejaviewed.dev/ai_presentation via dejaviewed-plugin (had to fix *.png gitignore)

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
- `reveal-dist/` — committed reveal.js CSS/JS/plugins (no npm needed)
- `cosmos-standalone/index.html` — standalone Three.js cosmos (942 lines)
- `all-seeing-eye/` — Next.js static export of ASE
- `webcam-energy.html` — hand-tracking visualizer for live demo
- `editor.html` — slide authoring tool
- `img/` — all presentation images

## Deploy notes

- Online copy synced to `dejaviewed-plugin/site/ai_presentation/`
- dejaviewed-plugin `.gitignore` has `*.png` — exception added for `site/ai_presentation/**/*.png`
- Any future changes need syncing: copy updated files to dejaviewed-plugin, commit+push both repos

## Next up

- Practice run-through with webcam demo before Monday
- Verify fullscreen looks good on projector resolution

## Don't forget

- Audience: mixed students + skeptical art faculty — tone matters
- Webcam demo needs good lighting, two hands visible
- Two repos to sync: ai_presentation (source) + dejaviewed-plugin (deploy)
