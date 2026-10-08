# Personal Challenge Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personal-challenge-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate and manage structured completion schedules for personal discipline challenges.

## Description
Transform abstract goals into concrete, day-by-day activity calendars. This MCP server provides tools to `generate_challenge_calendar` for new schedules, `log_daily_completion` to track progress, `mark_day_as_skipped` for planned breaks, and `get_challenge_summary` to monitor streaks and milestones. It is designed to help users maintain discipline through structured planning and progress tracking.


## Available Tools (4)
- **generate_challenge_calendar**: 
- **get_challenge_summary**: 
- **log_daily_completion**: 
- **mark_day_as_skipped**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Challenge Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 30-day pushup challenge starting tomorrow with a milestone at 50 pushups."

**🤖 AI Agent:**
> Your 30-day pushup challenge has been scheduled. The estimated end date is October 25th, 2024, with your first milestone at 50 repetitions.

---

**👤 You:**
> "I completed 15 pushups today for my challenge."

**🤖 AI Agent:**
> Progress logged. You have completed 15% of your total repetitions and your current streak is 1 day.

---

**👤 You:**
> "Show me my progress for the current challenge."

**🤖 AI Agent:**
> You are 45% complete. Your current streak is 5 days, and you have 12 active days remaining.


## ❓ FAQ

**Q: How do I start a new challenge?**
You can use the `generate_challenge_calendar` tool to create a master schedule by providing a start date, total repetitions, and your desired frequency.

**Q: What happens if I miss a day?**
You can use `mark_day_as_skipped` to record a planned break. This will adjust your schedule without reducing your total repetition target.

**Q: How can I see my current progress?**
Use the `get_challenge_summary` tool to view your completion percentage, current streak, and progress toward specific milestones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personal-challenge-calendar](https://vinkius.com/en/ai-agent-connect/personal-challenge-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Challenge Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-challenge-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Challenge Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-challenge-calendar": {
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
