# Alpha Vantage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alpha-vantage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access stock market data via Alpha Vantage — get real-time quotes, time series, technical indicators and crypto/forex data from any AI agent.

## Description
Connect to **Alpha Vantage** APIs through any AI agent and explore global financial markets through natural conversation.

### What you can do

- **Real-Time Quotes** — Get current stock prices, volume, high/low, open and previous close
- **Time Series** — Access daily, weekly, monthly and intraday OHLCV data with 20+ years of history
- **Technical Indicators** — Calculate RSI, SMA, EMA, MACD, Bollinger Bands and 50+ other indicators
- **Company Fundamentals** — Retrieve company overview, market cap, PE ratio, EPS and earnings history
- **Sector Performance** — Monitor real-time performance of all 11 market sectors
- **News Sentiment** — Fetch news articles with sentiment scores for stock tickers
- **Crypto & Forex** — Get daily cryptocurrency and foreign exchange rate data

### How it works

1. Subscribe to this server
2. Enter your Alpha Vantage API Key (free at alphavantage.co)
3. Start exploring financial markets from Claude, Cursor, or any MCP-compatible client

No more navigating complex financial terminals to check stock prices or technical indicators. Your AI acts as a dedicated market data analyst.

### Who is this for?

- **Traders** — quickly check quotes, review time series and calculate technical indicators without opening a trading platform
- **Investors** — explore company fundamentals, earnings history and sector performance for portfolio research
- **Developers** — access market data programmatically for building financial applications and analysis tools
- **Students** — learn about technical analysis, market trends and financial data through interactive conversation


## Available Tools
- **get_company_overview**: Useful for fundamental analysis and stock screening.

Get company overview and fundamentals
- **get_crypto_daily**: Requires the crypto symbol (e.g. "BTC") and the market currency (e.g. "USD"). Returns daily price data with dates.

Get daily cryptocurrency prices
- **get_daily_time_series**: Optionally set outputsize to "compact" (last 100 data points, default) or "full" (20+ years of data). Returns daily price data with dates.

Get daily stock time series
- **get_earnings**: Useful for earnings analysis and identifying beats/misses.

Get earnings history for a stock
- **get_forex_daily**: Requires the from symbol (e.g. "EUR") and to symbol (e.g. "USD"). Returns daily OHLCV forex data with dates.

Get daily foreign exchange rates
- **get_intraday_time_series**: Optionally set interval (1min, 5min, 15min, 30min, 60min) and outputsize. Returns price data at the specified interval. Useful for day trading analysis.

Get intraday stock time series
- **get_monthly_time_series**: Each data point represents a month of trading. Useful for long-term trend analysis and portfolio review.

Get monthly stock time series
- **get_news_sentiment**: Each article includes title, summary, source, sentiment scores (bullish/bearish score) and relevance score. Optionally filter by topics and limit the number of results.

Get news sentiment for stock tickers
- **get_quote**: Returns current trading data including change and change percent. Useful for quick price checks.

Get real-time stock quote
- **get_rsi**: RSI measures momentum on a 0-100 scale; above 70 indicates overbought, below 30 indicates oversold. Optionally set interval, time period and series type (close, open, high, low).

Get Relative Strength Index (RSI) indicator
- **get_sector_performance**: Returns change percentages for each sector.

Get real-time sector performance
- **get_weekly_time_series**: Each data point represents a week of trading. Useful for medium-term trend analysis.

Get weekly stock time series
- **search_symbol**: Returns best matches with symbol, name, type and region. Useful for discovering the correct symbol before querying price data.

Search for stock symbols by keywords


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alpha Vantage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current quote for Apple stock."

**🤖 AI Agent:**
> AAPL is currently trading at $189.45, up 1.23 (0.65%) from yesterday's close. Today's range: $187.80 - $190.12. Volume: 52.3M shares.

---

**👤 You:**
> "Show me the RSI for Tesla over the last 14 days."

**🤖 AI Agent:**
> TSLA's current RSI (14-day) is 68.5, approaching the overbought threshold of 70. The RSI has been trending up from 52 three weeks ago, indicating strengthening momentum.

---

**👤 You:**
> "What are the top performing sectors today?"

**🤖 AI Agent:**
> Today's sector performance: Technology (+2.1%), Healthcare (+1.5%), Financials (+1.2%), Energy (-0.3%), Utilities (-0.8%). Technology is leading with strong gains across semiconductor and software stocks.


## ❓ FAQ

**Q: How do I get an Alpha Vantage API key?**
Visit [**alphavantage.co/support/#api_key**](https://www.alphavantage.co/support/#api_key), fill in your name and email, and click **GET FREE API KEY**. The key is delivered instantly on the page. Free tier includes 25 requests per day.

**Q: What technical indicators are available?**
Alpha Vantage supports 50+ technical indicators including SMA, EMA, RSI, MACD, Bollinger Bands, Stochastic, ADX, ATR, CCI, Williams %R, and many more. Currently this MCP server exposes RSI, with more indicators available on request.

**Q: Can I get cryptocurrency data?**
Yes! Use `get_crypto_daily` with the crypto symbol (e.g. 'BTC', 'ETH', 'SOL') and market currency (e.g. 'USD', 'EUR'). Returns daily OHLCV data for the cryptocurrency pair.

**Q: How much historical data is available?**
Alpha Vantage provides 20+ years of historical data for most stocks. Use the `get_daily_time_series` tool with outputsize 'full' to access the complete history. The compact mode returns the last 100 data points.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alpha-vantage](https://vinkius.com/mcp/alpha-vantage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alpha Vantage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `alpha-vantage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alpha Vantage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alpha-vantage": {
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
