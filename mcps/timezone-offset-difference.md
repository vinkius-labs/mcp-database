# Timezone Offset Difference MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/timezone-offset-difference)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate hour differences and gaps between UTC offsets.

## Description
This MCP server provides precise tools for temporal calculations involving UTC offsets. Use `get_relative_offset_shift` to find the signed hour difference between two time zones, or `get_absolute_hour_gap` to find the total magnitude of time separating them. It also includes `get_offset_from_total_minutes` for converting minute counts to standard formats and `validate_offset_format` to ensure strings follow the strict ±HH:mm pattern.


## Available Tools (4)
- **get_relative_offset_shift**: Calculates the signed hour difference between two UTC offsets
- **validate_offset_format**: Validates if a string follows the strict ±HH:mm UTC offset format
- **get_absolute_hour_gap**: Calculates the absolute magnitude of hours separating two UTC offsets
- **get_offset_from_total_minutes**: Converts total minutes from UTC into a standard ±HH:mm string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Timezone Offset Difference** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the hour difference between +02:00 and -05:00?"

**🤖 AI Agent:**
> -7

---

**👤 You:**
> "How many hours separate UTC+00:00 and UTC+09:00?"

**🤖 AI Agent:**
> 9

---

**👤 You:**
> "Convert 150 minutes into a UTC offset string."

**🤖 AI Agent:**
> +02:30


## ❓ FAQ

**Q: How do I calculate the shift between two time zones?**
You can use the `get_relative_offset_shift` tool by providing the source and target offsets in the ±HH:mm format.

**Q: What format should the UTC offset be in?**
Offsets must follow the strict ±HH:mm format, such as '+05:30' or '-08:00'. You can use `validate_offset_format` to check your strings.

**Q: Can I find the absolute distance between two offsets?**
Yes, use the `get_absolute_hour_gap` tool to get the non-negative number of hours separating two time zones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/timezone-offset-difference](https://vinkius.com/en/ai-agent-connect/timezone-offset-difference)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Timezone Offset Difference** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `timezone-offset-difference` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Timezone Offset Difference** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "timezone-offset-difference": {
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
