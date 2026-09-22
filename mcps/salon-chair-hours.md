# Salon Chair Hours MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/salon-chair-hours)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate salon chair occupancy, utilization, and staffing needs.

## Description
Manage salon capacity and staffing efficiency with precise calculations. This MCP server provides tools to determine total chair occupancy including cleaning buffers, calculate utilization rates, check if appointments fit within a shift, and estimate the number of physical chairs required for a specific workload. Use `calculate_total_occupancy` to account for turnover time, `calculate_utilization_rate` to monitor efficiency, `get_chair_availability_summary` to plan shifts, and `estimate_required_chairs` to prepare for high-volume periods.


## Available Tools (4)
- **calculate_total_occupancy**: Calculate the total time a chair or group of chairs is occupied, including cleaning buffers
- **calculate_utilization_rate**: Calculate the percentage of available salon time used for appointments
- **estimate_required_chairs**: Estimate the minimum number of physical chairs needed to fulfill a volume of work
- **get_chair_availability_summary**: Determine if a set of appointments can fit within a specific shift


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salon Chair Hours** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much total time will 3 appointments of 30, 45, and 60 minutes take if I need a 10 minute cleaning buffer between each?"

**🤖 AI Agent:**
> The total occupied time is 165 minutes (135 minutes of service plus 30 minutes of total buffer time).

---

**👤 You:**
> "I have 400 minutes of total service time and 50 minutes of buffer time per appointment for 5 appointments. How many chairs do I need if each chair is available for 480 minutes?"

**🤖 AI Agent:**
> You will need 2 chairs to fulfill this workload.

---

**👤 You:**
> "Can I fit three 45-minute appointments with a 15-minute buffer into a 2-hour shift?"

**🤖 AI Agent:**
> No, the total time required is 180 minutes, which exceeds the 120-minute shift.


## ❓ FAQ

**Q: How does the tool account for cleaning time?**
The `calculate_total_occupancy` tool allows you to specify a buffer in minutes that is added to each appointment to ensure cleaning time is included in the total occupancy.

**Q: Can I use this to plan my daily staffing?**
Yes, you can use `estimate_required_chairs` to determine how many stations you need to handle your expected volume of clients within your operating hours.

**Q: How is utilization calculated?**
The `calculate_utilization_rate` tool calculates the ratio of total occupied minutes (including buffers) against the total available operating minutes of the salon.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/salon-chair-hours](https://vinkius.com/en/ai-agent-connect/salon-chair-hours)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salon Chair Hours** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salon-chair-hours` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salon Chair Hours** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salon-chair-hours": {
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
