# break-time-total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/break-time-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A precision utility for calculating and managing cumulative break durations.

## Description
This MCP server provides essential tools for workforce management and labor compliance by aggregating break periods. Use `calculate_total_break_time` to sum durations, `validate_break_compliance` to check against regulatory limits, `get_break_summary` for statistical overviews, and `filter_breaks_by_threshold` to identify long breaks.


## Available Tools (4)
- **calculate_total_break_time**: Calculates the sum of a provided list of break durations
- **filter_breaks_by_threshold**: Identifies specific break periods that exceed a certain length
- **get_break_summary**: Provides a statistical overview of a set of breaks
- **validate_break_compliance**: Checks if the total break time adheres to a specific regulatory limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **break-time-total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total time for breaks of 10, 15, and 25 minutes?"

**🤖 AI Agent:**
> The total duration is 50 minutes (00:50).

---

**👤 You:**
> "Are my breaks compliant if I took 60 minutes of breaks and the limit is 45?"

**🤖 AI Agent:**
> No, you have exceeded the limit by 15 minutes.

---

**👤 You:**
> "Find any breaks longer than 20 minutes in this list: 5, 25, 10, 30."

**🤖 AI Agent:**
> The breaks exceeding the threshold are 25 and 30 minutes.


## ❓ FAQ

**Q: How do I calculate the total time spent on breaks?**
You can use the `calculate_total_break_time` tool by providing a list of break durations in minutes.

**Q: Can I check if my breaks comply with labor laws?**
Yes, the `validate_break_compliance` tool allows you to check if your total break time is within a specific maximum limit.

**Q: How can I see a summary of all breaks taken?**
The `get_break_summary` tool provides a full statistical overview, including the count, total time, average duration, and the longest break.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/break-time-total](https://vinkius.com/en/ai-agent-connect/break-time-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **break-time-total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `break-time-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **break-time-total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "break-time-total": {
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
