# Service Utilization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/service-utilization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Measure resource efficiency by calculating booked versus available hours.

## Description
This MCP server provides tools to monitor and forecast resource efficiency. Use `get_resource_utilization` to check how much capacity a specific resource is using, or `get_team_utilization` to see the combined efficiency of a group. You can also use `get_resource_capacity_forecast` to plan for future workloads and `get_resource_availability_schedule` to view daily breakdowns of availability and bookings.


## Available Tools (4)
- **get_resource_availability_schedule**: Retrieves a breakdown of available versus booked hours per day within a range
- **get_resource_capacity_forecast**: Estimates future availability by comparing existing bookings against theoretical capacity
- **get_resource_utilization**: Calculates the utilization percentage for a specific resource over a defined timeframe
- **get_team_utilization**: Calculates the aggregate utilization for a group of resources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Service Utilization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the utilization for resource 'res-123' from 2024-01-01 to 2024-01-07?"

**🤖 AI Agent:**
> The utilization rate for resource 'res-123' is 85%, with 34 booked hours out of 40 available hours.

---

**👤 You:**
> "Is the team [res-01, res-02] overloaded this week?"

**🤖 AI Agent:**
> The aggregate utilization for the team is 105%, with 84 total booked hours and 80 total available hours, indicating they are currently overloaded.

---

**👤 You:**
> "How much capacity will resource 'res-456' have on 2024-12-25?"

**🤖 AI Agent:**
> On 2024-12-25, resource 'res-456' is expected to have 8 remaining capacity hours with an expected utilization of 20%.


## ❓ FAQ

**Q: How is the utilization rate calculated?**
The utilization rate is the ratio of booked hours to available hours. If booked hours exceed available hours, the rate will exceed 100% and the resource is marked as overloaded.

**Q: Can I check the utilization for an entire team?**
Yes, you can use `get_team_utilization` by providing a list of resource IDs to get the aggregate metrics for the group.

**Q: How do I forecast future capacity?**
Use the `get_resource_capacity_forecast` tool to estimate remaining capacity and expected utilization for a specific future date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/service-utilization](https://vinkius.com/en/ai-agent-connect/service-utilization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Service Utilization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `service-utilization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Service Utilization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "service-utilization": {
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
