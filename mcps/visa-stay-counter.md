# Visa Stay Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/visa-stay-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track visa usage and calculate remaining stay days.

## Description
This MCP server provides precise tools to manage visa durations. Use `calculate_stay_status` to determine used days, remaining days, and your latest legal exit date. You can also use `validate_visit_dates` to check date logic, `get_total_consumed_days` for cumulative usage, or `predict_future_entry_impact` to see how upcoming trips affect your limit.


## Available Tools (4)
- **calculate_stay_status**: Determine used days, remaining days, and the latest legal exit date
- **get_total_consumed_days**: Calculate the cumulative days spent in the territory
- **predict_future_entry_impact**: Estimate how a planned upcoming trip will affect the remaining visa allowance
- **validate_visit_dates**: Ensure entry and exit dates follow logical and temporal rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Visa Stay Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days have I used if my limit is 90 days and I visited from 2024-01-01 to 2024-01-15?"

**🤖 AI Agent:**
> You have used 15 days, leaving you with 75 days remaining.

---

**👤 You:**
> "Check my status: 30 day limit, visits: [{'entryDate': '2024-05-01', 'exitDate': '2024-05-10'}]"

**🤖 AI Agent:**
> You have used 10 days and have 20 days remaining.

---

**👤 You:**
> "Will a trip from 2024-08-01 to 2024-08-10 cause an overstay if I have 5 days left?"

**🤖 AI Agent:**
> No, that trip will use 10 days, which exceeds your remaining 5 days, so you will overstay.


## ❓ FAQ

**Q: How are stay durations calculated?**
The duration is calculated by counting the days from the entry date to the exit date, inclusive of both dates.

**Q: Can I check my status if I am currently in the country?**
Yes, by using `calculate_stay_status` and omitting the exit date for your current visit, the tool uses the current date to calculate your ongoing stay.

**Q: How do I plan for future trips?**
Use the `predict_future_entry_impact` tool to estimate how a planned trip will affect your remaining visa allowance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/visa-stay-counter](https://vinkius.com/en/ai-agent-connect/visa-stay-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Visa Stay Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `visa-stay-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Visa Stay Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "visa-stay-counter": {
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
