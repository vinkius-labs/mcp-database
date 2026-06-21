# ECB Full — Complete Eurozone Financial Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecb-full-complete-eurozone-financial-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

The definitive ECB Mega-Server: 14 tools for EUR exchange rates against 40+ currencies, key interest rates (MRO, DFR, MLFR), MFI bank rates, monetary aggregates (M1/M2/M3), government bond yield curves, euro banknotes, and a universal SDMX query engine for all ECB statistical data.

## Description
The **ultimate ECB Mega-Server** — 14 tools across 4 domains.

### 14 Tools
- 💱 Exchange Rates (3) — Single, multi-currency, latest
- 🏦 Interest Rates (5) — MRO, DFR, MLFR, all, MFI
- 💰 Monetary (4) — M1/M2/M3, yield curve, banknotes
- 🔍 Discovery (2) — Dataflows catalog, generic query

### No API Key Required


## Available Tools
- **list_dataflows**: Each dataflow has a code (e.g., EXR, FM, BSI) and description. Use these codes with the generic query tool to access any ECB data.

List all available ECB statistical dataflows
- **query_ecb_data**: Provide the dataflow code (EXR, FM, BSI, YC, MIR, BKN, etc.) and a SDMX series key. Use list_dataflows to find dataflow codes. Example: dataflow=EXR, key=D.USD.EUR.SP00.A for daily USD/EUR rate.

Query any ECB dataset with a SDMX series key — universal access
- **get_exchange_rate**: Daily, monthly, or annual frequency. The ECB publishes reference rates for ~40 currencies against the euro at around 16:00 CET each business day.

Get the EUR exchange rate against a specific currency from the ECB
- **get_multiple_rates**: Separate currency codes with commas. Useful for comparing EUR strength across multiple currencies.

Get EUR exchange rates against multiple currencies simultaneously
- **get_latest_rates**: Published daily at ~16:00 CET. Includes USD, GBP, JPY, CHF, CNY, AUD, CAD, and more.

Get the latest ECB reference exchange rates for all currencies
- **get_key_rates**: This is the rate at which banks can borrow from the ECB for one week. It's the most important eurozone interest rate for monetary policy.

Get the ECB's key interest rates — the main refinancing rate (MRO)
- **get_deposit_rate**: Since October 2019, this has become the most closely watched ECB rate as it effectively determines the lower bound of money market rates.

Get the ECB deposit facility rate — the floor of the interest rate corridor
- **get_marginal_lending_rate**: Forms the upper bound of the ECB's interest rate corridor.

Get the ECB marginal lending facility rate — the ceiling of the rate corridor
- **get_all_key_rates**: Shows the full rate corridor.

Get all 3 ECB key interest rates together: MRO, deposit, and marginal lending
- **get_mfi_rates**: Shows what banks actually charge/pay for loans and deposits. Key indicator of monetary policy transmission.

Get MFI interest rates — bank lending and deposit rates in the eurozone
- **get_monetary_aggregate**: M1 = notes, coins + overnight deposits. M2 = M1 + deposits up to 2 years. M3 = M2 + repos + money market funds + debt securities up to 2 years. M3 is the ECB's primary monetary aggregate for policy analysis.

Get eurozone monetary aggregates — M1, M2, M3 money supply
- **get_yield_curve**: AAA-rated or all government bonds. Maturities from 3 months to 30 years. The yield curve shape is a key indicator of economic expectations.

Get the eurozone government bond yield curve for a specific maturity
- **get_yield_curve_snapshot**: Shows the current shape of the eurozone yield curve — normal (upward), flat, or inverted.

Get a full yield curve snapshot — all maturities at the latest date
- **get_banknotes**: Covers all denominations from €5 to €500. Monthly data from the start of the euro.

Get eurozone banknotes in circulation statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ECB Full — Complete Eurozone Financial Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Full eurozone briefing: EUR rates, interest rates, yield curve, and money supply"

**🤖 AI Agent:**
> 🏦 **ECB Full Briefing**

💱 EUR/USD: 1.0842 | EUR/GBP: 0.8567 | EUR/JPY: 163.42
🏦 DFR: 2.50% | MRO: 2.65% | MLFR: 2.90%
📈 10Y Yield: 2.49% | 2Y: 2.31% (curve normal)
💰 M3: €16,423B (+4.2% YoY)
💶 Banknotes: €1,572B in circulation

5 ECB data sources queried simultaneously.

---

**👤 You:**
> "Show me the latest ECB key interest rates."

**🤖 AI Agent:**
> Here are the current key interest rates: the deposit facility rate (DFR) is at 2.50%, the main refinancing operations (MRO) is at 2.65%, and the marginal lending facility rate (MLFR) is at 2.90%.

---

**👤 You:**
> "What are the latest Eurozone monetary aggregates?"

**🤖 AI Agent:**
> The latest broad monetary aggregate M3 shows an annual growth rate of 4.2%. I can break this down into M1 and M2 components if you'd like to dive deeper.


## ❓ FAQ

**Q: Why Full instead of individual servers?**
The Full server has all 14 tools covering exchange rates, interest rates, monetary aggregates, yield curves, and data discovery. Query EUR/USD AND deposit rates AND yield curves AND M3 in a single session. Completely free and unrestricted.

**Q: Does the ECB Full server have authentication requirements?**
No, all 14 tools use the official public ECB SDMX APIs which require absolutely no authentication, tokens, or registration.

**Q: How quickly is the data refreshed?**
Data strictly reflects the European Central Bank's schedule in real-time. For example, the euro foreign exchange reference rates are updated every working day around 16:00 CET.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecb-full-complete-eurozone-financial-intelligence](https://vinkius.com/mcp/ecb-full-complete-eurozone-financial-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ECB Full — Complete Eurozone Financial Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ecb-full-complete-eurozone-financial-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ECB Full — Complete Eurozone Financial Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ecb-full-complete-eurozone-financial-intelligence": {
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
