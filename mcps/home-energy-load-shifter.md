# Home Energy Load Shifter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/home-energy-load-shifter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [smart-home](../categories/smart-home.md)

Schedules appliance usage into preferred electricity tariff windows.

## Description
This MCP server provides tools to optimize home energy consumption by shifting appliance loads into preferred tariff windows. It ensures that all scheduled tasks respect individual deadlines and stay within the home's maximum concurrent power capacity. Use `get_tariff_windows` to find available time slots, `calculate_optimal_schedule` to generate a complete plan, and `get_load_utilization_report` to visualize power usage over time.


## Available Tools (4)
- **calculate_optimal_schedule**: Generates a valid schedule that places appliance loads into tariff windows
- **get_load_utilization_report**: Analyzes a generated schedule to show how much of the power capacity is being used over time
- **get_tariff_windows**: Retrieves the available time intervals for electricity usage
- **validate_load_feasibility**: Checks if a single appliance can theoretically fit into the available windows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home Energy Load Shifter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my available electricity tariff windows?"

**🤖 AI Agent:**
> Your available tariff windows are from 02:00 to 06:00 and 13:00 to 17:00.

---

**👤 You:**
> "Can I run my dishwasher (2kW, 120 mins) before 10:00 AM?"

**🤖 AI Agent:**
> Yes, the dishwasher can be scheduled to run from 02:00 to 04:00 within the available tariff window.

---

**👤 You:**
> "Create a schedule for a 3kW washing machine (60 mins) and a 1kW dryer (90 mins) with a 5kW limit."

**🤖 AI Agent:**
> The washing machine is scheduled for 02:00-03:00 and the dryer is scheduled for 03:00-04:30.


## ❓ FAQ

**Q: How does the scheduling work?**
The engine uses `calculate_optimal_schedule` to fit appliance loads into windows where electricity is cheapest or most available, while ensuring the total power draw never exceeds your `maxConcurrentLoadKw` limit.

**Q: Can I check if a specific appliance can be scheduled?**
Yes, you can use the `validate_load_feasibility` tool to check if a single appliance can fit into the available tariff windows before attempting to schedule a full plan.

**Q: How do I see my power usage profile?**
Once a schedule is generated, you can use `get_load_utilization_report` to see a breakdown of total power usage and remaining capacity at different timestamps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/home-energy-load-shifter](https://vinkius.com/en/ai-agent-connect/home-energy-load-shifter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home Energy Load Shifter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `home-energy-load-shifter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home Energy Load Shifter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-energy-load-shifter": {
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
