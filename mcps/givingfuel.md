# GivingFuel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/givingfuel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Retrieve donation orders, track registrants, and oversee fundraising pages via AI agents with GivingFuel.

## Description
Connect your **GivingFuel** account to any AI agent to automate your fundraising data extraction and donor relationship management through the Model Context Protocol (MCP). GivingFuel is a powerful, flexible fundraising platform for nonprofits and ministries. This MCP server enables you to retrieve donation orders, track individual donor responses (registrants), and monitor active fundraising pages directly through natural conversation.

### Key Features

- **Donation Oversight** — List all donation orders for your organization, including transaction totals and status (completed, refunded, pending).
- **Donor Detail Discovery** — Retrieve detailed records for individual donors and their specific form responses to understand donor sentiment.
- **Financial Transaction Tracking** — Access financial processing data for both successful and failed charges to monitor payment health.
- **Page Management** — List all active fundraising pages and events, retrieving detailed configuration metadata for each.
- **Donor CRM Insights** — Access unified donor profiles from the Webconnex platform to track long-term donor engagement.
- **P2P Campaign Discovery** — Retrieve data related to Peer-to-Peer fundraising campaigns and participant activity.
- **Real-time Synchronization** — Keep your organization's fundraising data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GivingFuel API Key (found in Extras > Integrations > API Keys)
3. Start querying your donation data from Claude, Cursor, or any MCP client

### Who is this for?

- **Nonprofit Directors** — quickly check the status of recent donations or verify campaign progress without manual dashboard navigation.
- **Development Teams** — get a real-time overview of donor registrants and form responses via simple AI commands.
- **Finance Managers** — automate the retrieval of financial transaction data for auditing and reporting.


## Available Tools (10)
- **filter_orders_by_date**: Filter by date range
- **list_crm_contacts**: List donor profiles
- **list_donation_orders**: List all orders
- **list_peer_campaigns**: List P2P campaigns
- **list_fundraising_pages**: List donation pages
- **list_recent_donations**: List latest 10 orders
- **list_donation_registrants**: List individual donors
- **list_financial_transactions**: List successful charges
- **verify_api_connection**: Check connection
- **filter_orders_by_status**: Filter by completion


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GivingFuel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 donation orders received."

**🤖 AI Agent:**
> Retrieving orders... I found 5 recent donations, including $100 from 'Michael Scott' and $50 from 'Jim Halpert'. Would you like to see the registrant details for any of them?

---

**👤 You:**
> "Show me all fundraising pages active in my account."

**🤖 AI Agent:**
> Retrieving pages... I found 3 active donation pages: 'Fall Gala 2024', 'Building Fund', and 'Monthly Giving Circle'. Which one would you like to see the configuration for?

---

**👤 You:**
> "How many donations were marked as 'refunded' today?"

**🤖 AI Agent:**
> Checking transactions... I found 2 donation orders marked as 'refunded' today, totaling $75.00. One was for the 'Summer Camp' fund.


## ❓ FAQ

**Q: How do I get an API Key for GivingFuel?**
Log in to your GivingFuel account, navigate to Extras > Integrations > API Keys, and click 'Add API Key' to generate your key.

**Q: Can I add new donations via the agent?**
The GivingFuel Public API is primarily designed for data extraction and polling. To record new donations, use your GivingFuel hosted donation pages.

**Q: How do I filter donations for a specific date range?**
Use the 'filter_orders_by_date' tool and provide an ISO date (YYYY-MM-DD). The agent will retrieve all records created after that date.

**Q: Does this support multiple Webconnex products?**
This MCP server is specifically configured to filter results for GivingFuel (givingfuel.com). It ensures you only see fundraising-related data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/givingfuel](https://vinkius.com/mcp/givingfuel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GivingFuel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `givingfuel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GivingFuel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "givingfuel": {
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
