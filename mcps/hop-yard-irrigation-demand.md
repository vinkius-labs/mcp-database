# Hop Yard Irrigation Demand MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hop-yard-irrigation-demand)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise water requirements for hop production based on growth stages and variety.

## Description
This MCP server provides specialized irrigation management tools for hop growers. It connects AI agents to precise water demand calculations by accounting for crop coefficients ($K_c$), growth stages, and variety types. Use `calculate_daily_demand` to determine daily water needs, `generate_irrigation_schedule` to plan irrigation events based on soil moisture, and `calculate_seasonal_total` to estimate seasonal water requirements. The system specifically addresses the high sensitivity of hop cones to water stress during the `CONE_DEVELOPMENT` stage.


## Available Tools (3)
- **calculate_daily_demand**: Calculate daily water demand
- **calculate_seasonal_total**: Calculate seasonal water total
- **generate_irrigation_schedule**: Generate irrigation schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hop Yard Irrigation Demand** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much water do I need for 5 hectares of Alpha hops today if the ET is 5.2 and we are in the training stage with 85% efficiency?"

**🤖 AI Agent:**
> The daily water requirement for your 5 hectares is 30.59 units, with an irrigation depth of 6.12 mm.

---

**👤 You:**
> "Generate an irrigation schedule for soil with 50mm capacity and 30mm current moisture, given a daily demand of 5mm."

**🤖 AI Agent:**
> The next irrigation should occur on 2024-06-15 with a recommended volume of 12.5mm. You have 4 days until the next irrigation is required.

---

**👤 You:**
> "What is the estimated seasonal water total for 10 acres of Aroma hops with a forecast of [4, 5, 6, 5, 4] ET values and 90% efficiency?"

**🤖 AI Agent:**
> The total seasonal volume required is 245.5 units, with an average daily demand of 49.1 units.


## ❓ FAQ

**Q: How does the tool handle different hop varieties?**
The system uses specific crop coefficients for both 'ALPHA' and 'AROMA' varieties to ensure accurate water demand calculations.

**Q: Can I plan my irrigation schedule in advance?**
Yes, you can use `generate_irrigation_schedule` to create a planned sequence of irrigation events based on your current soil moisture and daily demand.

**Q: Does this account for water stress during cone development?**
Yes, by enabling stress sensitivity in the irrigation schedule, the system prioritizes higher moisture levels during the `CONE_DEVELOPMENT` stage to protect cone quality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hop-yard-irrigation-demand](https://vinkius.com/ai-agent-connect/hop-yard-irrigation-demand)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hop Yard Irrigation Demand** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hop-yard-irrigation-demand` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hop Yard Irrigation Demand** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hop-yard-irrigation-demand": {
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
