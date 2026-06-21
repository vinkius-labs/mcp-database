# Juhe Data / 聚合数据 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/juhe-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

China's leading API aggregator — access weather, ID verification, IP lookup, and news via AI.

## Description
Empower your AI agent to access a vast array of essential data services with **Juhe Data** (聚合数据), the premier API aggregator in China. By connecting Juhe to your agent, you transform fragmented data retrieval into a natural conversation. Your agent can instantly check real-time weather and forecasts for any Chinese city, verify ID card registration details, lookup IP address locations, and retrieve the latest news across multiple categories. Whether you are automating background checks, monitoring local conditions, or staying updated with domestic trends, your agent acts as a real-time data intelligence assistant, providing accurate and reliable information from a single, unified source.

### What you can do

- **Weather Intelligence** — Retrieve real-time weather and 3-day forecasts for cities across China.
- **Identity Verification** — Audit ID card numbers to retrieve area, sex, and birthday information.
- **Geographical Insights** — Lookup IP address locations to identify user regions and network providers.
- **Content Aggregation** — Retrieve the latest news headlines and articles across various categories.
- **Calendar & Culture** — Access lunar calendar data, holiday schedules, and even constellation horoscopes.

### How it works

1. Subscribe to this server
2. Enter your Juhe AppKeys for the services you wish to use (Weather, ID, News, etc.)
3. Start querying essential data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Teams** — monitor regional conditions and coordinate logistics based on accurate local data.
- **Compliance Officers** — automate basic identity verification and background auditing through natural language.
- **Research Analysts** — gather real-time data on news trends, currency rates, and market indicators.
- **Developers** — integrate a massive library of utility APIs into your AI-driven daily routines.


## Available Tools
- **get_calendar_day**: Get calendar and holiday info for a day
- **get_calendar_month**: Get holiday info for a month
- **get_constellation_horoscope**: Get constellation horoscope
- **get_driving_test_questions**: Get random driving test questions
- **get_exchange_rate**: Get currency exchange rate
- **get_id_card_info**: Get ID card basic information
- **get_ip_lookup**: Lookup IP address location
- **get_latest_news**: Get latest news headlines
- **get_oil_price**: Get latest oil prices in China
- **get_weather**: Get weather information for a city


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Juhe Data / 聚合数据** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather in Beijing today?"

**🤖 AI Agent:**
> In Beijing, it's currently Sunny at 22°C with 35% humidity. The wind is blowing from the North at level 2. The forecast for the next 3 days remains clear with temperatures ranging between 12°C and 25°C.

---

**👤 You:**
> "Check the information for ID card 110101199001011234."

**🤖 AI Agent:**
> The ID card information shows the holder is a Male, born on January 1, 1990. The registration area is Dongcheng District, Beijing.

---

**👤 You:**
> "Show me the latest tech news from Juhe."

**🤖 AI Agent:**
> I've retrieved the latest tech news. Headlines include 'New Advances in AI Chips' and 'The Growth of China's Digital Economy'. Would you like the links to the full articles?


## ❓ FAQ

**Q: How do I get my Juhe AppKey?**
Log in to the [Juhe Data](https://www.juhe.cn/) website, browse the API store, apply for the services you need (e.g., Weather, ID Card), and you will find the corresponding AppKey in your personal center under 'My APIs'.

**Q: Can I use one key for all tools?**
Usually, Juhe Data assigns separate AppKeys for different API services. Ensure you provide the correct key for each service (Weather, ID Card, News, etc.) in the credentials section of this server.

**Q: Is this data only for mainland China?**
Most Juhe services focus on mainland China (Weather, ID Card, Oil Prices). However, some services like IP Lookup and Exchange Rates provide global information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/juhe-data](https://vinkius.com/mcp/juhe-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Juhe Data / 聚合数据** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `juhe-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Juhe Data / 聚合数据** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "juhe-data": {
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
