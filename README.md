# architecture-tradeoff-simulator
An interactive browser-based prototype that visualizes how common infrastructure choices impact latency, cost, reliability, and system complexity in real time. Built with Three.js and vanilla HTML/JS as a thinking and communication tool.
This tool simulates how common infrastructure decisions — caching, queues, multi-region deployments, rate limiting, traffic volume, and payload size — affect latency, cost, reliability, and overall system complexity in real time.

It is intentionally simplified and designed as a **thinking and communication tool**, not a production-grade capacity planner.

---

## What this is

- A single-file web app (HTML + JS)
- Runs entirely in the browser
- Uses Three.js to visualize system components and request flow
- Updates metrics live as configuration changes

The goal is to make tradeoffs *visible* so they are easier to reason about and explain.

---

## What this is not

- Not a precise cost calculator
- Not a performance benchmarking tool
- Not tied to any specific cloud provider

The math is deterministic and opinionated by design.

---

## Features

- Interactive 3D system diagram
- Real-time metric simulation:
  - Estimated p95 latency
  - Estimated monthly cost
  - Reliability score
  - Complexity score
- Infrastructure toggles:
  - CDN
  - Cache
  - Queue
  - Multi-region
  - Read replicas
  - Rate limiting
- Load controls:
  - Requests per second
  - Payload size
  - Cache hit rate
- Scenario presets for common system profiles
- Clickable components with contextual explanations
- Runs locally or on static hosting (Netlify / GitHub Pages)

---

## Tech Stack

- HTML / CSS / JavaScript
- Three.js (ES modules via CDN)
- No build tools
- No frameworks
- No backend

---

## How to run

### Option 1: Local
1. Download or clone the repo
2. Open `index.html` in a modern browser

### Option 2: Static hosting
Deploy directly to:
- Netlify
- GitHub Pages
- Any static file host

No configuration required.

---

## Design philosophy

Most architecture discussions happen with whiteboards, static diagrams, or spreadsheets.

This project explores a different approach:
- Show how systems *behave*, not just how they are shaped
- Make tradeoffs obvious through motion and interaction
- Encourage clearer conversations around constraints and priorities

---

## Possible future improvements

- Custom, user-defined calculation models
- Exportable/shareable scenarios
- Constraint-based goals (e.g. “keep p95 under 200ms”)
- Metric breakdowns by component
- Collaboration or annotation features

---

## License

MIT

---

Built as an exploration of modern browser capabilities and visual system reasoning.
