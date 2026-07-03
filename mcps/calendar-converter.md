# Calendar Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calendar-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert dates between 15+ calendar systems including Gregorian, Chinese, Persian, and Japanese Era.

## Description
The Calendar Converter MCP server provides a powerful engine for bidirectional date conversions across over 15 distinct solar, lunar, and lunisolar calendar systems. Using Unix timestamps as a universal pivot, it allows AI agents to bridge the gap between different cultural and historical timekeeping methods.

Key capabilities include:
- **Multi-Calendar Conversion**: Seamlessly convert dates between Gregorian, Julian, Islamic (Hijri), Hebrew, Persian (Solar Hijri), Buddhist, Chinese, Ethiopian, Coptic, Indian National, Japanese Era, Thai Solar, and Unix timestamps.
- **Temporal Expansion**: Use the `expand_unix` tool to take a single Unix timestamp and instantly see its equivalent date and era/zodiac details across multiple requested calendars.
- **Cultural Metadata Retrieval**: Access seasonal or era-based metadata using `get_calendar_context`. For example, find the Chinese Zodiac animal for a specific year or identify the Imperial Era in the Japanese calendar.
- **Precise Timestamping**: Use `convert_to_unix` to find the exact Unix epoch for any valid date in supported systems, including hours, minutes, and seconds.

This server is ideal for applications requiring historical accuracy, cultural awareness, or cross-calendar synchronization.


## Available Tools (3)
- **convert_to_unix**: Do NOT use if you already have the timestamp.

Convert a date in a specific calendar to Unix timestamp
- **expand_unix**: Do NOT use for simple date formatting.

Expand a Unix timestamp into multiple calendars
- **get_calendar_context**: Do NOT use for timestamp conversion.

Get metadata for a specific year in a calendar system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calendar Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the Unix timestamp for January 1, 2000 at 12:00:00 UTC in the Gregorian calendar?"

**🤖 AI Agent:**
> 946694400

---

**👤 You:**
> "What is the Chinese Zodiac animal for the year 2024?"

**🤖 AI Agent:**
> The year 2024 is the Year of the Dragon.

---

**👤 You:**
> "Expand Unix timestamp 1704067200 to Gregorian and Persian calendars."

**🤖 AI Agent:**
> For the timestamp 1704067200, the Gregorian date is January 1, 2024, and the Persian (Solar Hijri) date is Dey 12, 1402.


## ❓ FAQ

**Q: Which calendar systems are supported?**
The server supports over 15 systems, including Gregorian, Julian, Islamic (Hijri), Hebrew, Persian (Solar Hijri), Buddhist, Chinese, Ethiopian, Coptic, Indian National, Japanese Era, Thai Solar, and Unix timestamps.

**Q: How can I see the Chinese Zodiac for a specific year?**
You can use the `get_calendar_context` tool with `calendarType` set to 'chinese' and provide the desired year.

**Q: Can I convert a Unix timestamp to multiple calendars at once?**
Yes, by using the `expand_unix` tool and providing a JSON array of the target calendar types you wish to expand into.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calendar-converter](https://vinkius.com/mcp/calendar-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calendar Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `calendar-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calendar Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calendar-converter": {
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
