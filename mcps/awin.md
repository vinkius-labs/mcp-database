# Awin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/awin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Global affiliate marketing automation — manage advertiser programmes, track transactions, and generate tracking links via AI.

## Description
Orchestrate your affiliate marketing performance with **Awin**, the world's leading affiliate network. By connecting Awin to your AI agent, you transform complex data retrieval and program management into a natural conversation. Your agent can instantly audit transaction history, list joined advertiser programmes, retrieve real-time performance reports, and even generate tracked affiliate links without you ever touching a dashboard. Whether you're a publisher optimizing revenue or an advertiser monitoring relationships, your agent acts as a direct bridge to your Awin account, ensuring your marketing efforts are always data-driven and efficient.

### What you can do

- **Account Oversight** — List all publisher and advertiser accounts you have access to across the Awin network.
- **Programme Management** — Explore joined or available advertiser programmes, auditing relationship statuses and requirements.
- **Transaction Auditing** — Retrieve detailed lists of individual transactions, complete with metadata, status, and conversion values.
- **Performance Reporting** — Access aggregated performance reports to analyze revenue and conversion trends over specific timeframes.
- **Link Generation** — Instantly generate tracking links for destination URLs to ensure your affiliate traffic is correctly attributed.

### How it works

1. Subscribe to this server
2. Enter your Awin API Token
3. Start managing your affiliate marketing data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Affiliate Marketers** — quickly generate tracking links and audit recent transaction successes via natural language.
- **Publisher Managers** — monitor advertiser relationships and discover new programmes to join directly from chat.
- **Data Analysts** — extract aggregated performance metrics for revenue reporting without manual CSV exports.
- **Operations Leads** — audit account connectivity and verify transaction statuses across multiple publisher accounts.


## Available Tools
- **generate_tracking_link**: Generate an Awin tracking link for a destination URL
- **get_account_check**: Verify Awin connection and list available accounts
- **get_aggregated_report**: Get aggregated performance reports
- **list_accounts**: List all accounts (publisher/advertiser) you have access to
- **list_available_programmes**: Helper to list only available programmes to join
- **list_joined_programmes**: Helper to list only joined programmes
- **list_programmes**: List joined or available advertiser programmes for a publisher
- **list_promotions**: Retrieve details of promotions and voucher codes for a publisher
- **list_publishers**: List all publishers with an active relationship (for advertisers)
- **list_transactions**: List individual transactions for a publisher (max 31 days)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Awin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all advertiser programmes I have joined on Awin for Publisher ID 12345."

**🤖 AI Agent:**
> I've retrieved your joined programmes for Publisher 12345. You are currently active in 15 programmes, including 'TechStore Global' and 'FashionHub'. Would you like details on a specific one?

---

**👤 You:**
> "Generate an Awin tracking link for https://example.com/product using Publisher 12345 and Advertiser 6789."

**🤖 AI Agent:**
> Tracking link generated successfully: https://www.awin1.com/cread.php?awinmid=6789&awinaffid=12345&p=https://example.com/product. You can now use this link for your affiliate promotion.

---

**👤 You:**
> "Show my aggregated performance report for the last 7 days in UTC."

**🤖 AI Agent:**
> Analyzing your performance for the last 7 days... You had 1,200 clicks, 45 conversions, and an estimated commission of €350. This is a 10% increase compared to the previous week.


## ❓ FAQ

**Q: How do I find my Publisher ID for queries?**
Use the `list_accounts` tool. It will return all accounts associated with your token, including their unique IDs and account types (Publisher or Advertiser).

**Q: Can I filter transactions by status?**
Yes. When using the `list_transactions` tool, you can provide a status parameter such as 'pending', 'approved', 'declined', or 'deleted' to narrow down your results.

**Q: How far back can I retrieve transaction data?**
The Awin API allows you to retrieve individual transactions for a maximum range of 31 days per request. For longer periods, you may need to perform multiple targeted queries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/awin](https://vinkius.com/mcp/awin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Awin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `awin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Awin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "awin": {
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
