# ISO 8601 Duration Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iso-8601-duration-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Extracts time components and calculates total seconds from ISO 8601 duration strings.

## Description
This MCP server provides deterministic parsing of ISO 8601 duration strings. It allows AI agents to break down time spans into specific components like years, months, and days, or convert a full duration into a total count of seconds. Use `parse_duration_components` to get a detailed breakdown, `calculate_total_seconds` for a single numeric magnitude, or `validate_syntax` to ensure a string follows the strict ISO 8601 format.


## Available Tools (3)
- **calculate_total_seconds**: Determines the total magnitude of a duration in seconds
- **parse_duration_components**: Extracts individual time units from a valid ISO 8601 duration string
- **validate_syntax**: Checks if a given string strictly adheres to the ISO 8601 duration specification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ISO 8601 Duration Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many seconds are in the duration P1Y?"

**🤖 AI Agent:**
> 31536000

---

**👤 You:**
> "Break down the duration P1M2DT3H."

**🤖 AI Agent:**
> 1 month, 2 days, and 3 hours.

---

**👤 You:**
> "Is 'PT15M' a valid ISO 8601 duration?"

**🤖 AI Agent:**
> Yes, it is a valid duration representing 15 minutes.


## ❓ FAQ

**Q: How are years and months calculated?**
To ensure deterministic results, a year is treated as exactly 365 days and a month is treated as exactly 30 days.

**Q: Can I validate a duration string before parsing it?**
Yes, you can use the `validate_syntax` tool to check if a string adheres to the ISO 8601 specification before attempting to extract components.

**Q: What tools are available in this MCP?**
The server provides `parse_duration_components` for unit extraction, `calculate_total_seconds` for magnitude calculation, and `validate_syntax` for format verification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iso-8601-duration-parser](https://vinkius.com/mcp/iso-8601-duration-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ISO 8601 Duration Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `iso-8601-duration-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ISO 8601 Duration Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "iso-8601-duration-parser": {
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
