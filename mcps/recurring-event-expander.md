# Recurring Event Expander MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recurring-event-expander)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Expands RFC 5545 RRULE strings into concrete lists of occurrence dates.

## Description
The Recurring Event Expander MCP server provides a specialized engine for expanding complex recurrence rules (RFC 5545) into actionable date lists. Using tools like `expand_occurrences`, `validate_rrule`, and `get_rrule_summary`, AI agents can calculate all event dates within a specific window, verify the structural integrity of RRULE strings, and translate technical patterns into human-readable summaries. It supports advanced logic including intervals, BYDAY, BYMONTHDAY, BYSETPOS, and handles exclusions (EXDATE) and additions (RDATE).


## Available Tools (3)
- **expand_occurrences**: Expands an RRULE string into a list of occurrence dates within a window
- **get_rrule_summary**: Generates a human-readable summary of an RRULE
- **validate_rrule**: Validates the syntax of an RRULE string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recurring Event Expander** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Expand this rule: 'FREQ=WEEKLY;BYDAY=MO,WE,FR' from 2024-01-01 to 2024-01-15."

**🤖 AI Agent:**
> The occurrences for the period are: 2024-01-01, 2024-01-03, 2024-01-05, 2024-01-08, 2024-01-10, 2024-01-12, and 2024-01-15.

---

**👤 You:**
> "Is this RRULE syntax correct: 'FREQ=MONTHLY;BYDAY=2TH'"

**🤖 AI Agent:**
> The rule is valid. It represents the second Thursday of every month.

---

**👤 You:**
> "What does this rule mean in plain English: 'FREQ=YEARLY;BYMONTH=12;BYMONTHDAY=25'"

**🤖 AI Agent:**
> This rule represents an event occurring on December 25th every year.


## ❓ FAQ

**Q: What is an RRULE?**
An RRULE (Recurrence Rule) is a standard format defined in RFC 5545 used to describe recurring events, such as 'every Monday' or 'the last Friday of the month'.

**Q: How can I verify if my rule is valid?**
You can use the `validate_rrule` tool to check your RRULE string for structural integrity and compliance with the iCalendar standard.

**Q: Can I exclude specific dates from the expansion?**
Yes, when using `expand_occurrences`, you can provide a list of ISO 8601 timestamps in the `exdates` parameter to exclude them from the resulting list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recurring-event-expander](https://vinkius.com/mcp/recurring-event-expander)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recurring Event Expander** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recurring-event-expander` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recurring Event Expander** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recurring-event-expander": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
