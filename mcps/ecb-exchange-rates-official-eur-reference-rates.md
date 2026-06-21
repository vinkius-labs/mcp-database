# ECB Exchange Rates — Official EUR Reference Rates MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecb-exchange-rates-official-eur-reference-rates)
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


## ❓ FAQ

**Q: When are ECB rates published?**
ECB reference rates are published every business day at approximately 16:00 CET. They are not published on TARGET closing days (weekends and certain holidays).

**Q: Do I need an API key to access the ECB exchange rates?**
No. The ECB provides its reference exchange rates as a completely free and open public good, requiring no authentication or API keys for retrieval.

**Q: Can I query historical data and past performance?**
Yes, you can pull complete structural snapshots covering specific chronological windows daily, monthly, or annually scaling back efficiently using the respective historical endpoints provided.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecb-exchange-rates-official-eur-reference-rates](https://vinkius.com/mcp/ecb-exchange-rates-official-eur-reference-rates)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ECB Exchange Rates — Official EUR Reference Rates** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ecb-exchange-rates-official-eur-reference-rates` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ECB Exchange Rates — Official EUR Reference Rates** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ecb-exchange-rates-official-eur-reference-rates": {
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
