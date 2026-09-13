# SAGD Process Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sagd-process-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Model Steam Assisted Gravity Drainage processes using Butler's analytical models.

## Description
This MCP server provides specialized engineering tools for modeling Steam Assisted Gravity Drainage (SAGD) processes. It uses Butler's analytical framework to calculate critical recovery metrics. Use `get_production_forecast` to predict oil recovery rates and steam-oil ratios. Use `optimize_well_geometry` to determine the ideal vertical spacing between injector and producer wells. The server also includes `analyze_heterogeneity_impact` to assess how reservoir variations affect steam chamber growth and `calculate_steam_requirements` to estimate daily steam demand and energy needs.


## Available Tools (4)
- **analyze_heterogeneity_impact**: Evaluates how variations in rock properties will affect the steam chamber
- **calculate_steam_requirements**: Determines the amount of steam needed to sustain the process for a specific period
- **get_production_forecast**: Predicts the expected oil recovery rate based on current reservoir and well parameters
- **optimize_well_geometry**: Recommends the ideal vertical distance between wells to maximize efficiency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SAGD Process Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected oil production rate for a reservoir with 2.0 Darcy permeability, 500 cP viscosity, 30m thickness, and 5m well spacing?"

**🤖 AI Agent:**
> The predicted production rate is 450 barrels per day with an estimated SOR of 2.8 and a chamber rise rate of 0.15 m/day.

---

**👤 You:**
> "Recommend the best vertical spacing for a reservoir with 1.5 Darcy permeability, 800 cP viscosity, and a target SOR of 3.0."

**🤖 AI Agent:**
> The optimal vertical spacing is 6.5 meters, providing an expected efficiency rating of 0.85.

---

**👤 You:**
> "How much steam will I need daily for a 40m thick reservoir with 2.5 Darcy permeability to produce 500 barrels of oil per day at 400 cP viscosity?"

**🤖 AI Agent:**
> The daily steam demand is 1,400 barrels per day, with a total energy requirement of 12.5 million BTU and an estimated process duration of 1,200 days.


## ❓ FAQ

**Q: What models are used for production forecasting?**
The server utilizes Butler's analytical models to predict oil production rates and steam-oil ratios.

**Q: Can I optimize my well placement?**
Yes, you can use the `optimize_well_geometry` tool to find the recommended vertical distance between wells to maximize efficiency.

**Q: How does reservoir heterogeneity affect my design?**
You can use `analyze_heterogeneity_impact` to evaluate how variations in rock properties might delay steam chamber growth or reduce recovery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sagd-process-design](https://vinkius.com/en/ai-agent-connect/sagd-process-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SAGD Process Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sagd-process-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SAGD Process Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sagd-process-design": {
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
