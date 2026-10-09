# Event RSVP Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/event-rsvp-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate event attendance statistics and response breakdowns.

## Description
This MCP server provides tools to manage and analyze event guest lists. Use `get_rsvp_summary` to see totals for confirmed, declined, and pending guests, or `get_attendance_milestones` to track progress toward specific attendance goals. You can also use `filter_guests_by_status` to isolate specific groups or `get_response_velocity` to monitor engagement levels.


## Available Tools (4)
- **get_rsvp_summary**: Get a summary of RSVP responses and attendance rate
- **filter_guests_by_status**: Filter the guest list by their response status
- **get_attendance_milestones**: Check progress towards specific attendance goals
- **get_response_velocity**: Calculate the response rate and pending ratio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Event RSVP Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current breakdown of my guest responses and the expected attendance rate?"

**🤖 AI Agent:**
> You have 45 confirmed guests, 10 declined, and 25 pending. The total invitations are 80, and your current attendance rate is 56.25%.

---

**👤 You:**
> "How close am I to reaching 80% attendance?"

**🤖 AI Agent:**
> Your current attendance is 56.25%. You need 9 more confirmed responses to reach your 80% goal.

---

**👤 You:**
> "Show me the names of everyone who has confirmed."

**🤖 AI Agent:**
> The confirmed guests are: Alice Smith, Bob Jones, and Charlie Brown.


## ❓ FAQ

**Q: How do I get a summary of my guest responses?**
You can use the `get_rsvp_summary` tool by providing your guest list as a JSON array.

**Q: Can I track if I have reached my attendance goal?**
Yes, use `get_attendance_milestones` with your target percentage to see if your goal is reached.

**Q: How can I see only the guests who have declined?**
Use the `filter_guests_by_status` tool and set the status filter to 'declined'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/event-rsvp-counter](https://vinkius.com/en/ai-agent-connect/event-rsvp-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Event RSVP Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `event-rsvp-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Event RSVP Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "event-rsvp-counter": {
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
