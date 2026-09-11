# Reservoir Saturation Height Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/reservoir-saturation-height-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates water saturation profiles and transition zone thickness using capillary pressure data.

## Description
This MCP server provides specialized tools for reservoir engineering to model fluid distribution. It connects AI agents to physical reservoir properties, allowing for the calculation of water saturation at specific elevations, determining the thickness of the transition zone, and generating continuous saturation profiles. Use `get_saturation_at_height` for single points, `get_transition_zone_depth` to find the saturation change interval, `get_saturation_profile` for vertical profiles, and `get_hydrocarbon_distribution` to calculate hydrocarbon volumes based on pore volume and saturation.


## Available Tools (4)
- **get_saturation_at_height**: Determines the specific water saturation at a single defined elevation
- **get_saturation_profile**: Generates a continuous list of saturation values across multiple elevations
- **get_transition_zone_depth**: Identifies the thickness of the zone where fluid saturation is actively changing
- **get_hydrocarbon_distribution**: Calculates the vertical distribution of oil or gas volume based on saturation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reservoir Saturation Height Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the water saturation at 5 meters above the FWL given a density difference of 0.05 and this capillary pressure data: {"0": 0.1, "0.5": 0.3, "1.0": 0.5}?"

**🤖 AI Agent:**
> The water saturation at 5 meters above the FWL is 0.5.

---

**👤 You:**
> "Calculate the hydrocarbon volume at 10 meters if the pore volume per unit height is 0.2, density difference is 0.06, and saturation data is {"0.6": 0.2, "1.2": 0.4}?"

**🤖 AI Agent:**
> The hydrocarbon volume at 10 meters is 0.12.

---

**👤 You:**
> "Find the thickness of the transition zone for a reservoir with irreducible water saturation of 0.2, density difference of 0.04, and data {"0.1": 0.8, "0.4": 0.2}?"

**🤖 AI Agent:**
> The transition zone thickness is 0.4 meters.


## ❓ FAQ

**Q: What is the purpose of this MCP?**
It calculates water saturation profiles and hydrocarbon distributions relative to the Free Water Level (FWL) using capillary pressure data.

**Q: How do I calculate the transition zone thickness?**
You can use the `get_transition_zone_depth` tool by providing the capillary pressure data, density difference, and the irreducible water saturation value.

**Q: Can I generate a full vertical profile?**
Yes, the `get_saturation_profile` tool allows you to pass an array of heights to generate a continuous list of saturation values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/reservoir-saturation-height-calculator](https://vinkius.com/ai-agent-connect/reservoir-saturation-height-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reservoir Saturation Height Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reservoir-saturation-height-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reservoir Saturation Height Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reservoir-saturation-height-calculator": {
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
