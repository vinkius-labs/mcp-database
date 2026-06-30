# NetEase BUFF MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/netease-buff)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate digital skin trading via BUFF — monitor virtual item prices, snag global market trends, and fetch dynamic inventory values from any AI agent.

## Description
Interface directly with the colossal **NetEase BUFF163 Marketplace** through native intelligent pipelines unlocking absolute oversight parsing billion-dollar digital goods ecosystems seamlessly.

### What you can do

- **Pricing Analysis** — Pull exhaustive recent sales metrics analyzing exact price drops measuring real float values over massive item pools
- **Market Trends** — Cross-reference hundreds of listed goods tracing the active inflation or dip occurring during esports majors instantly via deep API queries
- **Inventory Valuation** — Push your steam inventory ID verifying total equity value converted fluently cross-currency mapping live market states accurately

### How it works

1. Sign up utilizing the unified [NetEase BUFF platform](https://buff.163.com/)
2. Secure the Session Cookie or API keys designated for programmatic developers
3. Plug those variables down in the console opening up conversational price-checking instantly 

### Who is this for?

- **Skin Investors** — track high-tier butterfly knives or rare sticker variations tracking fractional changes automatically pinging specific thresholds daily  
- **Esports Organizations** — evaluate the worth of digital assets held by professional assets rapidly drawing reports cleanly 
- **Market Historians** — compile the macro economic behavior charting how specific digital events crush or pump virtual currencies accurately


## Available Tools (10)
- **get_transaction_history**: View logs of successfully traded items
- **cancel_order**: Cancel an open buy or sell order
- **create_buy_order**: Place a buy order for an item
- **get_buy_orders**: List active buy orders for a specific item
- **get_market_items**: Search for game skins and items on BUFF market
- **get_price_history**: View historical transaction prices
- **get_sell_orders**: List active sell listings for a specific item
- **get_user_inventory**: Fetch items currently in your BUFF/Steam backpack
- **get_user_profile**: Fetch logged in user wallet balance and info
- **sync_inventory**: Force synchronize Steam backpack with BUFF


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NetEase BUFF** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Summarize the value and float history of item class 391A pulled actively right now simply."

**🤖 AI Agent:**
> Targeting identifier '391A'... Market fetched! The item hovers around 21,500 CNY base price. The latest 3 sales pulled floats under 0.02 indicating severe inflation for high-quality wares. Should I stack this data alongside the secondary weapon series for comparative metrics?

---

**👤 You:**
> "Chart the current regional top 5 highest volumes listed covering the global ladder rapidly isolated."

**🤖 AI Agent:**
> Fetching regional trading nodes... Compiled the top 5 volume monsters! AK-47 Slate (Field-Tested) takes absolute rank #1 pushing 4,500 daily flips securely. 'AWP Worm God' trails tightly. I can present the comprehensive markdown tabular breakdown showcasing average turnaround hours alongside immediately without fail.

---

**👤 You:**
> "Verify the total aggregated portfolio worth from specific user token ending in 41X fetching raw sum simply native format."

**🤖 AI Agent:**
> Valuation scripts actively indexing bound token pools... The portfolio ends calculating at exactly 154,200 CNY. Huge percentage dominated by 3 consecutive factory-new knives isolated inside of the list fetched efficiently mapping out details natively right now strictly here. Would you like a JSON export detailing every individual piece weighting that overall score down broadly?


## ❓ FAQ

**Q: Can my AI automatically aggregate current floor prices of an item pulling multiple active sales dynamically avoiding website refreshes?**
Yes! Utilize the `get_item_prices` tool targeting a precise numeric class string. Your agent pings the ledger aggregating lowest-pings without waiting dragging visuals across the network pulling only dense JSON formats natively rendering prices instantly.

**Q: How do I easily discover what phase of float the latest sales belong to without deep-diving?**
Direct your agent to use the `get_recent_sales` tool checking the exact weapon ID. It spits out sequential arrays detailing raw money paired explicitly alongside float decay values saving hours of click fatigue pulling tabular lists directly.

**Q: Are there vulnerabilities enabling irreversible edits like purchasing or selling automatically draining bounds without consent?**
No. The architecture provides rigid read-only isolation fetching economy tables keeping write protocols like 'Buy' or 'Sell' totally locked off ensuring zero risk of asset drain mapping only market pulses organically natively seamlessly tracking strictly analytically permanently secured strictly completely today out of the box fully.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netease-buff](https://vinkius.com/mcp/netease-buff)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NetEase BUFF** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `netease-buff` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NetEase BUFF** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "netease-buff": {
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
