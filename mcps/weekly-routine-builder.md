# Weekly Routine Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/weekly-routine-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Construct realistic weekly schedules by balancing physiological needs and personal priorities.

## Description
This MCP server provides a specialized scheduling engine designed to build balanced weekly routines. It manages the complex interplay between fixed obligations, sleep hygiene, nutritional rhythms, and movement requirements. By using `get_available_capacity`, the engine calculates remaining time, while `build_tentative_routine` intelligently places meals, exercise, and high-priority tasks into available gaps. Users can ensure their schedule is sustainable using `validate_routine_health` to check for physiological balance, or use `identify_schedule_conflicts` to diagnose why certain tasks cannot be accommodated.


## Available Tools (4)
- **validate_routine_health**: Checks the generated routine against physiological and logical health standards
- **build_tentative_routine**: Attempts to place meals, movement, and personal priorities into the available gaps
- **get_available_capacity**: Calculates the remaining free time in a week after accounting for fixed obligations and sleep
- **identify_schedule_conflicts**: Pinpoints the specific cause of scheduling failures


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weekly Routine Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 168 hours total. I need 8 hours of sleep per night. I work Monday to Friday from 9 AM to 5 PM. Can you build a routine for me?"

**🤖 AI Agent:**
> I have calculated your capacity and generated a routine. Your schedule includes 8 hours of sleep nightly, your work blocks, and has successfully integrated meal times and exercise sessions into your remaining free time.

---

**👤 You:**
> "Why can't I fit my gym session into my current schedule?"

**🤖 AI Agent:**
> The conflict is due to an overlap between your scheduled gym session and your fixed work obligation from 9 AM to 5 PM.

---

**👤 You:**
> "Is my current weekly schedule balanced?"

**🤖 AI Agent:**
> Your routine has a health score of 85. It is well-balanced, though there is a warning that your movement frequency is slightly lower than recommended.


## ❓ FAQ

**Q: How does the engine handle conflicting tasks?**
The engine uses `identify_schedule_conflicts` to pinpoint whether a failure is due to an overlap with fixed obligations, insufficient total time, or a priority failure.

**Q: Can I check if my routine is healthy?**
Yes, the `validate_routine_health` tool evaluates your schedule against physiological standards, providing a health score and warnings about meal gaps or movement frequency.

**Q: What information is needed to start building a routine?**
You need to provide your total available weekly hours, your sleep target, a list of fixed obligations, and your requirements for meals, movement, and priority tasks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/weekly-routine-builder](https://vinkius.com/en/ai-agent-connect/weekly-routine-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weekly Routine Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weekly-routine-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weekly Routine Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weekly-routine-builder": {
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
