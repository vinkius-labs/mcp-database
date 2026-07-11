# Timezone Meeting Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/timezone-meeting-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Find optimal meeting times across international timezones by analyzing business hour overlaps and DST transitions.

## Description
A specialized utility for scheduling meetings across multiple cities. It analyzes 24-hour schedules, identifies daylight saving time (DST) conflicts using `dst_transitions`, and ranks the best 3 meeting windows based on an 'inconvenience score' via `rank_optimal_slots` to minimize disruption to participants' local business hours.


## Available Tools (4)
- **dst_transitions**: Identify upcoming Daylight Saving Time transitions for specific timezones
- **optimal_slots**: Find the best meeting time slots across multiple timezones
- **schedule_matrix**: Generate a 24-hour meeting availability matrix for multiple timezones
- **timezone_search**: Search for IANA timezones by city or region name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Timezone Meeting Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find a meeting time for London and New York on 2024-05-20."

**🤖 AI Agent:**
> The best meeting window is between 13:00 and 15:00 UTC, as this falls within business hours for both cities.

---

**👤 You:**
> "Search for timezones in Tokyo."

**🤖 AI Agent:**
> Found matching timezone: Asia/Tokyo.

---

**👤 You:**
> "Are there any DST transitions for Paris in 2024?"

**🤖 AI Agent:**
> Yes, a transition is detected on 2024-03-31.


## ❓ FAQ

**Q: How are meeting slots ranked?**
The `rank_optimal_slots` tool calculates an inconvenience score based on how far the slot is from the 09:00-17:00 business window.

**Q: Can I identify DST changes?**
Yes, use the `dst_transitions` tool to flag dates where clock offsets change for your selected cities.

**Q: How do I find a specific timezone?**
You can use the `timezone_search` tool to search for city or region names and get valid IANA identifiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/timezone-meeting-planner](https://vinkius.com/mcp/timezone-meeting-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Timezone Meeting Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `timezone-meeting-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Timezone Meeting Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "timezone-meeting-planner": {
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
