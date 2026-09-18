# China Financial Markets MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/china-financial-markets)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Keyless live data for China's A-share, HK and CNY markets — quotes, candle history, index breadth and FX, no API key.

## Description
Give your AI agent **live, keyless access to the Chinese financial markets** — the world's second-largest stock market plus its offshore yuan and benchmark indices — with no API key and no setup.

### What you can do

- **Look up any symbol** — `search_china_stock` resolves a company name, pinyin, code or FX pair to the right market-prefixed symbol (SSE / SZSE / BSE / HKEX) so quoting always hits the right exchange
- **Quote anything China-related** — `get_stock_quote` returns live price, change, P/E, P/B, market cap, turnover, limit-up/down and timestamp for A-shares, HK stocks, China ETFs, China futures and FX pairs, one batched call for many symbols
- **Read the candle history** — `get_kline` gives OHLCV bars (daily / weekly / monthly, forward- or back-adjusted) with automatic provider failover so you always get a series
- **Get the market headline in one call** — `get_index_snapshot` returns SSE Composite, SSE 50, CSI 300, CSI 500, SZSE Component, ChiNext and the Hang Seng Index together
- **Track the yuan** — `get_cny_rate` returns CNY crosses (default USDCNY + USDHKD) with the intraday move
- **See the day's momentum** — `get_top_movers` lists the biggest same-day A-share gainers or losers (the one tool that is region-throttled, and it degrades gracefully instead of failing)

### Why this is different

Most of the catalog's China coverage is dev-tooling (Baidu Cloud, Tencent Cloud SDKs) or marketing calculators. There is **no China market-data connector**: no way to ask an agent "how is CSI 300 doing, what's Moutai at, and where's the yuan?" This fills that gap with a deliberately keyless stack — the quotes, history, index snapshot and FX layers are served by endpoints that work globally without credentials, so the connector keeps working from any network.

### How it works

1. Add this server to your agent — no credentials, nothing to configure
2. Ask: "compare Moutai and BYD on CSI 300, and give me the yuan" and the agent composes `get_index_snapshot`, `get_stock_quote` and `get_cny_rate` automatically

### Who is this for?

- **International traders and portfolio managers** — a China market view with no key, no regional lock-in and a consistent field model across stocks, ETFs, futures and FX
- **Analysts and quants** — adjusted candle history and benchmark breadth as clean, typed rows you can feed straight into a backtest or a research note
- **FX and macro desks** — onshore yuan crosses with the intraday delta, alongside the headline China index moves


## Available Tools (6)
- **get_kline**: Default is forward-adjusted daily (dividends/splits smoothed). `period` accepts day, week or month; `adjust` accepts qfq (forward, default), hfq (back) or raw. Bounded by `limit` bars (1-250, default 60). Works for A-shares (sh/sz prefix) and ETFs; HK history is best-effort. If the primary history source is unreachable the tool automatically retries against a secondary provider and labels the `source` of whatever it returns. For a live snapshot instead, use get_stock_quote.

OHLCV candle history (daily / weekly / monthly, forward- or back-adjusted) for a China security
- **get_stock_quote**: Accepts one or many comma-separated codes; bare numbers are auto-routed to the right exchange (6xxxxx→SSE, 0/3xxxxx→SZSE, 8/4xxxxx→BSE, 4-5 digits→HK, USDCNY→FX). A-share prices are in CNY; HK in HKD; FX pairs in their quote currency. When a code is unknown or the market is closed you get back fewer rows than requested — diff against `requested` to spot misses. For a benchmark-breadth view use get_index_snapshot; for history use get_kline.

Live quotes for A-shares, HK stocks, China ETFs, China futures, FX pairs and indices in one call
- **get_top_movers**: `direction` is up (default) or down. This surface is the most region-sensitive in the connector: from many non-mainland networks the breadth service is throttled or unreachable, in which case the response sets `available=false` and points you to get_index_snapshot as the market-level fallback rather than failing. Use it to pick the names worth drilling into with get_stock_quote + get_kline.

