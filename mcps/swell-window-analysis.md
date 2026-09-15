# Swell Window Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/swell-window-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [geospatial](../categories/geospatial.md)

Geometric analysis of swell windows and coastal shadowing.

## Description
This MCP server provides geometric tools to analyze how ocean swell interacts with specific coastlines. It calculates the available swell window based on bathymetry, identifies blocked directions caused by offshore obstacles like islands or headlands using `analyze_obstruction_shadows`, and determines the most effective wave direction via `identify_optimal_direction`. It is designed for surf forecasting and coastal engineering analysis.


## Available Tools (4)
- **calculate_swell_window**: Determine the range of wave directions that can reach the coastline
- **analyze_obstruction_shadows**: Identify which swell directions are blocked by external physical features
- **get_break_exposure_summary**: Provide a high-level overview of the break's receptivity to different swell patterns
- **identify_optimal_direction**: Find the single best swell direction for maximum energy at the break


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swell Window Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the swell window for a coastline at 90 degrees with this bathymetry: [{"x": 10, "y": 5}]?"

**🤖 AI Agent:**
> The available swell window is between 45 and 135 degrees with a total width of 90 degrees.

---

**👤 You:**
> "Will an island at {x: 50, y: 50} with radius 5 block a swell coming from 180 degrees?"

**🤖 AI Agent:**
> Yes, the island at those coordinates creates a shadow zone that blocks the 180-degree swell direction.

---

**👤 You:**
> "What is the optimal swell direction for a coast at 0 degrees if available angles are [45, 90, 135] and 90 is blocked?"

**🤖 AI Agent:**
> The optimal swell direction is 45 degrees.


## ❓ FAQ

**Q: How do I calculate the available swell directions?**
You can use the `calculate_swell_window` tool by providing the coastline bearing and a JSON string representing the bathymetry profile.

**Q: Can this tool account for islands blocking waves?**
Yes, the `analyze_obstruction_shadows` tool identifies blocked angles and shadow zones created by offshore obstacles.

**Q: What is the best way to find the most energetic swell direction?**
Use the `identify_optimal_direction` tool, which finds the angle closest to perpendicular to the coastline that is not blocked by obstacles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/swell-window-analysis](https://vinkius.com/en/ai-agent-connect/swell-window-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swell Window Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swell-window-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swell Window Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swell-window-analysis": {
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
