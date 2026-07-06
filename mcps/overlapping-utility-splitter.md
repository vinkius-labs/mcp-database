# Overlapping Utility Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/overlapping-utility-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Splits utility bills between two residents when one moves out mid-cycle.

## Description
This MCP server provides tools to accurately divide utility costs when occupancy changes during a billing period. Using `calculate_split_amounts`, you can determine the exact portion each person owes based on their days in the property. You can also use `get_daily_cost_rate` to find the daily cost and `validate_residency_period` to ensure your input dates are logically sound within the billing cycle.


## Available Tools (3)
- **get_daily_cost_rate**: Calculates the daily cost rate of a utility
- **calculate_split_amounts**: Calculates the utility bill split between two residents
- **validate_residency_period**: Validates the residency period timeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Overlapping Utility Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The electric bill is $150 for a 30-day cycle. Person A moved out on day 12. How much should they pay?"

**🤖 AI Agent:**
> Person A owes $60.00, and Person B owes $90.00.

---

**👤 You:**
> "What is the daily rate for a $300 water bill over 31 days?"

**🤖 AI Agent:**
> $9.68 per day.

---

**👤 You:**
> "Is it valid to say someone moved out on day 35 of a 30-day cycle?"

**🤖 AI Agent:**
> No, that is not a valid residency period as the move-out day exceeds the billing cycle duration.


## ❓ FAQ

**Q: How does the split calculation work?**
It uses `calculate_split_amounts` to find a daily rate and allocates costs based on how many days each person resided in the property.

**Q: Can I verify if my move-out date is valid?**
Yes, use the `validate_residency_period` tool to check if the departure day falls within the billing cycle.

**Q: What inputs are needed for the split?**
You need the total bill amount, the day person A moved out, and the total days in the billing cycle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/overlapping-utility-splitter](https://vinkius.com/mcp/overlapping-utility-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Overlapping Utility Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `overlapping-utility-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Overlapping Utility Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "overlapping-utility-splitter": {
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
