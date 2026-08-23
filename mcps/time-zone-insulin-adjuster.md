# Time-Zone Insulin Adjuster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/time-zone-insulin-adjuster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Deterministic insulin basal adjustment and meal timing calculator for travel.

## Description
This MCP server provides precise insulin management strategies for travelers. By calculating the difference between departure and destination time zones, it generates specific instructions for basal insulin adjustments and meal bolus shifts. Use `calculate_travel_plan` to receive a complete adjustment strategy, including dose percentage changes and new local injection times. You can also use `get_insulin_type_guidance` to understand how rigid or flexible insulin profiles interact with circadian rhythm shifts.


## Available Tools (3)
- **calculate_travel_plan**: 
- **get_insulin_type_guidance**: 
- **validate_time_formats**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Time-Zone Insulin Adjuster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am traveling from UTC+0 to UTC+2 using flexible insulin. My usual injection time is 08:00. What is my plan?"

**🤖 AI Agent:**
> The hour difference is 2 hours. For traveling East with flexible insulin, your adjustment strategy is to reduce the basal dose by 8%. Your new local injection time will be 08:00, and you should align meal boluses to destination local time immediately.

---

**👤 You:**
> "What is the difference between rigid and flexible insulin profiles?"

**🤖 AI Agent:**
> Rigid profiles are highly predictable with minimal titration, while flexible profiles allow for moderate dose adjustments to accommodate day-length changes.

---

**👤 You:**
> "I'm flying from UTC-5 to UTC-8. My basal insulin is rigid and I usually inject at 20:00. Help me plan."

**🤖 AI Agent:**
> The hour difference is -3 hours. Traveling West with rigid insulin requires adjusting timing. Your adjustment strategy involves increasing the dose or splitting the dose by 12%. Your new local injection time is 20:00.


## ❓ FAQ

**Q: How does this tool help with insulin adjustment?**
The `calculate_travel_plan` tool calculates the exact hour difference between time zones and provides a specific dose adjustment percentage and new local injection time to maintain glycemic control.

**Q: Can I use this for different types of insulin?**
Yes, the server supports both rigid and flexible insulin profiles. You can use `get_insulin_type_guidance` to learn more about how each type behaves during travel.

**Q: What happens to my meal times when I travel?**
The tool provides `mealBolusShiftInstructions` to help you align your carbohydrate-related insulin shots to the destination's local meal times immediately upon arrival.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/time-zone-insulin-adjuster](https://vinkius.com/ai-agent-connect/time-zone-insulin-adjuster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Time-Zone Insulin Adjuster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `time-zone-insulin-adjuster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Time-Zone Insulin Adjuster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "time-zone-insulin-adjuster": {
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
