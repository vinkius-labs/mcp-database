# Tailoring Time Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tailoring-time-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and aggregate task durations for garment production workflows.

## Description
This MCP server provides tools to manage and analyze production time in garment tailoring. It allows users to record individual task durations, retrieve a full history of work performed on a specific garment, and calculate total production time. You can use `add_tailoring_task` to log new work, `list_garment_tasks` to see the history, `get_category_summary` to see time spent per production stage, and `get_garment_total_time` to calculate the total duration, including an optional safety buffer.


## Available Tools (4)
- **add_tailoring_task**: Records a new task duration for a specific garment
- **get_category_summary**: Aggregates task durations based on their production stage
- **get_garment_total_time**: Calculates the total time required to complete all tasks for a specific garment
- **list_garment_tasks**: Retrieves a detailed list of all tasks performed on a garment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tailoring Time Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add a task called 'Hemming' for garment G-123 that took 15 minutes in the 'Finishing' category."

**🤖 AI Agent:**
> The task 'Hemming' has been successfully recorded for garment G-123. The new total time for this garment is 15 minutes.

---

**👤 You:**
> "What is the total time spent on garment G-456, including a safety buffer?"

**🤖 AI Agent:**
> The total time for garment G-456, including the applied safety buffer, is 120 minutes across 5 tasks.

---

**👤 You:**
> "Show me all the tasks completed for garment G-789."

**🤖 AI Agent:**
> For garment G-789, the following tasks were recorded: Buttonhole Stitching (10 mins, Finishing), Lapel Shaping (25 mins, Assembly), and Sleeve Attachment (20 mins, Assembly).


## ❓ FAQ

**Q: How do I record a new task for a garment?**
Use the `add_tailoring_task` tool by providing the garment ID, the name of the task, the duration in minutes, and the production category.

**Q: Can I include a safety margin in the total time calculation?**
Yes, when using `get_garment_total_time`, you can set the `includeBuffer` parameter to true to apply a standard safety margin.

**Q: How can I see how much time was spent on each production stage?**
You can use the `get_category_summary` tool to get a breakdown of durations organized by their production category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tailoring-time-total](https://vinkius.com/en/ai-agent-connect/tailoring-time-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tailoring Time Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tailoring-time-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tailoring Time Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tailoring-time-total": {
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
