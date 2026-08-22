# Tide Curve Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tide-curve-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Deterministic sinusoidal tide prediction and surf window calculator.

## Description
This MCP server provides precise tidal modeling using a deterministic sinusoidal curve. It allows AI agents to calculate water levels, identify tidal states like rising or falling, and determine optimal surfing windows based on specific beach profiles. Use `predict_tide_height` to find the exact water level at any timestamp, `get_tide_lifecycle` for a summary of the tidal range and duration, or `find_surf_windows` to locate the best times to hit the waves.


## Available Tools (3)
- **find_surf_windows**: Identifies the time intervals most suitable for surfing based on the tidal cycle
- **get_tide_lifecycle**: Provides a summary of the characteristics of the current tidal cycle
- **predict_tide_height**: Calculates the predicted water level and tidal status at a specific moment in time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tide Curve Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will the tide height be at timestamp 1715683200?"

**🤖 AI Agent:**
> The predicted height is 1.45 meters and the tide is currently falling.

---

**👤 You:**
> "When is the next optimal surf window for a steep beach profile?"

**🤖 AI Agent:**
> The optimal surf window is between 1715680000 and 1715683600.

---

**👤 You:**
> "Give me a summary of the current tidal cycle."

**🤖 AI Agent:**
> The tidal range is 2.5 meters with a duration of 6.2 hours.


## ❓ FAQ

**Q: How accurate are the tide predictions?**
The predictions use a deterministic sinusoidal model based on the provided high and low tide extremes to calculate height and state.

**Q: Can I find the best time to surf?**
Yes, you can use the `find_surf_windows` tool to identify the best time intervals based on the beach profile.

**Q: What tidal states are supported?**
The system identifies rising, falling, and slack water states.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tide-curve-predictor](https://vinkius.com/ai-agent-connect/tide-curve-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tide Curve Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tide-curve-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tide Curve Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tide-curve-predictor": {
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
