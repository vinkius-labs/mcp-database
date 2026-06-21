# Asian Development Bank MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/asian-development-bank)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access comprehensive macroeconomic indicators for 49 Asia-Pacific economies — GDP, inflation, trade, population, and more — directly from the ADB.

## Description
The **Asian Development Bank MCP Server** connects your AI agent to the official Key Indicators Database (KIDB) maintained by the ADB — the principal multilateral development finance institution for the Asia-Pacific region.

### Core Capabilities

- **GDP & National Accounts** — Track economic output, growth rates, and GDP deflators across China, Japan, India, South Korea, and 45 other economies.
- **Inflation & Consumer Prices** — Monitor CPI-based inflation trends that drive monetary policy in the world's fastest-growing markets.
- **Trade & Balance of Payments** — Analyze import/export volumes and current account balances across the entire ASEAN corridor and beyond.
- **Shortcut Tools** — Dedicated quick-access endpoints for GDP and inflation that require only economy codes and a start year.

Zero authentication required. Covers the full breadth of ADB member economies from Afghanistan to Vanuatu. Essential for macro analysts, fund managers, trade consultants, and policy researchers focused on the Asia-Pacific.


## Available Tools
- **get_gdp_asia**: Economy codes: PRC, JPN, IND, KOR, INO, THA, VIE, PHI.

Get GDP data for Asia-Pacific economies
- **get_inflation_asia**: Economy codes: PRC, JPN, IND, KOR, INO, THA, VIE, PHI.

Get consumer price inflation rates for Asia-Pacific
- **query_adb_indicators**: Dataflow IDs: ADB,EO_NA (GDP), ADB,EO_INF (Inflation), ADB,EO_BOP (Trade). Common indicators: NGDP_XDC (GDP), PCPI_PCH (CPI). Economy codes: PRC, JPN, IND, KOR, INO, PHI, THA, VIE. Use + to combine.

Query macroeconomic indicators from the Asian Development Bank


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Asian Development Bank** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the GDP of China, Japan, and India from 2020 onwards?"

**🤖 AI Agent:**
> I've pulled GDP data from the ADB Key Indicators. China's GDP at current prices stands at approximately 121 trillion yuan (2023), Japan at around 591 trillion yen, and India at roughly 296 trillion rupees. All three show sustained growth since the post-pandemic recovery.

---

**👤 You:**
> "Compare inflation rates between Southeast Asian countries over the last 5 years."

**🤖 AI Agent:**
> I've compared CPI inflation across the ASEAN corridor. Thailand and Malaysia maintained relatively stable rates around 1-3%, while the Philippines and Indonesia experienced higher volatility. Vietnam showed a steady downward trend from its 2022 peak. The data comes directly from the ADB's official statistical database.


## ❓ FAQ

**Q: Do I need an API Key?**
No. The ADB KIDB API is completely open and requires zero authentication. The only limit is 20 queries per minute to maintain service stability.

**Q: What economies are covered?**
The database covers all 49 ADB member economies across the Asia-Pacific region, including China, Japan, India, South Korea, all ASEAN nations, Central Asian republics, and Pacific Island states.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/asian-development-bank](https://vinkius.com/mcp/asian-development-bank)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Asian Development Bank** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `asian-development-bank` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Asian Development Bank** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "asian-development-bank": {
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
