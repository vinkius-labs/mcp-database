# ECB Full — Complete Eurozone Financial Intelligence MCP Server

The definitive ECB Mega-Server: 14 tools for EUR exchange rates against 40+ currencies, key interest rates (MRO, DFR, MLFR), MFI bank rates, monetary aggregates (M1/M2/M3), government bond yield curves, euro banknotes, and a universal SDMX query engine for all ECB statistical data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ecb-full-complete-eurozone-financial-intelligence)

## Overview
**Category:** the-unthinkable
**Tools Count:** 14

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


## Installation & Usage

To install and use the **ECB Full — Complete Eurozone Financial Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecb-full-complete-eurozone-financial-intelligence](https://vinkius.com/mcp/ecb-full-complete-eurozone-financial-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
