# FoldPlan MCP

Public static user guide for FoldPlan MCP.

The page explains how MCP-supported AI tools can connect to FoldPlan, which
tools are available, how to test the MCP endpoint, and what is still limited to
private beta or development access.

Published URL:

```text
https://jybin00.github.io/foldplan-mcp/
```

This repository intentionally contains only the public static page files. It
does not configure or change:

- Flutter app routing
- `foldplan.com`
- Cloudflare Pages or DNS settings
- MCP runtime behavior
- backend/API/auth/session behavior

Local preview from this repository:

```bash
python3 -m http.server 4173 --bind 127.0.0.1
```

Open `http://127.0.0.1:4173/`.
