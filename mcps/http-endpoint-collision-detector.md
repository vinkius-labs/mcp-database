# HTTP Endpoint Collision Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/http-endpoint-collision-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [web-development](../categories/web-development.md)

Detect overlapping or conflicting HTTP route definitions in your codebase.

## Description
This MCP server identifies shadowing and duplication in HTTP routes across Express, FastAPI, Spring, and Django. Use `extract_raw_routes` to scan your project directory for route definitions. Then, run `analyze_route_collisions` to find exact matches or parameterized shadowing. You can also use `verify_path_equivalence` to check if two paths are functionally identical under normalization rules.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **HTTP Endpoint Collision Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any route conflicts in my Express project at /workspace/my-app?"

**🤖 AI Agent:**
> The `analyze_route_collisions` tool found 1 conflict: `/users/:id` shadows `/users/me`.

---

**👤 You:**
> "Check if `/api/v1/users/{id}` and `/api/v1/users/:id` are the same."

**🤖 AI Agent:**
> Yes, both paths are functionally equivalent after normalization.

---

**👤 You:**
> "Scan my project for routes."

**🤖 AI Agent:**
> The `extract_raw_routes` tool found 5 routes in your project.


## ❓ FAQ

**Q: How does it detect collisions?**
It uses `analyze_route_collisions` to build a routing tree and identify overlapping patterns. Tools available: `your_tool_name`.

**Q: Which frameworks are supported?**
The server supports Express, FastAPI, Spring, and Django.

**Q: Does it require API keys?**
No, this MCP server connects via Vinkius Edge without needing vendor credentials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/http-endpoint-collision-detector](https://vinkius.com/mcp/http-endpoint-collision-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HTTP Endpoint Collision Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `http-endpoint-collision-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HTTP Endpoint Collision Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "http-endpoint-collision-detector": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
