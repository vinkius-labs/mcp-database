# Consulting Utilization Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/consulting-utilization-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate billable utilization, revenue targets, and capacity plans for professional services.

## Description
This MCP server provides essential tools for professional services firms to manage consultant productivity. Use `get_consultant_utilization` to track how much time is spent on billable work, `calculate_revenue_targets` to determine necessary revenue based on overhead and rates, `get_capacity_plan` to account for holidays and working days, and `validate_utilization_health` to compare actual performance against firm benchmarks.


## Available Tools (4)
- **calculate_revenue_targets**: Determines the minimum revenue required from a consultant to meet firm targets
- **get_capacity_plan**: Provides a breakdown of available working time after accounting for holidays
- **get_consultant_utilization**: Calculates the billable utilization percentage for a specific consultant over a given period
- **validate_utilization_health**: Evaluates if a consultant's current utilization is meeting or exceeding firm standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Consulting Utilization Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the utilization for consultant C123 from 2024-01-01 to 2024-01-31?"

**🤖 AI Agent:**
> Consultant C123 had a utilization of 78% for January 2024, with 156 billable hours out of 200 available hours.

---

**👤 You:**
> "Calculate the revenue target for consultant C456 with a 75% target, $200 hourly rate, and 1.5 overhead multiplier for Q1 2024."

**🤖 AI Agent:**
> The target revenue for consultant C456 for Q1 2024 is $67,500, based on an expected 168.75 billable hours.

---

**👤 You:**
> "Is a consultant with 65% utilization healthy if the target is 70%?"

**🤖 AI Agent:**
> No, the consultant is not meeting the target. There is a negative variance of 5% from the benchmark.


## ❓ FAQ

**Q: How is billable utilization calculated?**
Utilization is the ratio of billable hours to the total available capacity, where available capacity is the number of working days (excluding holidays) multiplied by standard daily hours.

**Q: Can I plan for upcoming holidays?**
Yes, the `get_capacity_plan` tool automatically accounts for recognized holidays to provide an accurate count of working days and available hours.

**Q: How do I set revenue targets?**
Use `calculate_revenue_targets` by providing the consultant ID, desired utilization, hourly rate, and the overhead multiplier to find the minimum required revenue.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/consulting-utilization-plan](https://vinkius.com/en/ai-agent-connect/consulting-utilization-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Consulting Utilization Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `consulting-utilization-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Consulting Utilization Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "consulting-utilization-plan": {
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
