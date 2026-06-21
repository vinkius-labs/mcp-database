# Appfigures MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appfigures)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Analyze app store performance with Appfigures — track downloads, revenue, reviews, and rankings via AI.

## Description
The **Appfigures MCP Server** provides your AI agent with direct access to your mobile app intelligence and store data. Gain instant insights into your app's performance across iOS, Google Play, and other major stores using simple natural language.

### Key Features

- **Product Management** — List and search for your apps and those of your competitors across all major app stores.
- **Sales & Revenue Reporting** — Get detailed reports on downloads, updates, returns, and net proceeds.
- **Subscription Analytics** — Monitor your subscription health, churn, and active subscriber metrics.
- **Review Analysis** — Retrieve and analyze user feedback to identify bugs, feature requests, and sentiment.
- **Rankings & Visibility** — Track your daily category and keyword rankings to optimize your ASO strategy.
- **Competitive Intelligence** — Search and monitor any app on the market to stay ahead of the competition.

### Who is this for?

- **App Developers** — Keep a close eye on your daily metrics and user feedback without switching between multiple dashboards.
- **Product Managers** — Quickly gather data for performance reviews and strategic planning using AI-assisted reporting.
- **Marketing & ASO Teams** — Monitor rankings and featured status to measure the impact of your campaigns and optimizations.


## Available Tools
- **get_account_check**: Verify Appfigures account connection
- **get_external_accounts**: List linked store accounts
- **get_ranks**: Get daily category and keyword rankings
- **get_revenue_report**: Get revenue and proceeds data
- **get_sales_report**: Get sales data (downloads, updates, returns)
- **get_subscriptions_report**: Get subscription metrics (active, churn, etc.)
- **get_user_info**: Retrieve authenticated user information
- **list_featured**: Track when apps are featured on app stores
- **list_my_products**: List all mobile apps in your Appfigures account
- **list_reviews**: List app reviews for your products
- **search_products**: Search for any mobile app across all supported stores


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Appfigures** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the sales report for the last 30 days."

**🤖 AI Agent:**
> I've retrieved your sales report. You had 5,420 total downloads and 12,800 updates over the last 30 days.

---

**👤 You:**
> "What are the latest reviews for my iOS app?"

**🤖 AI Agent:**
> I found 10 new reviews for your iOS app. Most are positive, highlighting the new UI, but 2 users mentioned a crash on the login screen.

---

**👤 You:**
> "Search for the 'Instagram' app on the App Store."

**🤖 AI Agent:**
> I've searched for 'Instagram'. It's currently ranked #1 in Photo & Video with over 4 billion downloads estimated globally.


## ❓ FAQ

**Q: How do I get my Appfigures Client Key and Personal Access Token?**
Go to the [Appfigures Developer Settings](https://appfigures.com/developers/keys) to create an API Client Key and generate a Personal Access Token.

**Q: Can I track competitor apps with this server?**
Yes, you can use the `search_products` tool to find and monitor any app across all supported stores, not just your own.

**Q: Which app stores are supported?**
Appfigures supports iOS, Google Play, Amazon Appstore, Windows Store, and many others. If the store is linked to your Appfigures account, you can access its data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appfigures](https://vinkius.com/mcp/appfigures)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Appfigures** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `appfigures` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Appfigures** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appfigures": {
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
