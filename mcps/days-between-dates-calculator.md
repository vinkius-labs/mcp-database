# Days Between Dates Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/days-between-dates-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise intervals between two dates in years, months, weeks, and days.

## Description
This MCP server provides specialized tools to calculate the exact time elapsed between two dates. Use `get_date_breakdown` to receive a detailed breakdown of years, months, weeks, and days. You can also use `count_business_days` to determine the number of working days between two periods while optionally excluding regional holidays in the USA or Europe. Additionally, `verify_holiday_status` allows you to check if a specific date is recognized as a national holiday within your selected region.


## Available Tools
- **count_business_days**: Calculates the total number of working days between two dates
- **get_date_breakdown**: Provides a detailed breakdown of the time elapsed between two dates
- **verify_holiday_status**: Checks if a specific date is recognized as a national holiday in a given region


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Days Between Dates Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days are between 2023-01-01 and 2023-12-31?"

**🤖 AI Agent:**
> You can use `get_date_breakdown` with startDate: '2023-01-01' and endDate: '2023-12-31' to see the exact breakdown.

---

**👤 You:**
> "Check if 2024-07-04 is a holiday in the USA."

**🤖 AI Agent:**
> The `verify_holiday_status` tool can confirm this by checking targetDate: '2024-07-04' and region: 'USA'.

---

**👤 You:**
> "Calculate working days between 2024-01-01 and 2024-01-10, excluding holidays."

**🤖 AI Agent:**
> Use `count_business_days` with startDate: '2024-01-01', endDate: '2024-01-10', and excludeHolidays: true.


## ❓ FAQ

**Q: How do I calculate business days excluding holidays?**
Use the `count_business_days` tool and set the `excludeHolidays` parameter to true.

**Q: Which regions are supported for holiday lookups?**
The server currently supports holiday registries for the USA and Europe.

**Q: Can I get a breakdown of weeks and days?**
Yes, the `get_date_breakdown` tool provides a full breakdown including years, months, weeks, and remaining days.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/days-between-dates-calculator](https://vinkius.com/mcp/days-between-dates-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Days Between Dates Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `days-between-dates-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Days Between Dates Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "days-between-dates-calculator": {
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
