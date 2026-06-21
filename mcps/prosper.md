# Prosper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prosper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage your Prosper peer-to-peer investments — check account balances, search loan listings, submit bids, and track your portfolio performance.

## Description
Connect your **Prosper** investment account to any AI agent to automate your peer-to-peer lending strategy. Monitor your portfolio, discover new investment opportunities, and manage your notes through natural conversation.

### What you can do

- **Account Overview** — Retrieve real-time account balances, total value, and available cash for investment via `get_accounts`.
- **Marketplace Discovery** — Search active loan listings using filters like Prosper ratings, biddable status, and credit data with `search_listings`.
- **Automated Bidding** — Submit orders and bids on multiple listings simultaneously to build your portfolio using `submit_order`.
- **Portfolio Tracking** — List and inspect originated loans, specific notes, and payment histories to monitor returns with `list_loans` and `list_notes`.
- **Order Management** — Check the status of submitted orders to confirm successful investments or identify issues using `get_order`.

### How it works

1. Subscribe to this server
2. Enter your Prosper Personal Access Token
3. Start managing your P2P investments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Individual Investors** — automate the search for high-yield listings and track monthly payments without manual logins.
- **Financial Analysts** — pull portfolio data directly into analysis tools to calculate ROI and risk exposure.
- **Developers** — build custom investment bots or dashboards using the Prosper marketplace data.


## Available Tools
- **get_accounts**: Retrieve account balance and investment summaries
- **create_offer**: Generate personalized loan offers for potential borrowers
- **get_loan**: View details of a specific originated loan
- **get_note**: View details of a specific Note investment
- **get_order**: g., BID_SUCCEEDED, INSUFFICIENT_FUNDS).

Check the status of a submitted order
- **list_loans**: View originated loans you have invested in
- **list_notes**: View specific Note investments
- **list_payments**: Retrieve payment history for loans
- **search_listings**: Search for active loan listings to invest in
- **submit_order**: Submit bids on listings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prosper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current Prosper account balance and available cash?"

**🤖 AI Agent:**
> I've retrieved your account details. You have a total account value of $12,450.00, with $1,200.50 available in cash for new investments.

---

**👤 You:**
> "Find active AA-rated loan listings that I haven't invested in yet."

**🤖 AI Agent:**
> Searching the marketplace... I found 3 active AA-rated listings where you don't have an existing investment. Would you like to see the details for Listing ID 1092384?

---

**👤 You:**
> "Show me the details for loan number 123456 and its next payment date."

**🤖 AI Agent:**
> Inspecting loan 123456... The current principal balance is $2,100.00. The next payment of $145.20 is scheduled for October 15th.


## ❓ FAQ

**Q: Can I search for specific loan ratings like AA or HR?**
Yes, use the `search_listings` tool with the `prosper_rating` parameter to filter for specific risk profiles in the marketplace.

**Q: How do I check if my bid was successful?**
Use the `get_order` tool with your Order ID to retrieve the results, such as BID_SUCCEEDED or INSUFFICIENT_FUNDS.

**Q: Can I see my recent payment history for my investments?**
Yes, the `list_payments` tool fetches your payment history, defaulting to the last 90 days of transactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prosper](https://vinkius.com/mcp/prosper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prosper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `prosper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prosper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prosper": {
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
