# Soccer Formation Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/soccer-formation-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate team geometry, player spacing, and tactical coverage.

## Description
This MCP server provides deterministic tactical analysis for soccer formations. It allows AI agents to calculate team width, depth, and line spacing using `get_formation_geometry`. It also determines field control via `get_coverage_metrics` and identifies passing corridors or high-pressure zones with `analyze_tactical_lanes`.


## Available Tools (3)
- **analyze_tactical_lanes**: Identifies available passing corridors and potential high-pressure zones
- **get_coverage_metrics**: Determines how much of the field is effectively controlled by the players movement radii
- **get_formation_geometry**: Calculates the physical footprint and structural spacing of a team on the pitch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Soccer Formation Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the team width and depth for a 4-4-2 formation with these player positions: [{"role":"DF","x":0.2,"y":0.2}, {"role":"DF","x":0.8,"y":0.2}, {"role":"MF","x":0.5,"y":0.5}, {"role":"FW","x":0.5,"y":0.8}] on a 105x68m field."

**🤖 AI Agent:**
> The team width is 40.8 meters and the team depth is 39.6 meters.

---

**👤 You:**
> "How much of the field is covered by these players with a 12m radius on a 100x64m pitch?"

**🤖 AI Agent:**
> The total field coverage is 24.5%.

---

**👤 You:**
> "Check for passing lanes and pressing triggers for this setup."

**🤖 AI Agent:**
> The passing lane from MF to FW is clear, and a pressing trigger is detected at coordinates (0.5, 0.6) due to high player density.


## ❓ FAQ

**Q: What kind of data does this tool analyze?**
It analyzes player coordinates, field dimensions, and movement radii to provide spacing and coverage metrics.

**Q: Can I calculate passing lanes?**
Yes, the `analyze_tactical_lanes` tool identifies available passing corridors and potential pressing triggers.

**Q: What field dimensions are supported?**
The tool supports standard pitch dimensions, typically between 100-110m in length and 64-75m in width.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/soccer-formation-analyzer](https://vinkius.com/ai-agent-connect/soccer-formation-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Soccer Formation Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soccer-formation-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Soccer Formation Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soccer-formation-analyzer": {
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
