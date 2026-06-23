# ECB Monetary — Money Supply, Yield Curves & Banknotes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecb-monetary-money-supply-yield-curves-banknotes)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Eurozone monetary data: M1, M2, and M3 money supply aggregates, government bond yield curves from 3 months to 30 years, full yield curve snapshots, and euro banknotes in circulation statistics from the European Central Bank.

## Description
Eurozone monetary data.

### 4 Tools
- **M1/M2/M3** — Money supply aggregates
- **Yield Curve** — Government bonds by maturity
- **Curve Snapshot** — All maturities at once
- **Banknotes** — Euro notes in circulation


## Available Tools (4)
- **get_monetary_aggregate**: M1 = notes, coins + overnight deposits. M2 = M1 + deposits up to 2 years. M3 = M2 + repos + money market funds + debt securities up to 2 years. M3 is the ECB's primary monetary aggregate for policy analysis.

Get eurozone monetary aggregates — M1, M2, M3 money supply
- **get_yield_curve**: AAA-rated or all government bonds. Maturities from 3 months to 30 years. The yield curve shape is a key indicator of economic expectations.

Get the eurozone government bond yield curve for a specific maturity
- **get_yield_curve_snapshot**: Shows the current shape of the eurozone yield curve — normal (upward), flat, or inverted.

Get a full yield curve snapshot — all maturities at the latest date
- **get_banknotes**: Covers all denominations from €5 to €500. Monthly data from the start of the euro.

Get eurozone banknotes in circulation statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ECB Monetary — Money Supply, Yield Curves & Banknotes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current M3 money supply in the eurozone?"

**🤖 AI Agent:**
> 💰 **Eurozone M3 Money Supply**

Latest: €16,423 billion (Feb 2026)
Annual growth: +4.2%

M3 = M2 + repos + money market funds + short-term debt securities

Source: ECB, BSI dataflow

---

**👤 You:**
> "What is the 10-year Eurozone government bond yield?"

**🤖 AI Agent:**
> According to the latest ECB yield curve snapshot, the 10-year Eurozone government bond yield is currently around 2.49%, reflecting updated market expectations across member states.

---

**👤 You:**
> "Show me the growth of euro banknotes in circulation."

**🤖 AI Agent:**
> The total value of euro banknotes in circulation has reached approximately €1,572 billion. I can provide a breakdown of the specific denominations being printed and distributed.


## ❓ FAQ

**Q: What does an inverted yield curve mean?**
An inverted yield curve means short-term bonds yield more than long-term bonds. It often precedes recessions as markets expect central banks to cut rates. An inverted curve has preceded every US recession since 1970.

**Q: Does the server require an API key?**
No, the ECB's public API endpoints do not require any form of authentication or API tokens to fetch statistical data.

**Q: What maturities are included in the yield curve?**
The government bond yield curve data covers maturities ranging from 3 months all the way up to 30 years, giving a complete perspective on borrowing costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecb-monetary-money-supply-yield-curves-banknotes](https://vinkius.com/mcp/ecb-monetary-money-supply-yield-curves-banknotes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ECB Monetary — Money Supply, Yield Curves & Banknotes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ecb-monetary-money-supply-yield-curves-banknotes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ECB Monetary — Money Supply, Yield Curves & Banknotes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ecb-monetary-money-supply-yield-curves-banknotes": {
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
