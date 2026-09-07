# Reef Depth Safety MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/reef-depth-safety)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [maritime](../categories/maritime.md)

Assess reef navigation safety using tide, wave, and depth data.

## Description
This MCP server provides critical tools for maritime safety by analyzing the interaction between lunar tides, charted depths, and wave orbital motion. It allows AI agents to calculate the minimum water depth at wave troughs and determine safe passage windows for vessels. Use `calculate_current_depth` to find total water depth, `calculate_wave_trough_impact` to account for wave energy, and `assess_navigation_safety` to evaluate clearance against vessel draft.


## Available Tools (4)
- **calculate_current_depth**: Determines the total water depth available at the reef location
- **assess_navigation_safety**: Evaluates if a vessel can safely pass over the reef based on its physical requirements
- **calculate_wave_trough_impact**: Calculates how much the wave energy reduces the available water depth due to orbital motion and trough depth
- **determine_safe_passage_window**: Identifies if the current tidal state allows for a safe crossing given the wave conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reef Depth Safety** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it safe for a boat with a 2m draft to cross a reef with 5m charted depth, 1m tide, and 2m waves?"

**🤖 AI Agent:**
> No, the wave trough impact reduces the minimum depth below the required safety margin for a 2m draft.

---

**👤 You:**
> "What is the total water depth if the chart says 10m and the tide is 1.5m?"

**🤖 AI Agent:**
> The total water depth is 11.5 meters.

---

**👤 You:**
> "Can I pass through the reef now with a 3m draft and 0.5m safety buffer?"

**🤖 AI Agent:**
> Yes, the current depth and wave conditions allow for safe passage.


## ❓ FAQ

**Q: How does this tool account for wave motion?**
The `calculate_wave_trough_impact` tool uses wave height and period to calculate how orbital motion reduces the available water depth at the trough.

**Q: Can I use this to plan a crossing?**
Yes, the `determine_safe_passage_window` tool identifies if current tidal states allow for safe crossing and provides an estimated time window.

**Q: What is the difference between charted depth and total water depth?**
Charted depth is the static seabed measurement, while total water depth is the sum of charted depth and the current tide height, calculated via `calculate_current_depth`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/reef-depth-safety](https://vinkius.com/ai-agent-connect/reef-depth-safety)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reef Depth Safety** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reef-depth-safety` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reef Depth Safety** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reef-depth-safety": {
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
