# Injection Day Alignment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/injection-day-alignment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate precise medication injection schedules and manage weekday alignment shifts.

## Description
This MCP server provides precision utilities for managing recurring medical injections. Use `get_injection_schedule` to generate a full list of injection dates based on an initial date and frequency, with the ability to align the schedule to a preferred weekday. The `calculate_shift_offset` tool determines the exact delay needed to reach a target day of the week, while `verify_schedule_compliance` ensures that your provided list of dates adheres strictly to the required dosing interval.


## Available Tools (3)
- **calculate_shift_offset**: Determines exactly how many days of delay are highly required to move a medication day to a preferred weekday
- **get_injection_schedule**: Calculates a full list of injection dates based on a starting point and a frequency, with optional weekday realignment
- **verify_schedule_compliance**: Checks a provided list of dates against a specific frequency rule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Injection Day Alignment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate an injection schedule starting on 2024-05-01, every 7 days, for 5 doses, aligned to Thursdays."

**🤖 AI Agent:**
> The calculated schedule is: ['2024-05-02', '2024-05-09', '2024-05-16', '2024-05-23', '2024-05-30'].

---

**👤 You:**
> "How many days do I need to wait to move my Tuesday injection to a Friday?"

**🤖 AI Agent:**
> You will need to wait 3 days to reach the next Friday.

---

**👤 You:**
> "Check if this schedule is compliant: ['2024-01-01', '2024-01-08', '2024-01-15'] with a 7-day frequency."

**🤖 AI Agent:**
> The schedule is compliant and consistent with the 7-day frequency rule.


## ❓ FAQ

**Q: How can I align my injection to a specific day of the week?**
When using `get_injection_schedule`, provide the `targetDayOfWeek` parameter (0 for Sunday, 6 for Saturday). The tool will calculate the necessary shift delay and generate the sequence starting from that aligned date.

**Q: Can I verify if my current schedule is correct?**
Yes, use the `verify_schedule_compliance` tool. Input your list of dates and the expected frequency in days to check for any missed or incorrectly dated doses.

**Q: What format should I use for dates?**
All dates must be provided in ISO 8601 format (YYYY-MM-DD) to ensure accuracy and compatibility.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/injection-day-alignment](https://vinkius.com/mcp/injection-day-alignment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Injection Day Alignment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `injection-day-alignment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Injection Day Alignment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "injection-day-alignment": {
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
