# Synapse — the fabius operating console

The console one agent is operated from. fabius runs on every major model — Anthropic, OpenAI, Google, Mistral, Groq — under a single stance: **scout wide, strike narrow**. Synapse is the surface that makes that stance visible and drivable: the agent's own architecture rendered as a force-directed graph, and nine views that turn the graph into a working control room.

🔗 **Live:** https://synapse-vert-one.vercel.app

## The nine views

| View | What it does |
| --- | --- |
| **Graph** | The whole system as a canvas. Drag, zoom, hover to light up a node's neighbourhood, click for a full profile. |
| **Org** | Top-down structure: the agent, its layers, and the specialists under each. |
| **System** | A live map of the nervous system — router, lean core, skill layers, spine — with real counts. |
| **Cockpit** | Describe a mission, get a plan as a DAG, run it in resumable waves with an approvals inbox. |
| **Chat** | Talk to the agent directly; every turn is routed by layer, machinery and model tier. |
| **Missions** | A kanban of work; each card can open a flow or hand off to a single specialist. |
| **Memory** | Semantic recall over a compounding corpus, verify-gated so only certified output grounds later decisions. |
| **Operator** | fabius as a persistent background agent: a D1-checkpointed step-then-verify loop, a cron heartbeat, routines and an artifact store. |
| **Dashboard** | KPI rollups and an activity feed over everything above. |

## Stack

Vanilla HTML/CSS/JS, **no build step** — decoupled modules that talk only through a read-only global and a document event bus. force-graph (2D canvas) and GSAP via CDN. Backend is a Cloudflare Worker with D1 as the source of truth, Vectorize plus Workers AI for embeddings, and a five-provider runtime behind one routing contract. Every `/api/*` call is token-authenticated.

---

*Source code is private. This repo is the public overview. The agent itself is open: [ArielShemesh1999/fabius](https://github.com/ArielShemesh1999/fabius).*
