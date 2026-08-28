# Machinery Capacity Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/machinery-capacity-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate field capacity, completion probability, and machinery economics.

## Description
This MCP server provides essential tools for agricultural planning. Use `calculate_field_productivity` to determine the actual rate of land coverage based on implement width, speed, and efficiency. Use `evaluate_completion_feasibility` to estimate the likelihood of finishing tasks within a timeframe, accounting for weather reliability. The `compare_machinery_economics` tool helps decide between owning equipment or hiring contractors, while `get_operational_window` identifies expected daily working capacity.


## Available Tools (4)
- **calculate_field_productivity**: Calculate the actual rate at which a machine covers land
- **compare_machinery_economics**: Compare the costs of owning a machine versus hiring a contractor
- **evaluate_completion_feasibility**: Estimate if a task can be completed within a specific timeframe given weather risks
- **get_operational_window**: Identify the effective working capacity per day


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Machinery Capacity Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the field capacity for a 5m wide implement moving at 8km/h with 85% efficiency?"

**🤖 AI Agent:**
> The actual field capacity is 3.4 hectares per hour.

---

**👤 You:**
> "Is it feasible to cover 500 hectares in 10 days if I can do 50 hectares per day and weather reliability is 0.7?"

**🤖 AI Agent:**
> The total hours required is 10 hours, and the probability of completion is 0.7.

---

**👤 You:**
> "Should I own a machine or hire one for 1000 hectares if ownership costs $5000 fixed plus $20/ha, and hiring is $35/ha?"

**🤖 AI Agent:**
> Ownership is the preferred option with a total cost of $25,000 compared to $35,000 for custom hire.


## ❓ FAQ

**Q: How does the tool account for weather?**
The `evaluate_completion_feasibility` tool uses a weather reliability factor to adjust the probability of completing work within the available working days.

**Q: Can I compare ownership costs with hiring?**
Yes, the `compare_machinery_economics` tool compares total ownership costs (fixed and variable) against custom hire rates per hectare.

**Q: What is field efficiency?**
Field efficiency is the decimal representing the percentage of time a machine is actively working versus time lost to turns, refueling, or repositioning. It is used in `calculate_field_productivity` to find the actual hectares per hour.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/machinery-capacity-planner](https://vinkius.com/ai-agent-connect/machinery-capacity-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Machinery Capacity Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `machinery-capacity-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Machinery Capacity Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "machinery-capacity-planner": {
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
