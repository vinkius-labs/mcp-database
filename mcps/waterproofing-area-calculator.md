# Waterproofing Area Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/waterproofing-area-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate material quantity, consumption, and estimated costs for waterproofing projects across various environments.

## Description
This MCP server provides a specialized calculation engine for estimating waterproofing requirements. It allows users to calculate specific material needs and costs for individual zones using `calculate_zone_needs`, aggregate multiple areas into a comprehensive project overview with `aggregate_project and summary`, and perform financial efficiency analysis between different coating systems via `compare_system_economies`. Ideal for construction professionals managing budgets and material logistics for wet, exposed, or hydrostatic environments.


## Available Tools (3)
- **aggregate_project_summary**: Summarizes multiple zone calculations
- **calculate_zone_needs**: Calculates material quantity and cost for a single area
- **compare_system_economies**: Compares two waterproofing systems


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Waterproofing Area Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the needs for a 50m² bathroom with 2 layers of coating, coverage rate of 0.5L/m², and cost of $10 per m²."

**🤖 AI Agent:**
> For a 50m² area with 2 layers, the total material required is 50L and the estimated cost is $500.

---

**👤 You:**
> "I have two zones: one costs $200 for 20m² and another costs $300 for 30m². What is the total project cost?"

**🤖 AI Agent:**
> The total project area is 50m² and the cumulative cost for all zones is $500.

---

**👤 You:**
> "Compare a system costing $15/m² with one costing $12/m² for a 100m² area."

**🤖 AI Agent:**
> The cost difference is $300, representing a savings of 20% if you switch to the cheaper system.


## ❓ FAQ

**Q: How do I calculate the material needed for a single room?**
Use the `calculate_zone_needs` tool. You will need to provide the environment type, surface area in m², number of layers, coverage rate per m², and the unit price.

**Q: Can I summarize an entire construction project?**
Yes, the `aggregate_project_summary` tool allows you to pass a list of individual zone calculations to get total area, total cost, and average cost per meter for the whole project.

**Q: How can I compare two different waterproofing systems?**
Use the `compare_system_economies` tool by providing the cost per m² for both systems and the total area being compared to see the cost difference and potential savings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/waterproofing-area-calculator](https://vinkius.com/mcp/waterproofing-area-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Waterproofing Area Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `waterproofing-area-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Waterproofing Area Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "waterproofing-area-calculator": {
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
