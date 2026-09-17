# Cellar Space Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cellar-space-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimize cellar space through tank allocation, barrel stacking, and seasonal capacity forecasting.

## Description
This MCP server provides tools to optimize cellar space utilization. It helps manage wine production by calculating efficient tank allocation for batches, determining optimal barrel stacking configurations that respect ceiling heights and forklift access, and forecasting seasonal capacity to prevent bottlenecks. Use `get_tank_allocation` to distribute wine batches, `get_barrel_configuration` for stacking density, `forecast_seasonal_capacity` to predict shortages, and `analyze_workflow_efficiency` to ensure forklift paths remain clear.


## Available Tools (4)
- **analyze_workflow_efficiency**: Evaluates if the current or proposed layout allows for sufficient movement and access
- **forecast_seasonal_capacity**: Predicts space availability and identifies potential shortages throughout the production year
- **get_barrel_configuration**: Calculates the optimal stacking arrangement for barrels to maximize density
- **get_tank_allocation**: Determines how to distribute wine batches into available tanks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cellar Space Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How should I distribute these wine batches into my available tanks?"

**🤖 AI Agent:**
> Batch A (500L) should be allocated to Tank 1, and Batch B (300L) should be allocated to Tank 2.

---

**👤 You:**
> "What is the best way to stack my barrels in the current cellar?"

**🤖 AI Agent:**
> The optimal configuration consists of 5 stacks, each 3 barrels high, with 1.5m aisles between them.

---

**👤 You:**
> "Will I have enough space for the harvest peak in October?"

**🤖 AI Agent:**
> No, the forecast indicates a capacity bottleneck in October due to high tank volume requirements.


## ❓ FAQ

**Q: How does the tool handle forklift access?**
The `analyze_workflow_efficiency` tool evaluates if the layout allows for sufficient movement by checking if assets are blocked based on required aisle widths.

**Q: Can I predict when I will run out of tank space?**
Yes, you can use `forecast_seasonal_capacity` to identify potential bottlenecks and predict space availability throughout the production year.

**Q: How is barrel stacking calculated?**
The `get_barrel_configuration` tool calculates stacking arrangements by considering cellar dimensions, barrel sizes, and the minimum width required for forklift access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cellar-space-optimization](https://vinkius.com/en/ai-agent-connect/cellar-space-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cellar Space Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cellar-space-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cellar Space Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cellar-space-optimization": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
