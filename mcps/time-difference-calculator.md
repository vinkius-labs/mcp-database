# Time Difference Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/time-difference-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate exact duration between two clock times, handling midnight transitions.

## Description
This MCP server provides precise tools to calculate the elapsed time between two timestamps in a 24-hour format. Using `calculate_time_span`, you can find the exact hours and minutes passed, even if the period crosses midnight. The `detect_day_transition` tool identifies if a duration spans across a new day, while `summarize_time_difference` formats your results into a clean, human-readable string like '2h 30m'. It is ideal for scheduling, logging, and temporal analysis tasks.


## Available Tools (3)
- **detect_day_transition**: Detect if a period crosses midnight
- **summarize_time_difference**: Format duration into a string
- **calculate_time_span**: Handles midnight transitions.

Calculate exact duration between two times


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Time Difference Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much time is between 23:00 and 02:30?"

**🤖 AI Agent:**
> The duration is 3 hours and 30 minutes.

---

**👤 You:**
> "Calculate the span from 14:00 to 15:45."

**🤖 AI Agent:**
> The elapsed time is 1 hour and 45 minutes.

---

**👤 You:**
> "Format the duration of 5 hours and 10 minutes for me."

**🤖 AI Agent:**
> The formatted duration is 5h 10m.


## ❓ FAQ

**Q: How do I handle time ranges that cross midnight?**
The `calculate_time_span` tool automatically detects if the end time is earlier than the start time and adjusts the calculation to account for the day rollover.

**Q: What time format should I use?**
All inputs must be provided in the 24-hour HH:MM format (e.g., '09:30' or '22:15').

**Q: Can I use this to check if a day transition occurred?**
Yes, you can use the `detect_day_transition` tool to specifically identify if your specified time range includes a crossing of the midnight threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/time-difference-calculator](https://vinkius.com/mcp/time-difference-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Time Difference Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `time-difference-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Time Difference Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "time-difference-calculator": {
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
