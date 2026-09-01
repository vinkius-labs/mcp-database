# Time-Zone Insulin Adjuster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/time-zone-insulin-adjuster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Deterministic basal insulin and meal timing adjustment calculator for travel.

## Description
This MCP server provides precise calculations for adjusting basal insulin dosing and meal timing when traveling across time zones. By analyzing the direction of travel and the specific insulin type, it provides a complete adjustment plan to maintain glycemic stability. Users can use `calculate_travel_adjustment` to determine dose changes, new injection times, and meal bolus shift instructions. It also includes `get_insulin_type_details` for specific insulin characteristics and `validate_time_format` to ensure input accuracy.


## Available Tools (3)
- **validate_time_format**: Validates that a provided time string adheres to the required HH:mm format
- **calculate_travel_adjustment**: Provides a complete adjustment plan for basal insulin and meal timing based on travel direction and insulin type
- **get_insulin_type_details**: Provides specific characteristics and adjustment logic constraints for different insulin types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Time-Zone Insulin Adjuster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am traveling from UTC+0 to UTC+2 using Degludec. My usual injection time is 08:00. What is my adjustment plan?"

**🤖 AI Agent:**
> The hour difference is 2. Since you are traveling East, the adjustment strategy is to reduce the basal dose by 8% or inject earlier. Your new local injection time will be adjusted accordingly.

---

**👤 You:**
> "I am moving from UTC-5 to UTC-8 using Glargine. My usual time is 22:00. Help me adjust."

**🤖 AI Agent:**
> The hour difference is -3. Traveling West requires increasing the basal dose by 12% or splitting the dose. Your new local injection time will be updated to reflect the longer day.

---

**👤 You:**
> "Is '9:00 AM' a valid time format?"

**🤖 AI Agent:**
> No, the time must be in 24-hour HH:mm format, such as '09:00'.


## ❓ FAQ

**Q: How does the tool handle different insulin types?**
The tool distinguishes between ultra-long acting and long acting insulin. For ultra-long acting types, the `calculate_travel_adjustment` tool prioritizes timing shifts, whereas for long acting types, it focuses on dose percentage adjustments.

**Q: What happens if I travel East versus West?**
When traveling East, the day is shorter, so the tool suggests reducing the basal dose or injecting earlier. When traveling West, the day is longer, so it suggests increasing the dose or splitting it.

**Q: Can I validate my injection time format?**
Yes, you can use the `validate_time_format` tool to ensure your time is in the correct 24-hour HH:mm format.


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
