# Max Drawdown Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/max-drawdown-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate maximum drawdown, recovery periods, and stress indicators from historical price series.

## Description
The Max Drawdown Calculator is a specialized risk assessment tool designed to analyze financial volatility. By processing historical price data, it provides critical insights into investment risk using tools like `calculate_max_drawdown` for identifying the worst-case decline, `calculate_recovery_metrics` for analyzing bounce-back durations, `calculate_ulcer_index` for measuring accumulated psychological stress, and `get_current_drawdown_status` to compare recent prices against historical peaks.


## Available Tools (4)
- **calculate_max_drawdown**: Identify the single worst percentage decline and its duration
- **calculate_recovery_metrics**: Analyze how long it takes for assets to bounce back after losing value
- **get_current_drawdown_status**: Compare the most recent market state against historical highs
- **calculate_ulcer_index**: Provide a single metric representing the accumulated psychological stress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Max Drawdown Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the maximum drawdown for this price series: [{'timestamp': '2023-01-01', 'value': 100}, {'timestamp': '2023-01-02', 'value': 80}, {'timestamp': '2023-01-03', 'value': 90}]?"

**🤖 AI Agent:**
> The maximum drawdown was 20.0% (from 100 to 80) occurring between 2023-01-01 and 2023-01-02.

---

**👤 You:**
> "Calculate the Ulcer Index for these prices: [{'timestamp': '2023-01-01', 'value': 100}, {'timestamp': '2023-01-02', 'value': 90}, {'timestamp': '2023-01-03', 'value': 85}]"

**🤖 AI Agent:**
> The Ulcer Index value is 7.54.

---

**👤 You:**
> "Is the current price of 105 at an all-time high based on this history: [{'timestamp': '2023-01-01', 'value': 110}, {'timestamp': '2023-01-02', 'value': 105}]?"

**🤖 AI Agent:**
> No, the current price is not at an all-time high. It is currently in a drawdown of 4.55% from the peak of 110.


## ❓ FAQ

**Q: What is the purpose of the `calculate_max_drawdown` tool?**
It identifies the single largest percentage drop from a peak to a trough within your provided price series.

**Q: How can I measure investment stress?**
You can use the `calculate_ulcer_index` tool, which quantifies the depth and duration of drawdowns to represent accumulated psychological stress.

**Q: Can I check if my asset is currently at an all-time high?**
Yes, the `get_current_drawdown_status` tool compares the most recent price in your series to the historical peak.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/max-drawdown-calculator](https://vinkius.com/mcp/max-drawdown-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Max Drawdown Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `max-drawdown-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Max Drawdown Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "max-drawdown-calculator": {
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
