# Family Anniversary Reminder Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-anniversary-reminder-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate your family celebrations by transforming occasions into actionable reminder schedules.

## Description
This MCP server helps you manage significant life events by calculating necessary preparation times and organizing notifications. Use `generate_reminder_plan` to create a chronological calendar of reminders based on your event dates and lead times. You can also use `get_upcoming_reminders` to view scheduled notifications within a specific timeframe, `validate_notification_config` to check supported communication channels, and `calculate_preparation_window` to understand the time needed for each event.


## Available Tools (4)
- **calculate_preparation_window**: Determines the total range of preparation required for a specific occasion
- **generate_reminder_plan**: Transforms a set of occasions and lead times into a chronologically ordered calendar of reminders
- **get_upcoming_reminders**: Retrieves a filtered list of reminders that are scheduled to occur within a specific timeframe
- **validate_notification_config**: g., Email, SMS, Push).

Ensures that the requested notification channels are supported by the system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Anniversary Reminder Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a reminder plan for Mom's birthday on June 15th with a 7-day lead time, and for our Wedding Anniversary on October 20th with a 14-day lead time. Recipients are Mom (Email) and Dad (SMS)."

**🤖 AI Agent:**
> Here is your reminder plan: 1. June 8th: Mom's Birthday (Email), 2. October 6th: Wedding Anniversary (SMS), 3. October 6th: Wedding Anniversary (Email).

---

**👤 You:**
> "What reminders are scheduled between 2024-05-01 and 2024-06-30?"

**🤖 AI Agent:**
> You have one reminder scheduled: June 8th for Mom's Birthday.

---

**👤 You:**
> "How many days do I need to prepare if I have a 10-day lead time?"

**🤖 AI Agent:**
> You have 10 days to prepare before the event occurs.


## ❓ FAQ

**Q: How do I create a new reminder schedule?**
You can use the `generate_reminder_plan` tool by providing your occasions and recipient details.

**Q: Can I check which reminders are coming up soon?**
Yes, use the `get_upcoming_reminders` tool to filter reminders within a specific date range.

**Q: What notification channels are supported?**
The system supports standard channels like Email, SMS, and Push. You can verify specific support using `validate_notification_config`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-anniversary-reminder-plan](https://vinkius.com/en/ai-agent-connect/family-anniversary-reminder-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Anniversary Reminder Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-anniversary-reminder-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Anniversary Reminder Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-anniversary-reminder-plan": {
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
