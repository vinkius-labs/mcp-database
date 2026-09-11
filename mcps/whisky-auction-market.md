# Whisky Auction Market MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/whisky-auction-market)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

The whisky collectibles market as an MCP: real auction data for 160 distilleries (Macallan, Ardbeg, Yamazaki) — monthly bid min/mean/max, trading volumes, price spikes and global market overview. Keyless.

## Description
**Whisky as an asset class, finally queryable** — real auction market data aggregated from the world's whisky auction houses, as a single MCP server.

### What you can do
- **160 distilleries tracked** — Macallan, Ardbeg, Springbank, Yamazaki, Nikka, Buffalo Trace: 119 Scottish, 15 American, 13 Japanese, 5 Irish
- **Monthly price history** — winning bids min/mean/max, trading volume and lot counts per distillery, month by month (Aberfeldy alone: 222 months of data)
- **Price-spike hunting** — the biggest month-over-month jumps and drops in any distillery's history: investment signals, not vibes
- **Side-by-side comparisons** — "Macallan vs Ardbeg vs Yamazaki: which appreciates faster?" answered with all-time averages and latest month
- **Macro view** — the global market: total volume and lots across every auction house, month by month; plus where rare bottles actually trade (house rankings)

### Why it matters
Rare whisky quietly became one of the strongest collectible assets of the last decade — the Knight Frank Luxury Investment Index repeatedly ranked it top-3. But its market data lives scattered across auction houses. This MCP consolidates it for analysis.

### Who is this for?
Collectors and investors, distillery analysts, financial-content creators, sommeliers, and AI agents that need real market numbers instead of "it depends".


## Available Tools (6)
- **get_distillery_price_history**: Use slugs from list_distilleries (e.g. "macallan", "ardbeg", "yamazaki").

Get the full auction price history of one distillery (monthly bids, volume, lots)
- **list_distilleries**: Filter by country or name part. 119 Scottish, 15 American, 13 Japanese, 5 Irish.

List all 160 whisky distilleries tracked by auction data (Scotland, Japan, US...)
- **compare_distilleries**: Slugs from list_distilleries.

Compare auction performance of up to 6 distilleries side by side (latest month + all-time averages)
- **get_market_overview**: 2157+ auction-month rows.

Get the globalThis whisky auction market overview (all auctions aggregated per month)
- **get_auction_houses**: auction, Bonhams, JustWhisky...) with months recorded, mean bid and total volume — useful to know where rare bottles actually trade.

List every whisky auction house tracked, with activity stats
- **find_price_spikes**: Find the biggest price spikes and drops in a distillery's auction history


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Whisky Auction Market** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How has Macallan traded at auction recently?"

**🤖 AI Agent:**
> 🥃 **Macallan auction history**

Months recorded: 200+ (2010 → 2024)
Latest month: winning bids from 45 GBP min to 5,800 GBP max, mean 612 GBP
Trend: post-2022 correction cooling speculative lots, but older vintages still climbing.

Want the spike analysis — the months when Macallan jumped hardest?

---

**👤 You:**
> "Macallan vs Ardbeg vs Yamazaki — which is the better investment?"

**🤖 AI Agent:**
> 📈 **Distillery comparison (all-time auction data)**

- **Macallan**: highest mean bid, biggest total volume — the blue-chip
- **Ardbeg**: strong volume, more accessible lots — liquidity play
- **Yamazaki**: fewer lots but explosive spikes — the Japanese collectible premium

Verdict: Macallan for stability, Yamazaki for volatility with upside. Want the spike history for each?

---

**👤 You:**
> "When did Japanese whisky prices spike the most?"

**🤖 AI Agent:**
> 🔺 **Japanese whisky price spikes (Yamazaki/Nikka/Hakushu)**

Biggest jumps: 2015-2017 — the Suntory discontinuation era. Yamazaki 12 saw +40-80% month-over-month moves as age-statement bottles vanished from shelves.

Run find_price_spikes on yamazaki or nikka for the exact months. I can also pull the global market volume to see how the correction played out.


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. The WhiskyHunter API is fully public — distillery catalog, price histories and auction statistics all work without authentication.

**Q: Where does the data come from?**
WhiskyHunter aggregates real results from multiple whisky auction houses (Scotch Whisky Auctions, Whisky.auction, Bonhams and others). All prices are in GBP as recorded at auction, monthly-aggregated per distillery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/whisky-auction-market](https://vinkius.com/en/ai-agent-connect/whisky-auction-market)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Whisky Auction Market** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `whisky-auction-market` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Whisky Auction Market** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "whisky-auction-market": {
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
