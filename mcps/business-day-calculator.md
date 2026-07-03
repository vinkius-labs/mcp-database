# Business Day Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/business-day-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate workdays, holidays, and business day ranges across 50+ countries.

## Description
The Business Day Calculator MCP connects AI agents to a high-precision utility for global workforce planning. It allows you to perform complex date arithmetic by skipping weekends and public holidays across 50+ countries. Use `add_business_days` to project deadlines, `subtract_business_days` to calculate past work periods, or `count_business_days` to determine the exact number of working days between two dates. The tool supports diverse weekend structures like the Middle East's Friday-Saturday pattern and allows for custom holiday overrides via JSON input.


## Available Tools (5)
- **add_business_days**: Adds N business days to a date
- **count_business_days**: Counts business days between two dates
- **find_next_business_day**: Finds the next business day
- **get_workday_range**: Generates a list of business days in a range
- **subtract_business_days**: Subtracts N business days from a date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Business Day Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If today is 2024-05-01, what is the date after adding 5 business days in the US?"

**🤖 AI Agent:**
> The target date is 2024-05-08.

---

**👤 You:**
> "How many business days are there between 2024-12-24 and 2025-01-02 in the UK?"

**🤖 AI Agent:**
> There are 4 business days between these dates, accounting for Christmas and New Year's holidays.

---

**👤 You:**
> "Find the next business day after 2024-06-14 in the UAE."

**🤖 AI Agent:**
> The next business day is 2024-06-17, as Friday and Saturday are weekends in the UAE.


## ❓ FAQ

**Q: How does the tool handle different weekend structures?**
The tool automatically applies regional rules based on the `countryCode`. For example, it uses a Saturday-Sunday pattern for the US and a Friday-Saturday pattern for many Middle Eastern countries.

**Q: Can I add my own holidays to the calculation?**
Yes, you can provide a JSON array of ISO date strings in the `customHolidaysJson` parameter to treat specific dates as non-working days.

**Q: What happens if I provide an invalid country code?**
If the `countryCode` is unrecognized, the tool will return an error message describing the failure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/business-day-calculator](https://vinkius.com/mcp/business-day-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Business Day Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `business-day-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Business Day Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "business-day-calculator": {
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
