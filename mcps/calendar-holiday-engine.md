# Calendar & Holiday Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/calendar-holiday-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate exact dates for global holidays across Gregorian, Islamic, Hebrew, Chinese, and Hindu calendars.

## Description
This MCP server provides high-precision temporal calculations for global holidays. It bridges AI agents to multiple calendrical systems, including Gregorian, Islamic (Hijri), Hebrew (Lunisolar), Chinese (Lunisolar), and Hindu calendars. Use `get_holidays_by_year` to retrieve a full list of dates for any year between 1583 and 9999, or `get_holiday_details` to find specific metadata for a single event. The engine also supports `check_holiday_proximity` to determine the temporal distance to upcoming or past holidays relative to a specific date.


## Available Tools (3)
- **check_holiday_proximity**: Answers how many days remain until the next upcoming holiday or how many days have passed since the last one
- **get_holiday_details**: Provide the exact name of the holiday.

Provides deep metadata for a specific holiday occurring in a specific year
- **get_holidays_by_year**: You can optionally provide a country code to filter for public holidays.

Returns a complete list of all holidays for a specific year across all supported calendar systems and countries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calendar & Holiday Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What holidays are there in 2025 in the USA?"

**🤖 AI Agent:**
> In 2025, the USA has holidays such as New Year's Day on January 1st, Martin Luther King Jr. Day on January 20th, and Memorial Day on May 26th.

---

**👤 You:**
> "How many days until Christmas 2024?"

**🤖 AI Agent:**
> Christmas is on December 25th, 2024.

---

**👤 You:**
> "When is Eid al-Fitr in 2025?"

**🤖 AI Agent:**
> Eid al-Fitr in 2025 is expected to fall around March 30th.


## ❓ FAQ

**Q: What is the supported year range?**
The engine supports any year from 1583 to 9999.

**Q: Can I check if a holiday is a public holiday?**
Yes, by providing a valid ISO 3166-1 alpha-2 country code, the tools will indicate if the holiday is officially recognized in that territory.

**Q: Which calendar systems are supported?**
The engine supports Gregorian, Christian-Movable, Hijri, Hebrew, Chinese, Hindu, and Secular calendar systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/calendar-holiday-engine](https://vinkius.com/ai-agent-connect/calendar-holiday-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calendar & Holiday Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `calendar-holiday-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calendar & Holiday Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calendar-holiday-engine": {
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
