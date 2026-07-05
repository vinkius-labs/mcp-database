# Fasting Window Resolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fasting-window-resolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate and track feeding and fasting windows with precision.

## Description
The Fasting Window Resolver MCP server provides tools to manage intermittent fasting schedules. Use `get_current_state_details` to determine if you are currently in a feeding or fasting window, `get_window_boundaries` to see your full daily schedule including midnight transitions, and `calculate_duration_until_event` to find out exactly how much time remains until your next meal.


## Available Tools (3)
- **get_current_state_details**: Determines the user's current physiological state and how much time remains before the next transition
- **calculate_duration_until_event**: Calculates how much time remains before a specific target time is reached
- **get_window_boundaries**: Retrieves the complete schedule of all four boundary timestamps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fasting Window Resolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I start eating at 12:00 and my window is 8 hours long. What is my current state right now at 15:00?"

**🤖 AI Agent:**
> You are currently in your feeding window.

---

**👤 You:**
> "Show me all the boundaries for an 8-hour eating window starting at 12:00."

**🤖 AI Agent:**
> Your fasting window starts at 20:00 and your feeding window begins at 12:00.

---

**👤 You:**
> "It is 10:00. How long until my meal at 12:00?"

**🤖 AI Agent:**
> There are 2 hours remaining until your target time of 12:00.


## ❓ FAQ

**Q: How do I know if I am currently fasting?**
You can use the `get_current_state_details` tool by providing your feeding window start time, the duration of your feeding window, and the current time.

**Q: Can this tool handle schedules that cross midnight?**
Yes, the `get_window_boundaries` tool is specifically designed to calculate all four boundary timestamps, even when your schedule wraps around midnight.

**Q: How much time is left until my next meal?**
Use the `calculate_duration_until_event` tool. Just provide your target meal time and the current reference time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fasting-window-resolver](https://vinkius.com/mcp/fasting-window-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fasting Window Resolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fasting-window-resolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fasting Window Resolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fasting-window-resolver": {
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
