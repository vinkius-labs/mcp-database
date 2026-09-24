# Family Calendar Days MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-calendar-days)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze family calendar durations, activity density, and overlapping events.

## Description
This MCP server provides tools to analyze the temporal properties of family calendars. Use `get_calendar_summary` to see the total span and active days, `count_category_days` to find how many days are dedicated to specific activities like vacations, `find_overlapping_events` to identify simultaneous events, and `get_activity_density` to measure how busy a calendar is over a specific timeframe.


## Available Tools (4)
- **count_category_days**: Determines how many days are dedicated to a specific type of activity
- **find_overlapping_events**: Identifies periods where multiple events are occurring simultaneously
- **get_activity_density**: Analyzes how "busy" a calendar is by comparing active days to total span
- **get_calendar_summary**: Provides a high-level overview of the calendar's temporal footprint


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Calendar Days** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of the calendar with ID 'fam-123'."

**🤖 AI Agent:**
> The calendar 'fam-123' spans 30 days in total, with 12 unique active days and 5 total events recorded.

---

**👤 You:**
> "How many days are dedicated to 'Vacation' in calendar 'fam-123'?"

**🤖 AI Agent:**
> There are 7 total days and 7 unique active days dedicated to the 'Vacation' category in this calendar.

---

**👤 You:**
> "Are there any overlapping events in calendar 'fam-123'?"

**🤖 AI Agent:**
> Yes, there is an overlap on 2024-07-04 involving event IDs 'evt-001' and 'evt-002'.


## ❓ FAQ

**Q: How does the tool handle overlapping events?**
The `get_calendar_summary` tool counts unique active days, meaning if two events overlap on the same date, that date is only counted once in the active day total.

**Q: Can I filter by specific event types?**
Yes, you can use `count_category_days` to determine the total and unique active days for any specific category like 'Vacation' or 'School Holiday'.

**Q: What is activity density?**
Activity density is a score calculated by the `get_activity_density` tool, representing the ratio of active days to the total number of days in a given timeframe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-calendar-days](https://vinkius.com/en/ai-agent-connect/family-calendar-days)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Calendar Days** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-calendar-days` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Calendar Days** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-calendar-days": {
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
