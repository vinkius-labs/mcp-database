# Constellation Locator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/constellation-locator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate real-time constellation visibility, transit times, and celestial profiles.

## Description
Connect your AI agent to the celestial sphere. This MCP server provides precise astronomical calculations for observers on Earth. Use `get_visible_constellations` to see what is currently above your horizon, `get_constellation_transit_details` to find when a star pattern reaches its highest point, or `get_constellation_profile` to learn about specific IAU constellations. It calculates local sidereal time, altitude, and azimuth to provide accurate stargazing data.


## Available Tools (3)
- **get_constellation_profile**: Retrieves the fundamental characteristics and visibility classifications of a specific constellation
- **get_constellation_transit_details**: Finds the specific time when a requested constellation will reach its highest point (transit) in the sky
- **get_visible_constellations**: Identifies which constellations are currently above the horizon for a specific observer at a specific time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Constellation Locator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What constellations are visible from London right now?"

**🤖 AI Agent:**
> Currently, Orion, Taurus, and Ursa Major are visible above the horizon in London.

---

**👤 You:**
> "When will Cassiopeia reach its highest point tonight in New York?"

**🤖 AI Agent:**
> Cassiopeia will reach its transit point at 02:15 AM local time with a maximum altitude of 72°.

---

**👤 You:**
> "Tell me about the constellation Lyra."

**🤖 AI Agent:**
> Lyra is a small constellation in the northern sky, known for the bright star Vega. It is a seasonal constellation best viewed during summer months.


## ❓ FAQ

**Q: How accurate are the visibility calculations?**
Calculations are based on the observer's precise latitude and longitude, using local sidereal time to determine the exact position of constellations relative to the horizon.

**Q: Can I find out when a specific constellation will be highest in the sky?**
Yes, you can use the `get_constellation_transit_details` tool to find the exact transit time and maximum altitude for any IAU constellation.

**Q: Does this support both Northern and Southern Hemisphere observers?**
Yes, the tools account for your specific latitude, correctly identifying circumpolar constellations and seasonal visibility for both hemispheres.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/constellation-locator](https://vinkius.com/ai-agent-connect/constellation-locator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Constellation Locator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `constellation-locator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Constellation Locator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "constellation-locator": {
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
