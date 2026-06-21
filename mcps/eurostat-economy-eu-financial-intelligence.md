# Eurostat Economy — EU Financial Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eurostat-economy-eu-financial-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Official EU economic data: quarterly GDP for all 27 member states, government debt and deficit (Maastricht criteria), HICP inflation (the ECB's target measure), interest rates, and EUR exchange rates.

## Description
Connect your AI agent to the official economic statistics of the European Union.

### What you can do
- **GDP** — Quarterly and annual GDP for all 27 EU countries + euro area. Components: consumption, investment, government spending, trade
- **Government Debt** — Public debt (% of GDP) and deficit/surplus. Maastricht criteria monitoring: 60% debt ceiling, 3% deficit limit
- **Inflation (HICP)** — The Harmonised Index of Consumer Prices — the official inflation measure used by the ECB. Monthly rates, annual averages, by COICOP category
- **Interest Rates** — Short-term and long-term government bond yields across the EU
- **Exchange Rates** — EUR vs USD, GBP, JPY, CHF and 30+ currencies
- **Generic Query** — Access any of 7,000+ Eurostat datasets by code

### No API Key Required
Eurostat provides completely open, free access. No registration needed.

### Who is this for?
ECB watchers, sovereign debt analysts, EU policy researchers, macro strategists, and anyone tracking European economic performance.


## Available Tools
- **get_gdp**: Dataset: namq_10_gdp (quarterly) or nama_10_gdp (annual). Filter by country, unit (CLV10_MEUR, CP_MEUR, PC_GDP), and GDP component (B1GQ=GDP, P3=consumption, P5G=investment).

Get EU GDP data by country — quarterly or annual
- **get_government_debt**: Dataset: gov_10dd_edpt1 (annual EDP). Critical for Maastricht criteria monitoring (60% debt, 3% deficit).

Get EU government debt and deficit by country
- **get_inflation**: Datasets: prc_hicp_manr (annual rate, monthly), prc_hicp_mmor (monthly rate), prc_hicp_aind (annual average). The ECB targets 2% HICP inflation. Filter by country and COICOP category.

Get EU inflation (HICP) — the official measure used by the ECB
- **get_interest_rates**: Datasets: irt_st_m (short-term, monthly), irt_lt_mcby_m (long-term government bond yields). Key for ECB policy analysis.

Get EU short-term and long-term interest rates
- **get_exchange_rates**: Dataset: ert_bil_eur_m (monthly) or ert_bil_eur_d (daily).

Get EUR bilateral exchange rates against major currencies
- **get_economic_dataset**: Use the Eurostat Data Browser to find codes. Common: nama_10_gdp, gov_10q_ggnfa, tec00115, teina225.

Query any Eurostat economy/finance dataset by code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eurostat Economy — EU Financial Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare GDP growth across Germany, France, Italy, and Spain"

**🤖 AI Agent:**
> 🇪🇺 **GDP Growth — Top 4 Economies**

| Country | 2023 | 2024-Q3 |
|---------|------|--------|
| 🇩🇪 Germany | -0.3% | +0.2% |
| 🇫🇷 France | +0.7% | +1.1% |
| 🇮🇹 Italy | +0.9% | +0.7% |
| 🇪🇸 Spain | +2.5% | +3.1% |

Spain leads the Big 4 recovery. Germany narrowly avoided recession.

---

**👤 You:**
> "What is the current inflation rate in the eurozone?"

**🤖 AI Agent:**
> 📈 **Euro Area HICP Inflation**

Annual rate: 2.4%
ECB target: 2.0%
Core (ex food/energy): 2.7%

Highest: Estonia (4.1%), Croatia (3.8%)
Lowest: Finland (0.8%), Lithuania (1.1%)

Inflation converging toward ECB target but services inflation remains sticky.

---

**👤 You:**
> "Which EU countries exceed the Maastricht debt criteria?"

**🤖 AI Agent:**
> 🏛️ **Maastricht Debt Criteria (60% of GDP)**

Exceeding limit:
🇬🇷 Greece: 161%
🇮🇹 Italy: 137%
🇫🇷 France: 111%
🇪🇸 Spain: 107%
🇧🇪 Belgium: 106%
🇵🇹 Portugal: 99%

13 of 27 members exceed the 60% ceiling.


## ❓ FAQ

**Q: Do I need an API key for Eurostat?**
No! Eurostat is completely open — no registration, no API key, no authentication whatsoever. Just connect and start querying EU data immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eurostat-economy-eu-financial-intelligence](https://vinkius.com/mcp/eurostat-economy-eu-financial-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eurostat Economy — EU Financial Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `eurostat-economy-eu-financial-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eurostat Economy — EU Financial Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eurostat-economy-eu-financial-intelligence": {
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
