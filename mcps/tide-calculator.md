# Tide Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tide-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Predict tide levels, currents, and lunar phase modifiers.

## Description
This MCP server provides deterministic tide predictions using lunar correlation and sinusoidal approximation. It allows AI agents to calculate predicted high and low tide times and heights, determine tidal current direction and speed (flood or ebb), and retrieve lunar phase modifiers to adjust tidal amplitude. Use `predict_tide_levels` to get a full schedule of tides, `predict_tidal_currents` to check water movement at a specific time, or `get_lunar_phase_modifier` to understand how the moon phase affects tidal range.


## Available Tools (3)
- **get_lunar_phase_modifier**: Retrieves the multiplier used to scale tidal amplitude based on the moon phase for a given date
- **predict_tidal_currents**: Determines the direction and speed of water movement based on the tide state
- **predict_tide_levels**: Calculates the predicted times and heights for high and low tides for a specific date and location type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tide Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the predicted tide levels for 2024-05-20 with a semidiurnal pattern and a reference high tide at 08:00 with a height of 2.5m?"

**🤖 AI Agent:**
> On 2024-05-20, the predicted tides are: High at 08:00 (2.5m), Low at 14:12 (1.2m), High at 20:25 (2.4m), and Low at 02:37 (1.1m). The tidal range is 1.4m.

---

**👤 You:**
> "Is the tide coming in or going out at 10:00 on 2024-05-20?"

**🤖 AI Agent:**
> At 10:00, the tide is ebb, moving away from the shore at a speed of 0.45 m/s.

---

**👤 You:**
> "What is the lunar phase modifier for 2024-05-20?"

**🤖 AI Agent:**
> On 2024-05-20, the phase is Full Moon, with an amplitude multiplier of 1.1.


## ❓ FAQ

**Q: How accurate are these tide predictions?**
Predictions use a sinusoidal approximation with a 12h 25m period and adjust for spring/neap cycles based on lunar phases.

**Q: What tidal patterns are supported?**
The server supports semidiurnal, diurnal, and mixed tidal patterns.

**Q: Can I find out if the current is flood or ebb?**
Yes, by using `predict_tidal_currents`, you can determine if the water is moving toward the shore (flood) or away from it (ebb).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tide-calculator](https://vinkius.com/ai-agent-connect/tide-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tide Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tide-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tide Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tide-calculator": {
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
