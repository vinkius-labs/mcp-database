# Family Birthday Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-birthday-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and count birthday occurrences within specific timeframes.

## Description
This MCP server provides tools to manage and query birthday data from a calendar list. You can use `get_birthday_counts` to find how many birthdays occur in a date range, `find_upcoming_birthdays` to see who has a birthday coming up, `validate_calendar_integrity` to check for duplicates, and `filter_birthdays_by_month` to isolate specific months.


## Available Tools (4)
- **filter_birthdays_by_month**: Extracts all birthday occurrences for a specific month within a given year
- **find_upcoming_birthdays**: Identifies all birthdays occurring between today and a specified future date
- **get_birthday_counts**: Finds how many birthdays occur within a specific timeframe
- **validate_calendar_integrity**: Checks the provided calendar list for duplicate entries or invalid date formats


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Birthday Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many birthdays are there between 2024-01-01 and 2024-12-31?"

**🤖 AI Agent:**
> There are 5 birthdays in total for the year 2024.

---

**👤 You:**
> "Who has a birthday in the next 7 days?"

**🤖 AI Agent:**
> Alice has a birthday on 2024-05-20.

---

**👤 You:**
> "Show me all birthdays in May 2024."

**🤖 AI Agent:**
> The birthdays in May 2024 are Alice (2024-05-20) and Bob (2024-05-15).


## ❓ FAQ

**Q: How do I check for upcoming birthdays?**
Use the `find_upcoming_birthdays` tool by providing your calendar list and the number of days into the future you wish to look.

**Q: Can I verify if my calendar has duplicate entries?**
Yes, the `validate_calendar_integrity` tool checks your list for duplicate names on the same date or invalid formats.

**Q: How can I see how many birthdays happen in a specific year?**
You can use `get_birthday_counts` to specify a start and end date for the year you are interested in.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-birthday-counter](https://vinkius.com/en/ai-agent-connect/family-birthday-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Birthday Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-birthday-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Birthday Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-birthday-counter": {
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
