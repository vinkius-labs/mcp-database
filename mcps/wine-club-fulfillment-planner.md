# Wine Club Fulfillment Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-club-fulfillment-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Plans wine club shipment logistics, labor requirements, and seasonal staffing needs.

## Description
This MCP server provides essential logistics and capacity planning tools for wine club operations. It allows AI agents to calculate daily throughput using `get_daily_capacity`, estimate total man-hours with `calculate_labor_requirements`, and build operational timelines via `generate_shipping_schedule`. Additionally, it helps manage seasonal surges with `forecast_peak_staffing` and ensures fair stock distribution across membership levels using `get_tier_allocation_plan`.


## Available Tools (5)
- **calculate_labor_requirements**: Calculates the total labor hours needed to fulfill a specific shipment volume
- **forecast_peak_staffing**: Identifies the gap between current capacity and shipment demand to determine seasonal hiring needs
- **generate_shipping_schedule**: Creates a timeline of when shipments must be processed to meet delivery deadlines
- **get_daily_capacity**: Determines the maximum number of orders the facility can process in a single day
- **get_tier_allocation_plan**: Manages how stock is distributed across different membership tiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Club Fulfillment Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many orders can my team of 5 process in an 8-hour shift if they handle 10 bottles per hour?"

**🤖 AI Agent:**
> Your team can process 400 orders per day.

---

**👤 You:**
> "I have 5000 bottles to ship and my staff processes 50 bottles per hour. How many labor hours do I need?"

**🤖 AI Agent:**
> You will need 100 total labor hours to complete the shipment.

---

**👤 You:**
> "We have 1000 members and each gets 6 bottles. If our daily capacity is 100 orders, how many days will it take to finish?"

**🤖 AI Agent:**
> It will take 10 operational days to complete the shipment.


## ❓ FAQ

**Q: How can I calculate how many extra workers I need for the holiday rush?**
You can use the `forecast_peak_staffing` tool to identify the gap between your current capacity and the required capacity to meet your shipment deadline.

**Q: Can this tool help with member tier prioritization?**
Yes, the `get_tier_allocation_plan` tool manages stock distribution by applying priority weights to different membership tiers.

**Q: How do I determine the total labor hours for a shipment?**
Use the `calculate_labor_requirements` tool by providing the total number of bottles and the processing rate per staff member.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-club-fulfillment-planner](https://vinkius.com/ai-agent-connect/wine-club-fulfillment-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Club Fulfillment Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-club-fulfillment-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Club Fulfillment Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-club-fulfillment-planner": {
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
