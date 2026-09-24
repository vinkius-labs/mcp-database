# Jet Lag Adjustment Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/jet-lag-adjustment-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Calculate the days needed to adjust to new time zones.

## Description
This MCP server provides tools to manage circadian rhythm adjustments during travel. Use `get_adjustment_duration` to find the total days required for synchronization, `validate_shift_capacity` to ensure your daily shift limit is healthy, `get_travel_direction_impact` to identify travel direction, and `calculate_sync_progress` to track your adjustment status.


## Available Tools (4)
- **calculate_sync_progress**: Calculates how much of the total adjustment process is complete after a certain number of days
- **get_adjustment_duration**: Calculates how many days a traveler needs to stay at a destination to fully adjust to the new time zone
- **get_travel_direction_impact**: Determines whether the traveler is moving East or West to provide context for the adjustment
- **validate_shift_capacity**: Checks if a proposed daily shift limit is within a healthy physiological range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jet Lag Adjustment Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days will it take to adjust to a 9 hour time difference if I shift 2 hours per day?"

**🤖 AI Agent:**
> It will take 5 days to fully adjust to the new time zone.

---

**👤 You:**
> "Is a 4 hour daily shift limit safe?"

**🤖 AI Agent:**
> A 4 hour daily shift limit is above the typical healthy range of 1 to 3 hours per day.

---

**👤 You:**
> "I've been adjusting for 2 days with a 2 hour daily limit for a 6 hour offset. How much progress have I made?"

**🤖 AI Agent:**
> You have completed 66.67% of your adjustment, with 2 hours remaining to sync.


## ❓ FAQ

**Q: How do I know how many days I need to adjust?**
You can use the `get_adjustment_duration` tool by providing the total timezone offset and your preferred daily shift limit.

**Q: Is there a safe limit for shifting my body clock?**
Yes, you can use `validate_shift_capacity` to check if your proposed daily shift limit falls within a healthy physiological range.

**Q: Can I track my progress during the adjustment period?**
Yes, the `calculate_sync_progress` tool allows you to see the percentage of adjustment completed based on days elapsed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/jet-lag-adjustment-calculator](https://vinkius.com/en/ai-agent-connect/jet-lag-adjustment-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jet Lag Adjustment Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jet-lag-adjustment-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jet Lag Adjustment Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jet-lag-adjustment-calculator": {
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
