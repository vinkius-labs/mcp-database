# Slope Aspect Effect MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/slope-aspect-effect)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Calculates snow stability and solar/wind exposure based on terrain aspect.

## Description
This MCP server provides specialized tools to analyze how terrain orientation affects snow conditions. It calculates sun exposure hours using `get_sun_exposure`, determines wind-driven snow redistribution with `get_wind_loading_effect`, and assesses overall snowpack risk via `predict_snow_stability`. It also identifies terrain-induced shading through `get_terrain_shadow_status` to provide a complete picture of slope environmental stressors.


## Available Tools (4)
- **get_sun_exposure**: Calculates how many hours a specific slope receives direct sunlight
- **get_terrain_shadow_status**: Determines if a specific slope is currently in the shadow of a neighboring feature
- **get_wind_loading_effect**: Determines how much snow is being redistributed onto the slope by the wind
- **predict_snow_stability**: Provides a prediction of snowpack stability based on environmental stressors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Slope Aspect Effect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much sun exposure will a south-facing slope (180 degrees) at 45 degrees latitude get in winter at noon with 10% cloud cover?"

**🤖 AI Agent:**
> The south-facing slope will receive 6.5 hours of direct sunlight.

---

**👤 You:**
> "Is the snow stable if there are 4 hours of sun, 5 units of wind loading, and the temperature is -2 degrees?"

**🤖 AI Agent:**
> The snow stability is Moderate.

---

**👤 You:**
> "Will a slope facing 270 degrees be leeward if the wind is blowing from 90 degrees at 20 km/h?"

**🤖 AI Agent:**
> Yes, the slope is in a leeward position with a loading intensity of 7.2.


## ❓ FAQ

**Q: How does this tool help with avalanche safety?**
By using `predict_snow_stability`, you can assess how solar radiation and wind loading contribute to snowpack instability, helping to identify high-risk areas.

**Q: Can I check if a slope is in the shade?**
Yes, the `get_terrain_shadow_status` tool determines if a slope is currently obscured by neighboring terrain features.

**Q: What inputs are required for sun exposure?**
To use `get_sun_exposure`, you need the slope aspect, latitude, current season, time of day, cloud cover, and whether terrain shadowing is present.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/slope-aspect-effect](https://vinkius.com/en/ai-agent-connect/slope-aspect-effect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Slope Aspect Effect** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `slope-aspect-effect` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Slope Aspect Effect** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "slope-aspect-effect": {
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
