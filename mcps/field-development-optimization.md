# Field Development Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/field-development-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimize reservoir development plans, drilling schedules, and facility sizing.

## Description
This MCP server provides advanced tools for optimizing field development plans. It allows AI agents to calculate the most profitable drilling schedules using `get_optimal_drilling_plan`, determine ideal infrastructure scale with `optimize_facility_sizing`, and find the ideal number of wells via `evaluate_well_count`. Additionally, users can assess plan robustness against reservoir variability using `run_uncertainty_simulation`.


## Available Tools (4)
- **evaluate_well_count**: Suggests the optimal number of wells to balance reservoir drainage against capital expenditure
- **get_optimal_drilling_plan**: Determines the most profitable sequence and timing for drilling wells
- **optimize_facility_sizing**: Calculates the ideal size for surface infrastructure to support production
- **run_uncertainty_simulation**: Assesses the robustness of a proposed development plan against reservoir variability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Field Development Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best drilling schedule for a reservoir with high permeability and a well cost of 5 million dollars?"

**🤖 AI Agent:**
> The optimal drilling schedule involves drilling 4 wells in Year 1 and 2 wells in Year 2 to maximize the total NPV of 150 million dollars.

---

**👤 You:**
> "How many wells should I drill for this reservoir profile?"

**🤖 AI Agent:**
> Based on the reservoir characteristics and current economic parameters, the optimal well count is 8 wells.

---

**👤 You:**
> "What is the peak capacity needed for my facility?"

**🤖 AI Agent:**
> To support the planned production, the facility requires a maximum capacity of 50,000 barrels per day.


## ❓ FAQ

**Q: How do I determine the best time to drill wells?**
You can use the `get_optimal_drilling_plan` tool, which analyzes reservoir data and economic parameters to find the most profitable sequence.

**Q: Can I test how reservoir uncertainty affects my NPV?**
Yes, the `run_uncertainty_simulation` tool assesses the robustness of your plan by running multiple scenarios based on defined uncertainty ranges.

**Q: How is facility capacity determined?**
The `optimize_facility_sizing` tool calculates the required scale for surface infrastructure based on reservoir properties and target production rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/field-development-optimization](https://vinkius.com/en/ai-agent-connect/field-development-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Field Development Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `field-development-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Field Development Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "field-development-optimization": {
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
