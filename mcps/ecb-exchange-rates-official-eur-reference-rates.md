# ECB Exchange Rates — Official EUR Reference Rates MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecb-exchange-rates-official-eur-reference-rates)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ecb-exchange-rates-official-eur-reference-rates-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ecb-exchange-rates-official-eur-reference-rates-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Official ECB reference exchange rates: EUR against 40+ currencies updated daily at 16:00 CET. Get single pair rates, multi-currency comparisons, and the latest snapshot of all published rates — daily, monthly, or annual frequency.

## Description
Official ECB reference exchange rates.

### What you can do
- **Single Rate** — EUR vs any of 40+ currencies
- **Multi-Currency** — Compare EUR against multiple currencies
- **Latest Snapshot** — All rates at once
- **Historical** — Daily, monthly, or annual series

### No API Key Required
Completely open and unrestricted.


## Available Tools
- **get_exchange_rate**: Daily, monthly, or annual frequency. The ECB publishes reference rates for ~40 currencies against the euro at around 16:00 CET each business day.

Get the EUR exchange rate against a specific currency from the ECB
- **get_multiple_rates**: Separate currency codes with commas. Useful for comparing EUR strength across multiple currencies.

Get EUR exchange rates against multiple currencies simultaneously
- **get_latest_rates**: Published daily at ~16:00 CET. Includes USD, GBP, JPY, CHF, CNY, AUD, CAD, and more.

Get the latest ECB reference exchange rates for all currencies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ECB Exchange Rates — Official EUR Reference Rates** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current EUR/USD exchange rate?"

**🤖 AI Agent:**
> 💱 **EUR/USD Exchange Rate**

Latest: 1 EUR = 1.0842 USD
Date: 2026-04-03

Published by the ECB at 16:00 CET

30-day trend: 1.0780 → 1.0842 (+0.57%)
52-week range: 1.0520 — 1.1280

Source: ECB, dataflow EXR

---

**👤 You:**
> "Compare EUR against GBP, JPY, and CHF"

**🤖 AI Agent:**
> 💱 **EUR vs Major Currencies**

| Currency | Rate | Change (30d) |
|----------|------|-------------|
| GBP | 0.8567 | -0.3% |
| JPY | 163.42 | +1.2% |
| CHF | 0.9721 | +0.1% |

ECB reference rates, 2026-04-03

---

**👤 You:**
> "Retrieve the latest snapshot of all published ECB exchange rates for the Euro."

**🤖 AI Agent:**
> Retrieving complete reference matrix strictly linked centrally...
**Global ECB Snapshot**:
- USD: 1.0842
- GBP: 0.8567
- JPY: 163.42
- CHF: 0.9721
- AUD: 1.6321
- CAD: 1.4533
[... and 34 other currencies].
Data synced directly securely globally.


## Installation & Usage

To install and use the **ECB Exchange Rates — Official EUR Reference Rates** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecb-exchange-rates-official-eur-reference-rates](https://vinkius.com/mcp/ecb-exchange-rates-official-eur-reference-rates)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
