# iCalendar RRULE Iterator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/icalendar-rrule-iterator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Expand iCalendar recurrence rules into exact, deterministic event sequences.

## Description
The iCalendar RRULE Iterator is a precision engine designed to expand complex recurrence rules into chronological lists of timestamps. By utilizing UTC-based integer math, it ensures that event sequences remain identical regardless of the server's local timezone or daylight saving transitions. Use `decompose_rrule` to inspect rule components like FREQ and INTERVAL, `calculate_event_dates` to generate precise occurrence lists from a start date, and `audit_rule_syntax` to verify that your RRULE strings follow the correct structural syntax for scheduling.


## Available Tools (3)
- **audit_rule_syntax**: Audits the syntax of an RRULE
- **decompose_rrule**: Decomposes an RRULE into its constituent parts
- **calculate_event_dates**: Calculates event dates based on an RRULE


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iCalendar RRULE Iterator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the next three dates for a weekly event starting on 2024-01-01 with an interval of 2?"

**🤖 AI Agent:**
> The occurrences for RRULE:FREQ=WEEKLY;INTERVAL=2 starting from 2024-01-01 are: 2024-01-01, 2024-01-15, and 2024-01-29.

---

**👤 You:**
> "Check if this RRULE is valid: FREQ=MONTHLY;INTERVAL=1"

**🤖 AI Agent:**
> The syntax for the provided rule is valid and contains a properly defined frequency.

---

**👤 You:**
> "Break down this rule: FREQ=DAILY;COUNT=5"

**🤖 AI Agent:**
> The decomposed components are: FREQ: DAILY, COUNT: 5.


## ❓ FAQ

**Q: How does the engine handle timezone changes?**
The engine uses UTC-based integer math via the V8 Date object, ensuring that all calculations are deterministic and unaffected by local timezone shifts or daylight saving transitions.

**Q: Can I verify if my RRULE string is valid before processing it?**
Yes, you can use the `audit_rule_syntax` tool to check for structural errors like missing FREQ properties or malformed intervals.

**Q: What parameters can I extract from a rule?**
By using `decompose_rrule`, you can extract key-value pairs such as FREQ, INTERVAL, COUNT, and UNTIL to understand the rule's configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/icalendar-rrule-iterator](https://vinkius.com/ai-agent-connect/icalendar-rrule-iterator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **iCalendar RRULE Iterator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `icalendar-rrule-iterator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **iCalendar RRULE Iterator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "icalendar-rrule-iterator": {
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
