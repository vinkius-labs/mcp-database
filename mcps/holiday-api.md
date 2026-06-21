# Holiday API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/holiday-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage global holidays — audit public and federal holidays via AI.

## Description
Empower your AI agent to orchestrate your entire global event and holiday research workflow with **Holiday API**, the reliable source for holiday data. By connecting Holiday API to your agent, you transform complex calendar auditing into a natural conversation. Your agent can instantly retrieve public holidays for any country, audit workday counts, and identify supported languages without you ever touching a manual calendar. Whether you are planning international logistics or managing global payroll, your agent acts as a real-time event consultant, ensuring your schedules are always accurate and compliant.

### What you can do

- **Holiday Auditing** — Retrieve public and federal holidays for over 200 countries and retrieve detailed metadata, including names and dates.
- **Workday Oversight** — Calculate the next workday or count workdays between two dates to maintain a clear view of operational periods.
- **Global Discovery** — List all supported countries and languages in the Holiday API catalog to identify regional event markers.
- **Temporal Intelligence** — Query holidays for specific years to audit past and future global events instantly.
- **Usage Monitoring** — Get real-time API usage and status metadata to maintain strict control over your research volume.

### How it works

1. Subscribe to this server
2. Enter your Holiday API Key
3. Start managing your event intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Managers** — monitor international holidays and retrieve workday metadata straight from your workflow.
- **HR Specialists** — verify global public holidays and audit payroll cycles without manual searching.
- **Travel Planners** — perform rapid audits of local events and identify peak holiday periods through natural language.
- **Operations Leads** — automate holiday data querying to orchestrate cross-functional global teams smoothly.


## Available Tools (5)
- **get_holidays**: Get public holidays for a country and year
- **get_next_workday**: Get the date after a number of workdays from a start date
- **get_workdays_count**: Count the number of workdays between two dates
- **list_supported_countries**: List all countries supported by Holiday API
- **list_supported_languages**: List all languages supported by Holiday API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Holiday API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the public holidays in 'US' for 2024 using Holiday API?"

**🤖 AI Agent:**
> I've retrieved the 2024 public holidays for the United States. Notable dates include Independence Day on July 4th and Thanksgiving on November 28th. Would you like the full list of federal holidays?

---

**👤 You:**
> "Calculate the next 10 workdays from 2024-01-01 in Brazil."

**🤖 AI Agent:**
> I've calculated the date! After 10 workdays in Brazil starting from January 1st, 2024, the resulting date is January 15th, 2024. I've accounted for the New Year's holiday.

---

**👤 You:**
> "List all countries supported by Holiday API."

**🤖 AI Agent:**
> I've scanned the country catalog. Holiday API supports over 200 countries, including United Kingdom, Germany, and Japan. I can provide the country codes for any of them.


## ❓ FAQ

**Q: How do I find my Holiday API Key?**
Log in to your [**Holiday API dashboard**](https://holidayapi.com/dashboard), and you will find your API Key on the main page. Copy and paste it below.

**Q: Does the agent support historical years?**
Yes. Holiday API provides historical data. Depending on your plan, you can query holidays for past years to audit previous events.

**Q: Can the agent calculate the number of workdays?**
Yes. The `get_workdays_count` tool allows your agent to calculate the exact number of non-holiday business days between two dates for any country.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/holiday-api](https://vinkius.com/mcp/holiday-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Holiday API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `holiday-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Holiday API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "holiday-api": {
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
