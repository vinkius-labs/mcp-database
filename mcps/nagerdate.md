# Nager.Date MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nagerdate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage public holidays worldwide — audit global events and calendars via AI.

## Description
Empower your AI agent to orchestrate your entire public holiday and global event research workflow with **Nager.Date**, the open source API for world holidays. By connecting Nager.Date to your agent, you transform complex calendar auditing into a natural conversation. Your agent can instantly retrieve public holidays for over 100 countries, audit upcoming events worldwide, and identify regional variations without you ever touching a manual calendar. Whether you are planning international logistics or managing global product launches, your agent acts as a real-time event consultant, ensuring your schedules are always accurate and well-informed.

### What you can do

- **Holiday Auditing** — Retrieve all public holidays for any specific country and year to maintain a clear view of global event cycles.
- **Real-time Status** — Check if today is a public holiday in any country to assist in immediate operational decision-making.
- **Event Discovery** — Retrieve the next occurring public holidays worldwide to understand global temporal patterns instantly.
- **Regional Intelligence** — Query country-specific details, including common names and geographic regions, to assist in localization.
- **Global Discovery** — List all available countries in the Nager.Date catalog to identify regional event markers.

### How it works

1. Subscribe to this server
2. No API Key required (Nager.Date is a free and open service)
3. Start managing your global intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Managers** — monitor international holiday patterns and retrieve event metadata straight from your workflow.
- **Product Owners** — verify global launch dates and audit regional temporal constraints without manual searching.
- **HR Specialists** — perform rapid audits of public holidays for cross-functional global teams through natural language.
- **Operations Leads** — automate global event querying to orchestrate cross-functional international teams smoothly.


## Available Tools (6)
- **get_country_details**: Get additional details for a specific country
- **get_next_holidays**: Get the next public holidays for a specific country
- **is_holiday_today**: Check if today is a public holiday in a country
- **get_next_holidays_worldwide**: Get the next public holidays occurring worldwide
- **list_available_countries**: Date.

List all countries supported by Nager.Date
- **get_public_holidays**: Get all public holidays for a country and year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nager.Date** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the public holidays in 'US' for 2024 using Nager.Date?"

**🤖 AI Agent:**
> I've retrieved the 2024 public holidays for the United States. Notable dates include New Year's Day on January 1st and Independence Day on July 4th. Would you like the full list of dates?

---

**👤 You:**
> "Is today a public holiday in Brazil?"

**🤖 AI Agent:**
> I've checked the holiday status for Brazil. Today is not identified as a public holiday. The next upcoming holiday is Tiradentes Day on April 21st.

---

**👤 You:**
> "Show the next 5 public holidays occurring worldwide."

**🤖 AI Agent:**
> I've identified the next 5 global holidays. They include events in countries like Australia, India, and Norway. Would you like the local names and specific dates for each?


## ❓ FAQ

**Q: Is an API Key required for Nager.Date?**
No. Nager.Date is a free and open service. This server works out of the box without any static credentials required.

**Q: Can the agent check if today is a holiday?**
Yes. Use the `is_holiday_today` tool providing the 2-letter country code. Your agent will return a boolean indicating if it is a public holiday today instantly.

**Q: Does it support local names for holidays?**
Yes. The holiday records retrieved by your agent include both the English name and the local name used in that specific country.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nagerdate](https://vinkius.com/mcp/nagerdate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nager.Date** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nagerdate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nager.Date** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nagerdate": {
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
