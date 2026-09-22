# Workday Count Utility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/workday-count-utility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate the number of workdays between two dates.

## Description
This MCP server provides precise tools for business date calculations. Use `get_workday_count` to find the total number of weekdays in a range, `is_workday` to check if a specific date is a weekday, `get_workday_distribution` to see the count of each specific weekday, and `check_date_validity` to verify date formats.


## Available Tools (4)
- **check_date_validity**: A validation utility to ensure a date string adheres to the required format and represents a real calendar day
- **get_workday_count**: Calculates the total number of workdays within a specific date range
- **get_workday_distribution**: Provides a breakdown of how many workdays fall on each specific day of the week within a range
- **is_workday**: Determines if a specific date is a standard working day (Monday through Friday)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workday Count Utility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many workdays are there between 2024-01-01 and 2024-01-10?"

**🤖 AI Agent:**
> There are 7 workdays between 2024-01-01 and 2024-01-10.

---

**👤 You:**
> "Is 2024-12-25 a workday?"

**🤖 AI Agent:**
> Yes, 2024-12-25 is a Wednesday, which is a workday.

---

**👤 You:**
> "Give me the distribution of weekdays for the first week of January 2024."

**🤖 AI Agent:**
> In the first week of January 2024, there is 1 Monday, 1 Tuesday, 1 Wednesday, 1 Thursday, and 1 Friday.


## ❓ FAQ

**Q: Are the start and end dates included in the count?**
Yes, if the start or end dates fall on a weekday, they are included in the total count.

**Q: What date format should I use?**
All dates must be provided in the YYYY-MM-DD format.

**Q: Does this tool account for holidays?**
No, this tool specifically counts standard workdays (Monday through Friday) and does not exclude public holidays.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/workday-count-utility](https://vinkius.com/en/ai-agent-connect/workday-count-utility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Workday Count Utility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `workday-count-utility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Workday Count Utility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workday-count-utility": {
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
