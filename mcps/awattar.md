# Awattar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/awattar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Access real-time electricity prices from aWATTar — retrieve EPEX Spot market data and optimized YAML stats for home automation directly from your AI agent.

## Description
Connect to **aWATTar** to monitor electricity market prices and optimize your smart home energy consumption. This server provides direct access to EPEX Spot stock prices and specialized data formats for automation systems.

### What you can do

- **Market Price Tracking** — Fetch real-time and historical EPEX Spot electricity prices to understand market trends and costs.
- **Home Automation Integration** — Get price statistics and hourly thresholds formatted in YAML, specifically designed for LOXONE and other smart home controllers.
- **Smart Scheduling** — Access tomorrow's prices (updated daily at 14:00 CET) to schedule high-consumption appliances during the cheapest hours.
- **Data Analysis** — Retrieve market data for specific time intervals using epoch timestamps for precise energy reporting.

### How it works

1. Subscribe to this server
2. Configure your access credentials if required by your region
3. Start querying energy data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Smart Home Enthusiasts** — feed real-time price data into Loxone or Home Assistant to automatically save on energy bills.
- **Sustainability Advocates** — shift energy usage to times when renewable production is high and prices are low.
- **IoT Developers** — build energy-aware applications using clean, structured market data directly in your development workflow.


## Available Tools
- **get_current_yaml**: Get current aWATTar price statistics in YAML format
- **get_market_data**: Prices for the next day are typically updated daily at 14:00 (CET/CEST).

Get aWATTar market data (electricity prices)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Awattar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current electricity market data from aWATTar."

**🤖 AI Agent:**
> I've retrieved the latest EPEX Spot prices. The current price is 12.4 cents/kWh, with a peak of 15.2 cents at 19:00 and a low of 8.1 cents at 03:00. Would you like to see the full hourly breakdown?

---

**👤 You:**
> "Show me the YAML price statistics for Loxone, including tomorrow's data."

**🤖 AI Agent:**
> I've generated the YAML configuration for your Loxone system. It includes the hourly thresholds for today and tomorrow. Tomorrow's average price is slightly lower at 10.8 cents/kWh. You can copy this YAML directly into your automation logic.

---

**👤 You:**
> "What are the energy prices for the next 24 hours?"

**🤖 AI Agent:**
> Fetching market data for the next 24-hour window... I found that prices will drop significantly between 01:00 and 05:00 AM. This would be the best time to run high-energy appliances. Would you like the specific price for each hour?


## ❓ FAQ

**Q: When are the electricity prices for the next day available?**
Prices for the next day are typically updated daily at 14:00 (CET/CEST). You can use the `get_market_data` tool or `get_current_yaml` with the tomorrow parameter set to true to retrieve them.

**Q: Can I get data specifically formatted for Loxone home automation?**
Yes! Use the `get_current_yaml` tool. It returns price statistics and hourly thresholds optimized for LOXONE Home Automation systems in a ready-to-use YAML format.

**Q: What time format should I use for start and end parameters?**
The `get_market_data` tool expects time parameters in Epoch milliseconds. For example, 1704067200000 represents January 1st, 2024.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/awattar](https://vinkius.com/mcp/awattar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Awattar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `awattar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Awattar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "awattar": {
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
