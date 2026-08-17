# Timezone Meeting Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/timezone-meeting-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate global meetings by calculating overlapping working hours and DST offsets.

## Description
A deterministic engine for global time coordination. This MCP server allows AI agents to calculate precise meeting windows across multiple IANA time zones. It accounts for specific Daylight Saving Time (DST) transitions, provides exact UTC offsets for any given date, and identifies overlapping availability based on individual working hour constraints. Use `find_meeting_windows` to discover all possible meeting times or `validate_availability` to check a specific slot.


## Available Tools (3)
- **find_meeting_windows**: Identifies all time periods where all participants' working hours overlap
- **get_zone_offsets**: Retrieves the specific UTC offset for a list of time zones on a given date
- **validate_availability**: Checks if a specific proposed meeting time is valid for all participants


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Timezone Meeting Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find a meeting window for a team in New York (09:00-17:00) and London (09:00-17:00) on 2024-06-15."

**🤖 AI Agent:**
> The available meeting window is from 2024-06-15T13:00:00+00:00 to 2024-06-15T16:00:00+00:00, lasting 180 minutes.

---

**👤 You:**
> "What is the UTC offset for Tokyo on 2024-12-25?"

**🤖 AI Agent:**
> The UTC offset for Asia/Tokyo on 2024-12-25 is +09:00.

---

**👤 You:**
> "Is 2024-03-10T02:30:00-05:00 a valid time for someone in New York?"

**🤖 AI Agent:**
> No, that time is invalid because a DST transition is occurring at that moment in the America/New_York time zone.


## ❓ FAQ

**Q: How does the tool handle Daylight Saving Time?**
The engine uses the IANA database to calculate exact offsets for any date. If a DST transition occurs during a proposed meeting, the `dstTransitionOccurred` flag will be set to true.

**Q: Can I check if a specific time works for my team?**
Yes, you can use the `validate_availability` tool to verify if a specific ISO 8601 timestamp falls within the working hours of all participants.

**Q: What format should the time zones be in?**
You must use standard IANA time zone identifiers, such as `America/New_York` or `Europe/London`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/timezone-meeting-planner](https://vinkius.com/ai-agent-connect/timezone-meeting-planner)
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
