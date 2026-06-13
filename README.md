# Synapse — Organisation Brain

An interactive **organisation brain**: every team, human, AI agent, tool, workflow, SOP and project of a company on a single force-directed canvas — click any node to inspect a full profile. Apple design language, inspired by the "Conducting AI" org-graph concept.

🔗 **Live demo:** https://synapse-vert-one.vercel.app

> Demo company **Northwind AI** (fictional Series-B SaaS): 121 nodes / 343 links — 27 people, 60 AI sub-agents, 8 departments, 6 teams, 10 tools, 4 projects, 3 workflows, 2 SOPs.

## Highlights
- **Force-graph canvas** — drag / zoom / pan; hover highlights a node's 1-hop neighbourhood; click opens a profile + centers.
- **Profile drawer** — per-type tabs. People: Overview / Work / AI Access / Activity / Compliance (with reporting structure). AI agents: Mission / Operating Rules / Vibe / Tools / Access + source provenance.
- **Sidebar** — search, entity-type filters with live counts, Core/Enabling function filters, selected-node mini-card.
- **Deep links** — `?node=<id>` selects + focuses on load. Keyboard: `/` search, `Esc` close.

## Stack
Vanilla HTML/CSS/JS, **no build step**. force-graph (2D canvas) · GSAP · DiceBear · Simple Icons (CDN). Design tokens mapped from the Apple design system. AI-agent content sourced from real role definitions.

---

*Source code is private. This repo is the public overview.*
