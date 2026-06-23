# Givebutter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/givebutter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage fundraising campaigns, track donations, and oversee donors via AI agents with Givebutter.

## Description
Connect your **Givebutter** account to any AI agent to automate your fundraising operations and donor management through the Model Context Protocol (MCP). Givebutter is the modern fundraising platform for nonprofits and changemakers. This MCP server enables you to retrieve donation transactions, manage fundraising campaigns, and synchronize donor profiles (contacts) directly through natural conversation.

### Key Features

- **Donation Oversight** — List all donation transactions, fetch detailed metadata including status and timestamps, and monitor your revenue flow instantly.
- **Campaign Management** — Access active fundraising campaigns and events, retrieving detailed configuration and total raised amounts.
- **Donor Synchronization** — Search and list donor profiles, retrieve detailed contact metadata, and programmatically add new donors to your database.
- **Offline Recording** — Record offline donations or external payments programmatically to maintain a unified source of truth for your fundraising.
- **Recurring Plan Monitoring** — List and track configured recurring donation plans to understand long-term donor commitment.
- **Webhook Visibility** — Monitor active webhooks to ensure your internal systems are receiving real-time donation notifications.
- **Real-time Synchronization** — Keep your nonprofit's financial data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Givebutter API Key (found in Settings > Developers > API)
3. Start managing your fundraising from Claude, Cursor, or any MCP client

### Who is this for?

- **Nonprofit Ops & Finance** — quickly check if a large donation has been cleared or list recent successful transactions without manual dashboard navigation.
- **Development Directors** — get a real-time overview of campaign performance and donor activity via simple AI commands.
- **Donor Relations** — verify donor history and synchronize new contacts into your database seamlessly.


## Available Tools (12)
- **verify_api_connection**: Check connection
- **sync_donor_contact**: Add new donor
- **record_offline_donation**: Log a donation
- **get_account_details**: Get account identity
- **get_campaign_details**: Get campaign metadata
- **get_transaction_details**: Get transaction metadata
- **list_fundraising_campaigns**: List active campaigns
- **list_donor_contacts**: List donor profiles
- **list_recurring_plans**: List recurring plans
- **list_recent_donations**: List last 10 success
- **list_donation_transactions**: List donations
- **list_donation_webhooks**: List webhook configs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Givebutter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all successful donations from the last 24 hours."

**🤖 AI Agent:**
> Retrieving donations... I found 12 successful transactions in the last 24 hours, totaling $1,250.00. Would you like to see the details for the largest one?

---

**👤 You:**
> "Check the progress of our 'Annual Gala' campaign (ID: gala_2024)."

**🤖 AI Agent:**
> Fetching campaign details... The 'Annual Gala' has raised $45,000 so far, which is 75% of your $60,000 goal. There have been 150 unique donors.

---

**👤 You:**
> "Log an offline donation of $50.00 from 'Alice Smith' (ID: contact_123)."

**🤖 AI Agent:**
> Donation logged! I have successfully recorded the $50.00 offline transaction for Alice Smith. The new Transaction ID is 'tx_98765'.


## ❓ FAQ

**Q: How do I get an API Key for Givebutter?**
Log in to your Givebutter dashboard, navigate to Settings > Developers > API, and you can generate a new secret API key there.

**Q: Can I process live credit card transactions via the agent?**
No, this integration is for management and data retrieval. For security, live donor checkouts must still happen through Givebutter's secure forms.

**Q: What format should the donation amount be in?**
The Givebutter API uses major units for amounts. For example, to record a $10.50 donation, you should provide the decimal value '10.50'.

**Q: How do I link a transaction to a specific campaign?**
Use the 'campaign_id' parameter in the 'record_offline_donation' tool. You can find your campaign IDs using the 'list_fundraising_campaigns' tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/givebutter](https://vinkius.com/mcp/givebutter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Givebutter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `givebutter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Givebutter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "givebutter": {
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
