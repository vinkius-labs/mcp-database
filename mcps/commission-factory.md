# Commission Factory MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/commission-factory)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Commission Factory is a leading affiliate marketing network in Asia-Pacific. This MCP server allows affiliates and merchants to retrieve transactions, manage programs, and track performance programmatically.

## Description
Connect your **Commission Factory** account to any AI agent and manage your affiliate marketing programs through natural conversation.

### What you can do

- **Transaction Retrieval** — List your recent affiliate transactions, access detailed reports, and monitor clicks or conversions.
- **Program Management** — Find details about merchants you have joined and check their status.
- **Promotional Tools** — Retrieve active coupons, promotional codes, and creative banners from your partnered merchants.
- **Performance Tracking** — Calculate your commissions, track generated sales value, and summarize performance data.

### How it works

1. Subscribe to this server
2. Enter your Commission Factory API Key
3. Start managing your affiliate marketing through Claude, Cursor, or any MCP-compatible client

Your AI agent becomes your growth partner, giving you instant access to affiliate data without navigating through complex dashboards.

### Who is this for?

- **Affiliate Marketers** — track conversions and discover new coupons via quick chat commands.
- **Content Creators** — instantly generate affiliate links for products or retrieve active promotional campaigns.
- **Merchants** — programmatically monitor affiliate performance and validate tracked transactions.


## Available Tools
- **get_merchant_details**: Retrieve detailed information about a specific merchant
- **get_performance_summary**: Calculate basic commission and sale totals for a set of transactions
- **get_transaction_details**: Retrieve details of a specific transaction
- **list_affiliate_merchants**: Retrieve a list of merchants available in the Commission Factory network
- **list_affiliate_transactions**: Retrieve a list of transactions for your affiliate account
- **list_merchant_affiliates**: Retrieve a list of affiliates joined to your merchant program
- **list_merchant_transactions**: Retrieve transactions generated for your merchant campaign
- **list_promotions**: Retrieve active coupon codes and promotions from joined merchants


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Commission Factory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 20 affiliate transactions in Commission Factory."

**🤖 AI Agent:**
> I've fetched your last 20 transactions. You have 5 approved transactions and 15 pending ones. The total commission value is $240.20. Would you like a breakdown by merchant?

---

**👤 You:**
> "List all active promotions and coupon codes from my joined merchants in Commission Factory."

**🤖 AI Agent:**
> Here are the active coupons from your merchants: 1. '10% Off Shoes' at TrendyFootwear (Code: TF10), 2. 'Free Shipping' at GadgetStore (Code: FREESHIP). Do you need the affiliate links for any of these?

---

**👤 You:**
> "Calculate my total commission and sales value for the current month in Commission Factory."

**🤖 AI Agent:**
> For the current month, your total generated sales value is $4,250.00, resulting in a total commission of $450.75 across 32 conversions.


## ❓ FAQ

**Q: How do I get my Commission Factory API key?**
You can generate an API key in your Commission Factory dashboard under Profile and Preferences > Apps and API keys.

**Q: Is this for affiliates or merchants?**
This MCP server supports tools for both Affiliates and Merchants. Your API key determines the data you can access.

**Q: What is the UniqueId in transactions?**
The UniqueId (often called SubID or ClickID) is a custom value you passed during the initial click to track specific sources or campaigns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commission-factory](https://vinkius.com/mcp/commission-factory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Commission Factory** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `commission-factory` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Commission Factory** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "commission-factory": {
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
