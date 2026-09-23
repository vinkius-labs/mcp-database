# Calendar Free Time MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/calendar-free-time)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate available time windows by subtracting scheduled commitments from an availability period.

## Description
This MCP server provides tools to manage and analyze availability. It allows AI agents to calculate total free time using `get_availability_summary`, identify specific available windows with `list_free_time_slots`, verify if a new event fits using `check_slot_availability`, and measure schedule disruption via `calculate_fragmentation_index`.


## Available Tools (4)
- **calculate_fragmentation_index**: Answers "How interrupted is my free time?"
- **check_slot_availability**: Answers "Can I fit a specific task/meeting into my current schedule?"
- **get_availability_summary**: Answers "How much total free time do I have within my active hours?"
- **list_free_time_slots**: Answers "When exactly are my available windows?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calendar Free Time** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much total free time do I have between 9:00 AM and 5:00 PM if I have a meeting from 10:00 AM to 11:00 AM?"

**🤖 AI Agent:**
> You have 7 hours (420 minutes) of total free time available.

---

**👤 You:**
> "When are my available windows between 1:00 PM and 4:00 PM if I am busy from 2:00 PM to 2:30 PM?"

**🤖 AI Agent:**
> Your available windows are 1:00 PM to 2:00 PM and 2:30 PM to 4:00 PM.

---

**👤 You:**
> "Can I fit a 45-minute meeting from 3:00 PM to 3:45 PM into my schedule?"

**🤖 AI Agent:**
> Yes, that time slot is available.


## ❓ FAQ

**Q: How do I know if a meeting fits in my schedule?**
You can use the `check_slot_availability` tool to verify if a specific time range is available within your defined availability period.

**Q: Can I see my exact free time slots?**
Yes, the `list_free_time_slots` tool returns a list of all continuous available windows between your scheduled commitments.

**Q: How much total free time is left in my day?**
The `get_availability_summary` tool calculates the total minutes of free time remaining within your active hours.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/calendar-free-time](https://vinkius.com/en/ai-agent-connect/calendar-free-time)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calendar Free Time** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `calendar-free-time` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calendar Free Time** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calendar-free-time": {
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