Biggest same-day gainers or losers on the Shanghai + Shenzhen A-share markets
- **get_cny_rate**: Default pairs are USDCNY and USDHKD; request any CNY cross with `pairs` (comma-separated, e.g. "USDCNY,USDCNH,EURCNY"). Rates are the last-quoted value, not a mid-term average — treat as indicative. A pair that is not quotable is simply omitted, so diff the requested list against what comes back. For USD-based multi-currency conversion beyond CNY, prefer a dedicated FX connector.

CNY cross-rates (onshore CNY) against major currencies, with intraday move and timestamp
- **get_index_snapshot**: Good default for dashboards, daily briefings and the first step of any market-stance question. No parameters. For a specific name or sector, drop to get_stock_quote; for the underlying constituents, use get_kline on an index-tracker ETF.

One-call snapshot of the headline China benchmarks: SSE, CSI 300, CSI 500, ChiNext, SZSE Component and the Hang Seng
- **search_china_stock**: Returns the normalized market code, exchange classification and a ready-to-use quote id. When the symbol search is unreachable from your region, the response says so and tells you to pass a market-prefixed code directly (sh600519, sz300750, hk00700, whUSDCNY) to get_stock_quote instead. Use this first whenever you are not sure of the exact exchange prefix.

Search Chinese stocks, indices and FX by name or code (Pinyin/English names supported)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **China Financial Markets** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How is the Chinese market today? Give me the benchmark indices, Moutai and BYD, and where the yuan is."

**🤖 AI Agent:**
> I called get_index_snapshot, get_stock_quote for sh600519 and sz002594, and get_cny_rate. CSI 300 is at 3,902 (+0.4%), ChiNext +0.9%, Hang Seng +1.1% — a broadly risk-on day. Moutai (sh600519) is at ¥1,258 (−0.6%, P/E 19.1, cap ¥1.576T) and BYD (sz002594) at ¥102.4 (+2.1%). The yuan is USDCNY 7.091 (−0.04% intraday). Want me to pull the last 60 daily bars on either name with get_kline?

---

**👤 You:**
> "Is the China tech basket beating the broad market this week? Show me CSI 300 vs ChiNext and the daily closes for the last two weeks."

**🤖 AI Agent:**
> get_index_snapshot shows ChiNext at +3.2% on the week vs CSI 300 at +0.7% — tech is clearly leading. I pulled get_kline for sh000300 and sz399006 (day, qfq, limit 10) and computed the 10-day change: CSI 300 3,811→3,838 (+0.7 %), ChiNext 2,144→2,213 (+3.2 %). The outperformance is broad-based across the last two sessions. Want the top ChiNext movers with get_top_movers?


## ❓ FAQ

**Q: Do I need an API key?**
No. Every layer — symbol search, live quotes, candle history, index snapshot and CNY rates — is keyless and works from any network. There is nothing to enter or maintain.

**Q: Which markets and instruments are covered?**
Shanghai (SSE) and Shenzhen (SZSE, incl. ChiNext and STAR) A-shares, the Beijing exchange, HKEX-listed stocks, China ETFs, China futures and CNY currency crosses, plus the seven headline China benchmark indices. Pass codes like sh600519, sz300750, hk00700 or whUSDCNY, or a bare number and it is routed automatically.

**Q: Why does get_top_movers sometimes come back with no data?**
Market-breadth (top gainers/losers) is the one surface that gets throttled from many non-mainland networks. When it can't be reached the tool returns available=false with a note and points you to get_index_snapshot as the market-level fallback — it degrades instead of erroring.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/china-financial-markets](https://vinkius.com/en/ai-agent-connect/china-financial-markets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **China Financial Markets** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `china-financial-markets` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **China Financial Markets** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "china-financial-markets": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
