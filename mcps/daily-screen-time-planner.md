# Daily Screen Time Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/daily-screen-time-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Allocates daily screen time across work, communication, entertainment, and learning blocks.

## Description
Manage your digital wellbeing by distributing your daily screen time limit into structured activity blocks. This MCP allows you to use `calculate_allocation` to divide your time, `get_block_status` to monitor usage health, `validate_daily_plan` to ensure your schedule fits within limits, and `summary_report` to view your overall utilization. It helps maintain a balanced digital lifestyle through precise time management.


## Available Tools (4)
- **get_block_status**: Evaluates if a specific activity block is within its healthy usage range
- **summary_report**: Generates a high-level breakdown of the user's current screen time status
- **validate_daily_plan**: Checks the integrity of a proposed daily plan against total time constraints
- **calculate_allocation**: Determines how the total daily screen time is divided across the four primary activity blocks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Daily Screen Time Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 600 minutes of screen time today. How should I allocate it?"

**🤖 AI Agent:**
> Your 600-minute allocation is: Work: 240 minutes, Communication: 120 minutes, Entertainment: 120 minutes, Learning: 90 minutes, with 30 minutes remaining.

---

**👤 You:**
> "I've used 150 minutes for work. Is that okay?"

**🤖 AI Agent:**
> Your work usage is currently within the optimal range.

---

**👤 You:**
> "Give me a summary of my usage: 200m work, 50m communication, 100m entertainment, 50m learning, with a 500m limit."

**🤖 AI Agent:**
> Total used: 400 minutes. Utilization: 80%. Remaining: 100 minutes.


## ❓ FAQ

**Q: How does the time allocation work?**
The `calculate_allocation` tool divides your total limit into Work (40%), Communication (20%), Entertainment (20%), and Learning (15%), leaving 5% as a flexible allowance.

**Q: Can I check if my current usage is healthy?**
Yes, you can use `get_block_status` to see if your usage in a specific category is optimal, a warning, or excessive.

**Q: How do I know if my planned schedule is valid?**
Use the `validate_daily_plan` tool to check if your proposed minutes for all categories stay within your maximum daily limit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/daily-screen-time-planner](https://vinkius.com/en/ai-agent-connect/daily-screen-time-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Daily Screen Time Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `daily-screen-time-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Daily Screen Time Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "daily-screen-time-planner": {
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
