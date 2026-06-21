# Adrecord MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adrecord)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Affiliate marketing network — manage programs, track transactions, and audit earnings via AI.

## Description
Connect your **Adrecord (powered by Adtraction)** affiliate account to your AI agent to unlock professional performance marketing management. From auditing advertiser programs to tracking real-time sales and managing your media channels, your agent handles your affiliate ecosystem through natural conversation.

### What you can do

- **Program Management** — List and retrieve details for available advertiser programs, including commission rates and rules
- **Transaction Auditing** — Retrieve detailed logs of sales and leads to monitor your marketing performance and ROI
- **Channel Oversight** — List and manage your registered media channels (websites, social media) across the network
- **Product Feed Access** — Retrieve and audit product data from advertisers to power your affiliate content
- **Performance Insights** — Quickly identify top-performing programs and track your pending earnings directly from chat

### How it works

1. Subscribe to this server
2. Enter your Adrecord/Adtraction API Token
3. Start managing your affiliate marketing and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Affiliate Marketers** — automate program audits and transaction tracking effortlessly
- **Content Publishers** — quickly retrieve product feeds and check program commission structures
- **Marketing Operations** — monitor account health and sync affiliate data with internal BI tools
- **Growth Hackers** — identify high-payout programs and track campaign conversions using simple commands


## Available Tools
- **list_programs**: List advertiser programs
- **get_program_details**: Get program metadata
- **list_transactions**: Filterable by status.

List sales and leads
- **list_channels**: List media channels
- **get_product_feed**: Fetch advertiser product data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adrecord** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active advertiser programs I am partnered with."

**🤖 AI Agent:**
> I've retrieved your partnered programs. You are currently active in 15 programs, including 'Sport Gear Store', 'Fashion Hub', and 'Travel Deals'. Would you like to check the commission rates for any of them?

---

**👤 You:**
> "Show me all transactions from the last 30 days."

**🤖 AI Agent:**
> I've retrieved your transactions for the last 30 days. You had 120 tracked events resulting in $450 in approved commissions and $150 still pending. Would you like a breakdown by media channel?

---

**👤 You:**
> "Retrieve the product feed for program ID 5678."

**🤖 AI Agent:**
> I've pulled the product feed for program 5678. It contains 250 items including names, prices, and your affiliate tracking links. Would you like to filter for a specific product category?


## ❓ FAQ

**Q: Where do I find my Adrecord API Token?**
Log in to your account (Adrecord or Adtraction), navigate to **Account** > **Settings**. You can generate or retrieve your API Token there. It will be used in the `X-Token` header for all requests.

**Q: Can I see my pending commissions?**
Yes! Use the `list_transactions` tool to retrieve all tracked sales and leads, including their current status (Pending, Approved, Denied) and commission amounts.

**Q: Does this server support product feeds?**
Yes, you can use the `get_product_feed` tool to retrieve structured product data from advertisers you are partnered with.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adrecord](https://vinkius.com/mcp/adrecord)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adrecord** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `adrecord` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adrecord** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adrecord": {
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
