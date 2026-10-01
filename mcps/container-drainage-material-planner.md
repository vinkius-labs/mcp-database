# Container Drainage Material Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/container-drainage-material-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate drainage media and liner quantities for planting projects.

## Description
This MCP server provides precision tools for planning containerized planting projects. It calculates the exact volume of drainage media needed using `calculate_drainage_volume`, determines the required liner surface area with `calculate_liner_surface_area`, and provides cost estimates via `estimate_material_costs`. You can also use `generate_project_summary` to consolidate all data into a single procurement report.


## Available Tools (4)
- **calculate_drainage_volume**: Determines the total volume of drainage media needed for the entire project
- **calculate_liner_surface_area**: Determines the total surface area of liner material required to line all containers
- **estimate_material_costs**: Provides a high-level cost estimate for the drainage media based on the required number of bags
- **generate_project_summary**: Aggregates all calculated material and surface area data into a single consolidated report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Container Drainage Material Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much drainage media do I need for 50 pots with a 10cm diameter and 5cm drainage depth, assuming a 10% waste rate?"

**🤖 AI Agent:**
> You will need 1 bag of drainage media for this project.

---

**👤 You:**
> "Calculate the liner area for 100 pots that are 20cm in diameter and 30cm tall."

**🤖 AI Agent:**
> The total liner area required is 2.19 square meters.

---

**👤 You:**
> "What is the cost for 5 bags of media if each bag costs $15.00?"

**🤖 AI Agent:**
> The total cost including tax is $81.00.


## ❓ FAQ

**Q: How do I calculate the total media needed?**
Use the `calculate_drainage_volume` tool by providing the pot diameter, drainage layer depth, total pot count, and your preferred waste rate.

**Q: Can I get a full procurement report?**
Yes, once you have the outputs from the volume, area, and cost tools, use `generate_project_summary` to create a consolidated report.

**Q: Does this account for waste during installation?**
Yes, the `calculate_drainage_volume` tool includes a waste rate parameter to account for settling and spills.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/container-drainage-material-planner](https://vinkius.com/en/ai-agent-connect/container-drainage-material-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Container Drainage Material Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `container-drainage-material-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Container Drainage Material Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "container-drainage-material-planner": {
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
