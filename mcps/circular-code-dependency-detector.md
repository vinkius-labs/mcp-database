# Circular Code Dependency Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/circular-code-dependency-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Identify import cycles and measure module interdependence in JavaScript, TypeScript, and Python projects.

## Description
This MCP server provides specialized tools to prevent runtime initialization errors caused by circular dependencies. Use `scan_dependencies` to build a dependency map of your project, `detect_cycles` to find exact loop paths like A -> B -> C -> A, and `compute_coupling_metrics` to identify critical bottleneck modules using in-degree and out-degree analysis.


## Available Tools (3)
- **compute_coupling_metrics**: Compute coupling metrics for a module
- **detect_cycles**: Detect circular dependencies
- **scan_dependencies**: Scan a directory for dependencies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circular Code Dependency Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan my current directory for dependencies and tell me if there are any cycles."

**🤖 AI Agent:**
> The scan completed successfully. No circular dependencies were detected in the current dependency map.

---

**👤 You:**
> "Check for cycles in this dependency map: {"src/index.ts": ["src/utils.ts"], "src/utils.ts": ["src/index.ts"]}"

**🤖 AI Agent:**
> A cycle was detected: ['src/index.ts', 'src/utils.ts', 'src/index.ts'].

---

**👤 You:**
> "How coupled is the module 'auth_service.py'?"

**🤖 AI Agent:**
> The module 'auth_service.py' has an in-degree of 5 and an out-degree of 2, indicating a moderate coupling level.


## ❓ FAQ

**Q: How do I start detecting cycles in my project?**
First, use the `scan_dependencies` tool on your project directory to generate a dependency map. Then, pass that map into `detect_cycles` to see all identified loops.

**Q: Can I analyze Python projects?**
Yes, the scanner supports `python` syntax alongside `javascript` and `typescript`.

**Q: What are coupling metrics?**
They quantify module interdependence. By using `compute_coupling_metrics`, you can see the in-degree and out-degree of a module to find high-risk files.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/circular-code-dependency-detector](https://vinkius.com/mcp/circular-code-dependency-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circular Code Dependency Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `circular-code-dependency-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circular Code Dependency Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circular-code-dependency-detector": {
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
