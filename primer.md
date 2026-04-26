# AI Art Class Presentation — Primer

## Current Status
Presentation is functional and serveable. Webcam energy conductor has 4 modes, 5 color themes, toggles, keyboard shortcuts. Slide editor built. All running at localhost:8082.

## What Changed (Session 2026-04-25)
- Built full reveal.js 6.0.1 presentation (13 horizontal sections, vertical drill-downs)
- Extracted images from BrownBag PowerPoint (benchmark chart, METR growth, AI-as-UI diagram)
- Took 1920x1080 Playwright screenshots of DejaViewed, Graph Cosmos, portfolio
- Built webcam-energy.html: MediaPipe hand tracking + Canvas 2D neon effects
- Iterated on visualizer: removed palm beam + particles, added pinch effects, optimized batching
- Made lightning mode blue/realistic with recursive branching forks
- Added 5 color themes (neon/electric/fire/matrix/vapor)
- Added toggle controls: skeleton, nodes, pinch FX, mirror cam, lite mode
- Added keyboard shortcuts: 1-4 modes, H/F/S/N/P/L
- Updated presentation Section 12 with actual prompt slides + short version (42 words)
- Built editor.html — slide card editor that exports slides.json
- Moved Kay's bird files to KayDubs/kaydubs-birds/

## Next Up
1. Victor test webcam-energy.html latest (lightning, themes, toggles)
2. Victor review/edit slides in editor.html, save slides.json
3. I compose slides.json into index.html if Victor changes content
4. Find "All-Seeing Eye" project and integrate
5. Integrate Websites project (Three.js cosmos hero)
6. Content refinement pass based on Victor's feedback
7. Deploy to 1gabe.com/demo/ if time
8. Get wireless presenter/clicker for Monday

## Blockers
- None critical. Presentation is usable as-is.

## Open Questions
- "All-Seeing Eye" project — what folder?
- Does Victor want webcam-visualizer.html (WebGL shaders) kept in the presentation too, or just energy conductor?
- Deploy strategy for 1gabe.com?

## Don't Forget
- reveal.js 6.0.1 plugin paths are `dist/plugin/` not `plugin/` (v6 breaking change)
- Dev server: `npx serve -l 8080` from ai_art_class/
- Playwright MCP can connect to existing Chrome via CDP port 38117 for authenticated screenshots
- Victor's audience is skeptical art faculty — tone matters
