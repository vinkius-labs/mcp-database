# Work Hours Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/work-hours-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Aggregates work durations and calculates labor costs and overtime.

## Description
This MCP server provides precise tools for managing work time. It allows AI agents to sum multiple work durations using `calculate_total_duration`, determine financial expenditure with `calculate_labor_cost`, and analyze work breakdowns via `analyze_overtime`. For a complete report including total time, cost, and overtime status, use `summarize_work_period`.


## Available Tools (4)
- **calculate_labor_cost**: Determines the total cost of work based on a provided rate and duration
- **calculate_total_duration**: Calculates the cumulative sum of multiple provided work durations
- **summarize_work_period**: Provides a comprehensive overview of a work period including total time, cost, and overtime status
- **analyze_overtime**: Splits a total duration into standard hours and overtime hours based on a specific limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Work Hours Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Sum these durations: 2 hours 30 minutes, 1 hour 45 minutes, and 4 hours."

**🤖 AI Agent:**
> The total duration is 8 hours and 15 minutes.

---

**👤 You:**
> "What is the cost for 40 hours and 30 minutes of work at a rate of 50 per hour?"

**🤖 AI Agent:**
> The total cost is 2025.

---

**👤 You:**
> "I worked 45 hours total. If my threshold is 40 hours, how much is overtime?"

**🤖 AI Agent:**
> You have 40 standard hours and 5 overtime hours.


## ❓ FAQ

**Q: How can I sum multiple work entries?**
You can use the `calculate_total_duration` tool by providing an array of duration objects containing hours and minutes.

**Q: Can I calculate overtime automatically?**
Yes, the `analyze_overtime` tool splits your total duration into standard and overtime hours based on a threshold you define.

**Q: How do I get a full report of my work period?**
The `summarize_work_period` tool provides a unified report including total time, total cost, and overtime breakdown.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/work-hours-total](https://vinkius.com/en/ai-agent-connect/work-hours-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Work Hours Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `work-hours-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Work Hours Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "work-hours-total": {
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
