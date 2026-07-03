# FoldPlan MCP static explanation page

This folder is a small static GitHub Pages surface for explaining the FoldPlan
MCP safety model.

It intentionally does not change:

- Flutter app routing
- `foldplan.com`
- Cloudflare Pages or DNS settings
- MCP runtime behavior
- backend/API/auth/session behavior

The page source lives under `docs/mcp/`, but do not configure branch-based
GitHub Pages to publish this repository's entire `/docs` folder. This repo also
contains internal planning, security, and operations notes under `docs/`.

Safe publishing should use a dedicated publish branch or a future GitHub Pages
Actions artifact that contains only the contents of `docs/mcp/`. This PR does
not change repository Pages settings, custom domains, workflows, or production
deployment pipelines.

Local preview:

```bash
python3 -m http.server 4173 --bind 127.0.0.1 --directory docs/mcp
```

Open `http://127.0.0.1:4173/` from the repository root. This repository
intentionally does not add a Gemfile, package script, or Pages workflow for the
page; avoid dependency churn unless the coordinator explicitly asks for a
publish pipeline.
