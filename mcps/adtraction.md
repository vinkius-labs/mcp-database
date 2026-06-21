# Adtraction MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adtraction)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Affiliate marketing network — manage programs, track transactions, and audit performance via AI.

## Description
Connect your **Adtraction** affiliate account to your AI agent to unlock professional performance marketing management. From auditing advertiser programs across multiple categories to tracking real-time transactions and managing your product feeds, your agent handles your affiliate operations through natural conversation.

### What you can do

- **Program Management** — List and retrieve details for available advertiser programs, including commission structures and categories
- **Transaction Auditing** — Retrieve detailed logs of sales and leads to monitor your marketing performance and earnings status
- **Real-time Statistics** — Retrieve performance data broken down by day or by advertiser program directly from chat
- **Product Feed Access** — List and retrieve metadata for advertiser product feeds to support your affiliate content strategy
- **Channel Oversight** — List and manage your approved marketing channels (websites, social media) within the network

### How it works

1. Subscribe to this server
2. Enter your Adtraction API Token
3. Start managing your affiliate partnerships and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Affiliate Marketers** — automate program audits and transaction tracking across multiple advertisers
- **Content Publishers** — quickly retrieve product feeds and check commission rates for targeted brands
- **Growth Specialists** — monitor daily performance trends and identify high-payout opportunities
- **Marketing Operations** — audit channel statuses and sync transaction data with internal reporting tools


## Available Tools (5)
- **list_programs**: List affiliate programs
- **get_program_details**: Get program metadata
- **list_transactions**: List affiliate transactions
- **get_stats_by_program**: Get performance stats per program
- **list_channels**: List approved media channels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adtraction** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all advertiser programs in the 'Fashion' category."

**🤖 AI Agent:**
> I've retrieved the advertiser programs for the Fashion category. You have 10 available programs, including 'Luxury Apparel', 'Daily Wear', and 'Street Style Shop'. Would you like to see the commission structure for any of them?

---

**👤 You:**
> "Show me my performance stats for today."

**🤖 AI Agent:**
> I've pulled your performance stats for today. So far, you have 500 clicks, 12 sales, and $85.50 in pending commissions. Your conversion rate is currently 2.4%.

---

**👤 You:**
> "Retrieve the latest 5 approved transactions."

**🤖 AI Agent:**
> I've retrieved your latest 5 approved transactions. They come from programs like 'Tech Store' and 'Travel Booking', totaling $120 in commissions. Would you like to see the breakdown by date?


## ❓ FAQ

**Q: Where do I find my Adtraction API Token?**
Log in to your Adtraction account, navigate to **Account** > **Settings** > **API**. You can generate or retrieve your unique token there. It will be used in the `X-Token` header.

**Q: Can I see my earnings by advertiser?**
Yes! Use the `get_stats_by_program` tool. Your agent will retrieve aggregated statistics for each advertiser you are partnered with, including commissions and conversion rates.

**Q: Does this support transaction status tracking?**
Yes, the `list_transactions` tool provides the current status (Pending, Approved, Denied) for every sale or lead tracked in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adtraction](https://vinkius.com/mcp/adtraction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adtraction** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adtraction` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adtraction** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adtraction": {
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
