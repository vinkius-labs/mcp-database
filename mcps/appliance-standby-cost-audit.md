# Appliance Standby Cost Audit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/appliance-standby-cost-audit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the energy consumption and financial cost of appliances in standby mode.

## Description
This MCP server provides tools to audit the cumulative energy usage and monetary impact of electrical devices left in standby mode. Use `calculate_device_standby_costs` to get detailed reports for individual appliances, or `get_total_audit_summary` to see the aggregate impact of all devices. You can also use `find_highest_standby_offender` to identify which device is driving your electricity costs.


## Available Tools (4)
- **find_highest_standby_offender**: Identifies which specific device is responsible for the largest portion of energy consumption or cost
- **get_total_audit_summary**: Aggregates the results of all device calculations into a single high-level report
- **validate_audit_parameters**: Checks if the provided input parameters are within realistic or logical bounds before processing
- **calculate_device_standby_costs**: Calculates the specific energy usage and monetary cost for each individual device provided in a list


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Appliance Standby Cost Audit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the standby cost for a TV (20W, 10 hours/day) and a Microwave (5W, 24 hours/day) over 30 days at 0.15 per kWh."

**🤖 AI Agent:**
> The TV costs $0.90 and the Microwave costs $0.54 for the 30-day period.

---

**👤 You:**
> "Which device is the biggest energy consumer: a Gaming Console (60W, 5 hours/day) or a Desktop PC (100W, 2 hours/day) over 7 days?"

**🤖 AI Agent:**
> The Gaming Console is the highest offender with a cost contribution of $0.63.

---

**👤 You:**
> "Give me a summary of the total energy used by these devices: Fridge (10W, 24h), Lamp (5W, 5h), and Router (15W, 24h) over 30 days."

**🤖 AI Agent:**
> The total energy consumption is 15.36 kWh for the 30-day period across 3 devices.


## ❓ FAQ

**Q: How do I calculate the cost for multiple devices?**
You can use `calculate_device_standby_costs` to process a list of devices and get individual results for each.

**Q: Can I find out which device is costing me the most?**
Yes, the `find_highest_standby_offender` tool identifies the specific device responsible for the largest energy or cost contribution.

**Q: What inputs are required for the audit?**
You need to provide the standby watts, daily standby hours for each device, the electricity rate per kWh, and the total number of days for the audit period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/appliance-standby-cost-audit](https://vinkius.com/en/ai-agent-connect/appliance-standby-cost-audit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Appliance Standby Cost Audit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `appliance-standby-cost-audit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Appliance Standby Cost Audit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appliance-standby-cost-audit": {
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
