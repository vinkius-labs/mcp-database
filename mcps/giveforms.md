# GiveForms MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/giveforms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [payment-processing](../categories/payment-processing.md)

Retrieve donation records and oversee fundraising data via AI agents with GiveForms.

## Description
Connect your **GiveForms** account to any AI agent to automate your donation data extraction and fundraising reporting through the Model Context Protocol (MCP). GiveForms is a high-conversion donation platform for nonprofits. This MCP server enables you to retrieve detailed donation records, filter contributions by campaign, and search for donor activity directly through natural conversation.

### Key Features

- **Donation Oversight** — List all donation records for your organization and fetch detailed metadata for specific contributions.
- **Campaign-Specific Tracking** — Filter and retrieve donations associated with a specific fundraising campaign ID.
- **Donor History Discovery** — Search for donation records using a donor's email address or their full name to understand their giving history.
- **Real-time Data Access** — Safely query your donation database with a secure integration designed for data visibility and reporting.
- **Organization Insights** — Access high-level metadata for your authenticated organization to verify connectivity and settings.
- **Real-time Synchronization** — Keep your fundraising data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GiveForms Organization ID and API Key (found in Settings > Integrations)
3. Start querying your donation data from Claude, Cursor, or any MCP client

### Who is this for?

- **Nonprofit Development Leads** — quickly check if a specific donation has been recorded or list recent contributions without manual dashboard navigation.
- **Finance & Audit Teams** — get a real-time overview of campaign performance and donor history via simple AI commands.
- **Donor Relations Managers** — verify an individual donor's total contributions and campaign involvement seamlessly.


## Available Tools (8)
- **verify_api_connection**: Check connection
- **find_donations_by_email**: Search donor by email
- **find_donations_by_name**: Search donor by name
- **get_organization_info**: Get org metadata
- **get_donation_details**: Get donation metadata
- **list_campaign_donations**: Filter by campaign
- **list_all_donations**: List all records
- **list_recent_donations**: List latest records


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GiveForms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all donations received this month."

**🤖 AI Agent:**
> Retrieving donations... I found 15 donations for this month, including $100 from 'John Smith' and $25 from 'Jane Doe'. Would you like the full details for the largest contribution?

---

**👤 You:**
> "Find all donations from donor 'alice@email.com'."

**🤖 AI Agent:**
> Searching records... Alice Smith has made 3 donations totaling $150. Her most recent was $50 for the 'Winter Fundraiser'.

---

**👤 You:**
> "Show me the 5 most recent donations for campaign '98765'."

**🤖 AI Agent:**
> Fetching campaign donations... For campaign 98765, I found 5 recent contributions. All are processed successfully. Would you like to see the donor names?


## ❓ FAQ

**Q: How do I get an API Key for GiveForms?**
Log in to your GiveForms dashboard, navigate to Settings > Integrations, and look for the REST API section to find your Organization ID and API Key.

**Q: Can I manually add donations via the agent?**
The current version of the GiveForms API is primarily designed for data retrieval and auditing. Creation tools may be added in future updates.

**Q: How do I find a specific Campaign ID?**
The Campaign ID is the number found at the end of the URL when you view or edit a campaign within your GiveForms dashboard.

**Q: Is the donation data returned in real-time?**
Yes, all data retrieved through this MCP server is fetched directly from the GiveForms REST API, providing you with the latest available donation records.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/giveforms](https://vinkius.com/mcp/giveforms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GiveForms** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `giveforms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GiveForms** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "giveforms": {
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
