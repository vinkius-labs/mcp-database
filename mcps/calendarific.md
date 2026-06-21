# Calendarific MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calendarific)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access global holiday data via Calendarific — track public, religious, and local holidays across 230+ countries directly from any AI agent.

## Description
Connect your **Calendarific** account to any AI agent and orchestrate your global scheduling, vacation planning, and local observability through natural conversation.

### What you can do

- **Holiday Oversight** — List all public, religious, and local holidays for a specific country and year.
- **Regional Observability** — Filter holidays by state or region to ensure your planning accounts for local variations.
- **Categorized Discovery** — List holidays by type, such as National, Observance, or Religious holidays.
- **Country & Language Directory** — Access the list of 230+ supported countries and their respective ISO codes.
- **Date-Specific Queries** — Retrieve holidays for a specific month or day to verify work availability.
- **Reference Data** — Get detailed metadata for each holiday, including descriptions and observance regions.

### How it works

1. Subscribe to this server
2. Enter your Calendarific API Key
3. Start exploring global holidays from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations & Project Managers** — quickly check for upcoming holidays in international offices without manual searches.
- **Travel & Logistics Teams** — retrieve holiday calendars for planning and resource allocation straight from their workflow tools.
- **Developers** — integrate holiday checking logic into their applications using natural language.


## Available Tools
- **get_account_info**: Check the status of the integration
- **list_supported_countries**: List all supported countries and their ISO codes
- **list_holidays_by_location**: List holidays for a specific state or region
- **list_holidays_by_type**: List holidays filtered by type (e.g. national, religious)
- **list_holidays**: List holidays for a specific country and year
- **list_supported_languages**: List all supported languages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calendarific** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all public holidays in Brazil for 2024."

**🤖 AI Agent:**
> I've retrieved the holidays for Brazil. There are several upcoming observances, including 'Carnaval' (Feb 12-13) and 'Tiradentes' (Apr 21). Would you like the full list?

---

**👤 You:**
> "Are there any holidays in New York (US-NY) on December 25th?"

**🤖 AI Agent:**
> Yes, December 25th is 'Christmas Day' in New York, which is a federal and state holiday in the US.

---

**👤 You:**
> "Show me the religious holidays in Italy for 2024."

**🤖 AI Agent:**
> Retrieving religious holidays for Italy... Notable dates include 'Epiphany' (Jan 6), 'Easter Monday' (Apr 1), and 'All Saints' Day' (Nov 1).


## ❓ FAQ

**Q: How do I list all the holidays for a specific country in 2024?**
Simply ask the agent to `list_holidays` and provide the Country code (e.g., 'US' or 'BR') and the year '2024'. It will retrieve the full list from Calendarific.

**Q: Can I filter holidays by type, like only religious holidays?**
Yes! Use the `list_holidays_by_type` tool and provide the country, year, and type (e.g., 'religious'). Your agent will return only the matching observances.

**Q: How do I see which countries are supported by Calendarific?**
Use the `list_supported_countries` tool. It will retrieve the complete directory of over 230 countries currently available in the Calendarific API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calendarific](https://vinkius.com/mcp/calendarific)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calendarific** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `calendarific` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calendarific** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calendarific": {
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
