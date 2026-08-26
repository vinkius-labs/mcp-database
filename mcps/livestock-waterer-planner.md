# Livestock Waterer Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/livestock-waterer-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate waterer space, flow rates, and freezing risks for livestock systems.

## Description
This MCP server provides specialized tools for livestock management and infrastructure planning. It helps producers ensure animal welfare by calculating precise physical access requirements using `get_space_requirements`. It also manages hydraulic planning through `calculate_hydraulic_capacity` to ensure water supply meets peak demand, and evaluates environmental safety with `assess_freezing_risk` to prevent equipment failure in cold climates. For a complete overview, use `get_system_summary` to generate a consolidated report of all requirements.


## Available Tools (4)
- **assess_freezing_risk**: Evaluates if the system design is vulnerable to freezing in cold environments
- **calculate_hydraulic_capacity**: Calculates the necessary flow rate and tank replenishment speed
- **get_space_requirements**: Determines how much physical access space is needed for a specific group of animals
- **get_system_summary**: Provides a consolidated overview of all calculated requirements for a livestock setup


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Livestock Waterer Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much trough space do I need for 50 cattle weighing 500kg each?"

**🤖 AI Agent:**
> For 50 cattle at 500kg each, you require 2500 cm of total linear trough space.

---

**👤 You:**
> "Will my water system freeze if the temperature is -5°C with a flow rate of 10 L/min?"

**🤖 AI Agent:**
> The risk level is high. It is recommended to use insulated troughs or water heaters to prevent freezing.

---

**👤 You:**
> "Calculate the flow rate for a 500L peak demand over 30 minutes."

**🤖 AI Agent:**
> The required flow rate is 16.67 L/min.


## ❓ FAQ

**Q: How does this tool determine space requirements?**
The `get_space_requirements` tool uses species-specific biological standards to calculate either linear trough length or the number of animals per nipple or cup.

**Q: Can I check if my water system will freeze in winter?**
Yes, the `assess_freezing_risk` tool evaluates the risk level based on your expected ambient temperature and the calculated flow rate.

**Q: What information do I need for hydraulic calculations?**
To use `calculate_hydraulic_capacity`, you need the peak water demand in liters, the duration of that peak period, and your total tank volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/livestock-waterer-planner](https://vinkius.com/ai-agent-connect/livestock-waterer-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Livestock Waterer Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `livestock-waterer-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Livestock Waterer Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "livestock-waterer-planner": {
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
