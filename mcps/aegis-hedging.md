# AEGIS Hedging MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aegis-hedging)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Energy risk management — manage trades, valuations, and market data via AI.

## Description
Connect your **AEGIS Hedging** (Revenue Intelligence) account to your AI agent to orchestrate your energy risk management and trade lifecycle. From monitoring real-time Mark-to-Market (MTM) valuations to auditing trade entries and retrieving forward market curves, your agent handles complex energy data through natural conversation.

### What you can do

- **Trade Lifecycle Management** — List and audit trades executed on the AEGIS Marketplace and monitor their status in your system
- **Valuation & MTM** — Retrieve current Mark-to-Market data and settlement estimates for your hedge positions
- **Market Intelligence** — Access energy forward curves, historical price data, and daily market insights
- **Reporting & Compliance** — Retrieve normalized data for revenue, taxes, and fees to support financial forecasting and SDR reporting
- **Strategic Oversight** — Quickly identify portfolio risks or hedging opportunities based on current market volatility

### How it works

1. Subscribe to this server
2. Enter your AEGIS Instance URL and Bearer Token
3. Start managing your energy risk and trade data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Energy Risk Managers** — monitor hedge percentages and portfolio VaR (Value at Risk) instantly
- **Financial Controllers** — audit trade entries and retrieve data for month-end accounting
- **Traders & Analysts** — access forward curves and market insights for faster decision making
- **Compliance Officers** — verify SDR reporting and maintain a complete audit trail of hedging activities


## Available Tools
- **list_trades**: List energy hedge trades
- **get_valuations**: Get real-time MTM valuations
- **get_forward_curves**: Retrieve energy forward curves
- **check_api_version**: Check AEGIS API version


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AEGIS Hedging** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all energy trades executed in the last 30 days."

**🤖 AI Agent:**
> I've retrieved your trade logs. You have 12 new trades executed on the AEGIS SEF in the last 30 days, including natural gas swaps and crude oil options. Would you like to see the valuation for these positions?

---

**👤 You:**
> "Show me the current Mark-to-Market valuation for my natural gas portfolio."

**🤖 AI Agent:**
> I've analyzed your natural gas positions. Based on current forward curves, your MTM valuation is +$1.2M. The settlement estimate for the next month is currently trending higher due to market volatility. Would you like to see the underlying data?

---

**👤 You:**
> "Retrieve the energy forward curves for the next 12 months."

**🤖 AI Agent:**
> I've retrieved the forward market data. The curves show a steady increase in pricing for Q4 2026. I've prepared a summary of the monthly benchmarks for you. Would you like to audit your current hedge coverage against these curves?


## ❓ FAQ

**Q: How do I find my AEGIS Bearer Token?**
Bearer tokens are managed within your AEGIS platform settings under the API or Integrations section. If you don't have access, contact your AEGIS Administrator or Account Manager.

**Q: Can I see real-time Mark-to-Market valuations?**
Yes! Use the `get_valuations` tool. It retrieves the latest Mark-to-Market (MTM) data and settlement estimates for your active hedge positions.

**Q: Does this support trade automation from the SEF?**
The `list_trades` tool allows your agent to audit trades executed on the AEGIS SEF (Swap Execution Facility), supporting straight-through processing into your internal systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aegis-hedging](https://vinkius.com/mcp/aegis-hedging)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AEGIS Hedging** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `aegis-hedging` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AEGIS Hedging** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aegis-hedging": {
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
