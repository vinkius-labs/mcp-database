# Break Reminder Schedule MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/break-reminder-schedule)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates work-break reminders and total break time based on your work hours and focus intervals.

## Description
This MCP server helps you manage your energy by calculating optimal break times. By providing your work window, focus intervals, and scheduled interruptions like meetings or lunch, you can use `get_break_schedule` to receive specific timestamps for when to stop working. You can also use `validate_work_window` to ensure your schedule is logically sound, `calculate_focus_capacity` to see how much work you can fit in, and `get_break_density` to check if your work-to-rest ratio is healthy.


## Available Tools (4)
- **get_break_density**: 
- **get_break_schedule**: 
- **validate_work_window**: 
- **calculate_focus_capacity**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Break Reminder Schedule** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my break schedule for a workday from 9:00 AM to 5:00 PM with 50 minute focus intervals and 10 minute breaks. I have a meeting from 11:00 AM to 11:30 AM."

**🤖 AI Agent:**
> Your scheduled breaks are at 9:50 AM, 10:50 AM, 12:40 PM, 1:40 PM, 2:40 PM, 3:40 PM, and 4:40 PM. Your total break time is 70 minutes.

---

**👤 You:**
> "Is my schedule valid? I work from 8:00 AM to 4:00 PM and have a meeting from 1:00 PM to 2:00 PM."

**🤖 AI Agent:**
> Yes, your schedule is logically consistent.

---

**👤 You:**
> "How many focus intervals can I complete between 10:00 AM and 2:00 PM if my focus interval is 45 minutes and I have a meeting from 12:00 PM to 12:30 PM?"

**🤖 AI Agent:**
> You can complete 3 full focus intervals.


## ❓ FAQ

**Q: How do I get my break times?**
You can use the `get_break_schedule` tool by providing your start time, end time, focus interval, and break duration.

**Q: Can I include meetings in my schedule?**
Yes, you can provide a list of meetings to ensure breaks are not scheduled during your meetings.

**Q: How does the tool handle lunch?**
You can specify a lunch period to ensure the scheduling logic accounts for this interruption.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/break-reminder-schedule](https://vinkius.com/en/ai-agent-connect/break-reminder-schedule)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Break Reminder Schedule** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `break-reminder-schedule` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Break Reminder Schedule** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "break-reminder-schedule": {
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
