# Advanced Timezone Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/advanced-timezone-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Precise IANA timezone operations including historical DST transitions, ambiguity detection, and global time synchronization.

## Description
The Advanced Timezone Engine provides high-fidelity temporal operations using the IANA Timezone Database (TZDB) for the years 1970 through 2030. This MCP server acts as a bridge, allowing AI agents to perform complex timezone calculations with extreme precision.

Key capabilities include:
- **Time Conversion**: Convert timestamps between any two IANA timezones while automatically accounting for historical Daylight Saving Time (DST) rules using `convert_time`.
- **Global Synchronization**: Identify all active timezones globally that currently display a specific local time via `find_active_zones`.
- **Historical Analysis**: Retrieve the exact UTC offset for any timezone at any point in history or the near future with `get_historical_offset`.
- **DST Transition Detection**: Detect 'Spring Forward' invalid times and 'Fall Back' ambiguous times using `check_datetime_validity` to ensure temporal accuracy during DST shifts.
- **Standardized Formatting**: Generate precise, timezone-aware ISO 8601 strings with `format_iso_8601`.

This engine is designed for developers and AI agents requiring reliable, automated handling of complex temporal logic without manual offset calculations.


## Available Tools (5)
- **check_datetime_validity**: Checks if a specific time is valid in a timezone
- **find_active_zones**: Finds all timezones displaying a specific local time
- **format_iso8601**: Formats an ISO 8601 string into a readable format
- **get_historical_offset**: Retrieves the UTC offset for a specific timezone at a given time
- **convert_time**: Converts a timestamp from one timezone to another


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Advanced Timezone Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 2024-03-10T01:30:00 to America/New_York."

**🤖 AI Agent:**
> The converted time in America/New_York is 2024-03-10T01:30:00-04:00. Note that this specific time was invalid due to the DST spring forward transition.

---

**👤 You:**
> "What is the UTC offset for Europe/London on 2023-07-01?"

**🤖 AI Agent:**
> The UTC offset for Europe/London on 2023-07-01 is +01:00.

---

**👤 You:**
> "Is the time 2024-11-03T01:30:00 in America/New_York valid?"

**🤖 AI Agent:**
> The status is AMBIGUOUS. This time occurs twice during the DST fall-back transition.


## ❓ FAQ

**Q: What is the supported date range for timezone operations?**
The engine supports all dates from 1970 through 2030, covering historical and near-future DST transitions.

**Q: How does the tool handle Daylight Saving Time (DST) changes?**
The tool automatically detects if a time is invalid due to 'Spring Forward' or ambiguous due to 'Fall Back' transitions using the IANA database.

**Q: Can I find all cities where it is currently 9:00 AM?**
Yes, by using the `find_active_zones` tool with the target time '09:00'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/advanced-timezone-engine](https://vinkius.com/mcp/advanced-timezone-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Advanced Timezone Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `advanced-timezone-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Advanced Timezone Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "advanced-timezone-engine": {
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
