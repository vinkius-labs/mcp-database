# Evening Routine Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/evening-routine-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Constructs structured evening wind-down sequences by working backwards from your target sleep time.

## Description
This MCP server acts as a specialized scheduling engine to help you prepare for sleep. By providing your target sleep time, a list of tasks, and a mandatory screen-free buffer, the `generate_routine` tool calculates a precise chronological sequence of activities. It also includes tools like `validate_task_feasibility` to ensure your planned activities fit within your available time and `get_constraint_conflicts` to check if your schedule respects household rules like quiet hours.


## Available Tools (4)
- **generate_routine**: Calculates the optimal chronological sequence of activities and their start/end times
- **get_constraint_conflicts**: Identifies if any proposed tasks or the screen-off buffer violate specific household rules
- **validate_task_feasibility**: Checks if a specific set of tasks can physically fit into a window of time while respecting the screen-off buffer
- **calculate_buffer_start**: Determines the exact time the user must put away all screens


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Evening Routine Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan my evening. I want to sleep at 22:30. I need to do reading (20 mins), stretching (15 mins), and cleaning the kitchen (20 mins). My screen-off buffer is 30 minutes."

**🤖 AI Agent:**
> Your evening routine is set. You will start reading at 21:05, finish stretching at 21:40, and finish cleaning the kitchen at 22:00. Your screen-off period begins at 22:00, leading directly to your 22:30 sleep time.

---

**👤 You:**
> "Can I fit a 45-minute bath and 30 minutes of meditation into my routine if I start at 20:00 and want to sleep at 21:00, with a 15-minute screen-off buffer?"

**🤖 AI Agent:**
> No, those tasks will not fit. You are over-scheduled by 10 minutes.

---

**👤 You:**
> "When should I turn off my phone if I want to be asleep by 23:00 and I want a 45-minute buffer?"

**🤖 AI Agent:**
> You should turn off your screens at 22:15.


## ❓ FAQ

**Q: How does the routine calculation work?**
The engine uses backwards scheduling. It starts from your target sleep time, subtracts the mandatory screen-off buffer, and then fits your tasks into the remaining time while respecting any household constraints.

**Q: Can I add specific household rules?**
Yes, you can provide constraints such as quiet hours. The `get_constraint_conflicts` tool will then check if your proposed activities violate those rules.

**Q: What happens if my tasks are too long for my schedule?**
If your tasks exceed the available time, the `validate_task_feasibility` tool will identify the issue and tell you exactly how many minutes you are over-scheduled.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/evening-routine-builder](https://vinkius.com/en/ai-agent-connect/evening-routine-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Evening Routine Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `evening-routine-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Evening Routine Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "evening-routine-builder": {
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
