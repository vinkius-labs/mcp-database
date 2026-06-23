# ShowAPI / 易源数据 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/showapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Massive API data marketplace — access weather, translation, stock info, and utilities via AI.

## Description
Empower your AI agent to orchestrate your data retrieval with **ShowAPI** (易源数据), the premier API marketplace in China. By connecting ShowAPI to your agent, you transform complex API consumption into a natural conversation. Your agent can instantly retrieve real-time weather data, lookup IP geographical information, provide daily jokes and inspirational quotes, translate text between languages, and even audit stock market performance and currency rates without you ever needing to write a single line of integration code. Whether you are automating content research, monitoring financial indicators, or stays updated with historical events, your agent acts as a real-time information assistant, providing accurate and reliable data from a massive library of utility services.

### What you can do

- **Information Retrieval** — Access real-time weather, IP lookup, and historical events for any date.
- **Linguistic Support** — Translate text between languages and lookup comprehensive English word definitions and Chinese idioms.
- **Financial Monitoring** — Retrieve real-time stock information and global currency exchange rates.
- **Content Aggregation** — Browse a vast collection of jokes and famous quotes to power your creative workflows.
- **Utility Orchestration** — Leverage a massive library of utility APIs through a single, unified AI interface.

### How it works

1. Subscribe to this server
2. Enter your ShowAPI App ID and App Secret (Sign)
3. Start managing your data orchestration through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — automate research for news, quotes, and jokes through natural language queries.
- **Financial Analysts** — monitor real-time stock data and currency fluctuations directly from your AI-powered workspace.
- **Operations Teams** — coordinate regional activities based on accurate weather and IP geographical metadata.
- **ShowAPI Users** — integrate your existing data marketplace workflows into your AI-driven daily routines.


## Available Tools (10)
- **get_currency_rates**: Get current foreign exchange rates
- **get_english_dictionary**: Lookup English word definitions
- **get_history_today**: Get historical events for today
- **get_idiom_info**: Get Chinese idiom information
- **get_inspirational_quotes**: Get inspirational and famous quotes
- **get_ip_lookup**: Lookup IP address geographical information
- **get_jokes**: Get funny jokes and short stories
- **get_stock_info**: Get stock market information
- **get_weather**: Get weather information for an area
- **translate_text**: Translate text between languages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShowAPI / 易源数据** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Translate 'Hello, how are you?' into Chinese using ShowAPI."

**🤖 AI Agent:**
> I've translated your text. 'Hello, how are you?' in Chinese is '你好，你好吗？'. Would you like me to translate it into any other language?

---

**👤 You:**
> "Show me the latest stock info for 'sh600000'."

**🤖 AI Agent:**
> I've retrieved the stock data for sh600000 (Shanghai Pudong Development Bank). The current price is ¥7.42, with a daily change of +0.54%. Would you like a more detailed breakdown of the technical indicators?

---

**👤 You:**
> "Tell me a random joke from ShowAPI."

**🤖 AI Agent:**
> Here's a joke for you: 'Why don't scientists trust atoms? Because they make up everything!'. Should I find another one or perhaps an inspirational quote?


## ❓ FAQ

**Q: How do I find my ShowAPI App ID and Secret?**
Log in to the [ShowAPI](https://www.showapi.com/) website, go to your Personal Center -> [Secret Management], and you will find your `showapi_appid` and `showapi_sign` there.

**Q: Does this support all 1000+ APIs from ShowAPI?**
This server provides 10 essential tools covering the most popular categories like weather, finance, and translation. For other specific APIs, you can extend the engine or use the marketplace directly.

**Q: Are there usage limits for these tools?**
The usage limits and quotas depend on your ShowAPI subscription plan. Ensure your account has sufficient balance or points for the API points you are calling.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/showapi](https://vinkius.com/mcp/showapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ShowAPI / 易源数据** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `showapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ShowAPI / 易源数据** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "showapi": {
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
