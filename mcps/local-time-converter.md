# Local Time Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-time-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert dates and times between different UTC offsets.

## Description
This MCP server provides precise temporal conversion tools. Use `convert_time_between_offsets` to shift a specific moment from one timezone to another, or `calculate_offset_difference` to find the exact time gap between two regions. It also includes `validate_iso_format` for timestamp verification and `get_timezone_relation` to compare offsets.


## Available Tools (4)
- **calculate_offset_difference**: Calculates the difference in hours and minutes between two UTC offsets
- **convert_time_between_offsets**: Converts a date and time between two supplied UTC offsets
- **validate_iso_format**: Validates if a timestamp string follows the ISO 8601 format
- **get_timezone_relation**: Determines if one timezone is ahead of, behind, or equal to another


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Time Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What time will it be in London (+01:00) if it is 14:00 in New York (-05:00)?"

**🤖 AI Agent:**
> It will be 20:00 in London.

---

**👤 You:**
> "How many hours difference is there between +05:00 and -03:00?"

**🤖 AI Agent:**
> There is an 8 hour difference between these two offsets.

---

**👤 You:**
> "Is '2023-12-25T12:00:00Z' a valid ISO 8601 timestamp?"

**🤖 AI Agent:**
> Yes, the timestamp is valid.


## ❓ FAQ

**Q: What format should the timestamp be in?**
Timestamps must follow the ISO 8601 standard for accurate conversion.

**Q: How do I specify the UTC offset?**
Offsets should be provided with a sign and HH:mm format, such as '+05:00' or '-08:00'.

**Q: Can I compare two different timezones?**
Yes, you can use `get_timezone_relation` to determine if one zone is ahead of, behind, or equal to another.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-time-converter](https://vinkius.com/en/ai-agent-connect/local-time-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Time Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-time-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Time Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-time-converter": {
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
