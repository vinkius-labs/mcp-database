# Astro Server Island Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/astro-server-island-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [web-development](../categories/web-development.md)

Extracts Astro Server Island directives from HTML/JSX to prevent misconfigured streaming SSR components.

## Description
The Astro Server Island Detector is a specialized MCP server designed to audit and validate Astro component strategies within HTML or JSX snippets. It identifies components using `server:defer` or `server:only` directives, ensuring that streaming SSR (Server-Side Rendering) configurations are correctly implemented. By utilizing the `detect_islands` tool, developers can programmatically scan code for island architectures, extracting component names and their associated strategies while flagging any invalid configuration attempts. This prevents common AI agent errors where components are misconfigured, leading to broken hydration or failed streaming.


## Available Tools (1)
- **detect_islands**: Detect Astro islands in an HTML snippet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Astro Server Island Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check this snippet for Astro islands: <div class='container'><MyComponent server:defer /></div>"

**🤖 AI Agent:**
> Found 1 island: MyComponent using the server:defer strategy.

---

**👤 You:**
> "Are there any islands in this code? <header><Nav server:only /></header>"

**🤖 AI Agent:**
> Found 1 island: Nav using the server:only strategy.

---

**👤 You:**
> "Scan this HTML for any invalid Astro strategies: <div server:invalid='true'></div>"

**🤖 AI Agent:**
> No valid islands found, and the has_invalid_strategy flag is true due to the unrecognized directive.


## ❓ FAQ

**Q: What does this MCP server do?**
It scans HTML or JSX snippets to find Astro components using `server:defer` or `server:only` directives, providing a list of detected islands and their strategies.

**Q: How can I use the detection tool?**
You can call the `detect_islands` tool by providing an `html_snippet` containing your Astro component code.

**Q: Does it support both defer and only strategies?**
Yes, the engine is specifically designed to detect both `server:defer` and `server:only` directives within your code snippets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/astro-server-island-detector](https://vinkius.com/ai-agent-connect/astro-server-island-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Astro Server Island Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `astro-server-island-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Astro Server Island Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "astro-server-island-detector": {
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
