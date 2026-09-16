# Water Temperature & Comfort MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/water-temperature-comfort)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Get wetsuit thickness recommendations and hypothermia risk assessments based on water and air conditions.

## Description
This MCP server provides essential thermal safety tools for aquatic activities. It uses a thermal comfort model to calculate the ideal wetsuit thickness and determine if supplemental gear like gloves or booties is necessary. Users can also estimate safe session durations to avoid hypothermia and assess the overall thermal stability of their environment using wind-adjusted air temperatures. Key tools include `get_wetsuit_recommendation` for gear selection, `calculate_hypothermia_risk` for safety timing, and `evaluate_thermal_safety_margin` for environmental assessment.


## Available Tools (4)
- **evaluate_thermal_safety_margin**: Provides a quick assessment of the "buffer" between current conditions and dangerous thermal levels
- **get_gear_tier_info**: Provides descriptive information about the types of gear available in the catalog
- **get_wetsuit_recommendation**: Recommends the ideal wetsuit thickness and supplemental gear for a planned session
- **calculate_hypothermia_risk**: Determines how long a user can safely remain in the water before reaching a critical hypothermia threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Water Temperature & Comfort** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What wetsuit should I wear for 15°C water, 10°C air, and 15 km/h wind?"

**🤖 AI Agent:**
> For those conditions, a 5mm wetsuit is recommended, and you will also need gloves and booties.

---

**👤 You:**
> "Is it safe to stay in 12°C water for 60 minutes with a 3mm wetsuit?"

**🤖 AI Agent:**
> No, staying in 12°C water for 60 minutes with a 3mm wetsuit carries a High risk of hypothermia. The safe duration for that thickness is approximately 35 minutes.

---

**👤 You:**
> "What is the thermal comfort category for 25°C water and 25°C air?"

**🤖 AI Agent:**
> The environment is categorized as Tropical with a high safety margin score.


## ❓ FAQ

**Q: How does wind speed affect my gear recommendation?**
Wind speed increases heat loss through wind chill. The `get_wetsuit_recommendation` tool accounts for this by adjusting the effective air temperature, which may result in a recommendation for thicker wetsuits or extra gear.

**Q: Can I use this to check if my current wetsuit is safe for a long session?**
Yes. You can use `calculate_hypothermia_risk` by providing the water temperature, your current wetsuit thickness, and your planned session duration to see if you stay within safe limits.

**Q: What is a thermal safety margin?**
It is a numerical assessment of the buffer between current environmental conditions and dangerous thermal levels. You can find this using the `evaluate_thermal_safety_margin` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/water-temperature-comfort](https://vinkius.com/en/ai-agent-connect/water-temperature-comfort)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Water Temperature & Comfort** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `water-temperature-comfort` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Water Temperature & Comfort** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "water-temperature-comfort": {
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
