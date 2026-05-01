# HermesMade Site (China Mirror)

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-success?style=flat-square&logo=github)](https://minirr890112-byte.github.io/hermesmade-site-cf/)
[![China Accessible](https://img.shields.io/badge/China%20Accessible-No%20GFW%20Block-red?style=flat-square)](https://minirr890112-byte.github.io/hermesmade-site-cf/)
[![Neo-Brutalist](https://img.shields.io/badge/Design-Neo--Brutalist-orange?style=flat-square)](https://minirr890112-byte.github.io/hermesmade-site-cf/)
[![No CDN](https://img.shields.io/badge/Zero%20CDN-Self--Contained-blue?style=flat-square)](https://minirr890112-byte.github.io/hermesmade-site-cf/)

> A China-accessible mirror of **HermesMade** — pain-driven CLI tools for developers who are tired of broken APIs, vanishing free tiers, and undocumented AI services.

---

## What Is This?

**HermesMade** is a suite of CLI tools that scrape real developer pain signals from V2EX, Reddit, CSDN, and Juejin. The official site is deployed on **Vercel** — but Vercel is blocked by the Great Firewall of China (GFW).

This repository hosts a **static mirror** served via **GitHub Pages** so developers inside China can access the site without a VPN. Everything is self-contained: no external CDN dependencies, no trackers, no JavaScript.

-   **Live mirror:** [minirr890112-byte.github.io/hermesmade-site-cf](https://minirr890112-byte.github.io/hermesmade-site-cf/)
-   **Main repo:** [github.com/minirr890112-byte/HermesMade](https://github.com/minirr890112-byte/HermesMade)

---

## Design

The site uses a **neo-brutalist** aesthetic:

| Element | Detail |
|:--------|:-------|
| Font | JetBrains Mono (system fallback: Fira Code, SF Mono) |
| Background | `#0a0a0a` with SVG noise overlay |
| Text | `#f0f0f0` |
| Accent | `#ff6b35` (burn orange) |
| Cards | Hard drop-shadow (`6px 6px 0`), thick borders, glitch effects |
| Responsive | Clamped typography, mobile-friendly cards |

Zero JavaScript. Zero external CDN fetches. Works behind the GFW.

---

## Tools Showcased

Seven HermesMade CLI tools are featured on the mirror site:

| Tool | What It Does |
|:-----|:-------------|
| `api-cost-compare` | Compares LLM API pricing across providers, alerts on token inflation and subscription bloat. |
| `code-inspector` | Audits codebases for security flaws, performance issues, and anti-patterns. |
| `llm-deploy-helper` | Deploys 30B-parameter models on consumer GPUs (8 GB VRAM) without Docker. |
| `model-watch` | Tracks AI model quality degradation across version upgrades (e.g., GPT-5.4 → 5.5). |
| `prompt-inspector` | Detects hallucination, censorship, and prompt-injection vulnerabilities in LLM endpoints. |
| `task-cost-estimator` | Estimates compute cost and token usage for a given task before you run it. |
| `v2ex-pain-scanner` | Scrapes V2EX forums to surface trending pain points from the Chinese dev community. |

---

## Why a Mirror?

-   Vercel’s default `*.vercel.app` domain is blocked by the GFW.
-   Many Chinese developers browse without reliable VPN access.
-   GitHub Pages is reachable from mainland China (though sometimes slow).
-   The mirror uses **zero external resources** — fonts are system-stack, the noise texture is inline SVG, and there are no third-party scripts.

This ensures the page renders correctly even under deep packet inspection and intermittent connectivity.

---

## Quick Start

```bash
# Clone the mirror
git clone https://github.com/minirr890112-byte/hermesmade-site-cf.git

# Serve locally (Python 3)
cd hermesmade-site-cf
python3 -m http.server 8080
# Open http://localhost:8080
```

For the actual CLI tools, see the [main HermesMade repository](https://github.com/minirr890112-byte/HermesMade).

---

## Structure

```
hermesmade-site-cf/
├── index.html        # Main landing page (296 lines, pure HTML + CSS)
├── dashboard.html    # Live pain-point dashboard
└── README.md         # This file
```

---

## License

MIT — same as the main HermesMade project.

---

*Built with pain. Deployed via GitHub Pages. No JS. No tracking. No BS.*
