# GiveWP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/givewp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage donation forms, track donors, and oversee fundraising stats via AI agents with GiveWP.

## Description
Connect your **GiveWP** (WordPress plugin) account to any AI agent to automate your donation data extraction and fundraising reporting through the Model Context Protocol (MCP). GiveWP is the most popular WordPress plugin for online giving. This MCP server enables you to retrieve donation forms, track individual donor profiles, and monitor real-time fundraising statistics directly through natural conversation.

### Key Features

- **Form Oversight** — List all donation forms published on your WordPress site and fetch detailed configuration metadata and goal progress.
- **Donation Management** — List all donations processed via the plugin, with support for filtering by specific forms or donors.
- **Donor Discovery** — Retrieve detailed profile metadata for your unique donors and search across their giving history.
- **Real-time Analytics** — Fetch high-level earnings and donation count statistics for your entire site or individual forms.
- **Read-only Security** — Safely query your WordPress donation database with a secure integration designed for data visibility.
- **Plugin Transparency** — Access high-level plugin metadata to verify API connectivity and account health.
- **Real-time Synchronization** — Keep your self-hosted fundraising data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your WordPress Base URL and GiveWP API Keys (found in User Profile > Account Management)
3. Start querying your donation data from Claude, Cursor, or any MCP client

### Who is this for?

- **Nonprofit Site Admins** — quickly check if a donation has been synchronized or list active forms without manual dashboard navigation.
- **Digital Fundraisers** — get a real-time overview of campaign performance and donor activity via simple AI commands.
- **Marketing Analysts** — automate the retrieval of donation statistics for weekly fundraising reports.


## Available Tools (9)
- **find_donor_history**: Search by donor
- **get_form_performance**: Get form stats
- **get_form_details**: Get form metadata
- **get_plugin_stats**: Get general stats
- **list_plugin_donations**: List all donations
- **list_donation_forms**: List all forms
- **list_recent_donations**: List latest records
- **verify_api_connection**: Check connection
- **list_plugin_donors**: List all donors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GiveWP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active donation forms on my website."

**🤖 AI Agent:**
> Retrieving forms... I found 4 active donation forms, including 'Emergency Relief Fund' (ID: 123) and 'Monthly Sponsorship'. Would you like to see the goal progress for any of them?

---

**👤 You:**
> "Show me the donation history for donor 'jane@example.com'."

**🤖 AI Agent:**
> Fetching history... Jane Doe has made 5 donations totaling $250.00. Her most recent contribution was $50.00 on September 15th for the 'Holiday Campaign'.

---

**👤 You:**
> "Get the fundraising stats for the 'Annual Fund' form (ID: 987)."

**🤖 AI Agent:**
> Retrieving stats... The 'Annual Fund' form has raised $12,450.00 from 145 unique donations. The average donation amount is $85.86.


## ❓ FAQ

**Q: How do I get API Keys for GiveWP?**
Log in to your WordPress admin, go to your User Profile, and scroll to 'Account Management'. Check 'Generate API Keys' and update your profile to see your keys.

**Q: What is the WordPress Base URL?**
This is the root domain where your WordPress site is installed, for example: 'https://my-nonprofit.org'. Do not include '/wp-admin/'.

**Q: Can I edit donation forms via the agent?**
The current version of the GiveWP API tools is primarily designed for data retrieval and reporting. Editing capabilities are not supported in this release.

**Q: How do I see donor history?**
Use the 'find_donor_history' tool and provide the donor's email address. The agent will retrieve all donation records associated with that person.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/givewp](https://vinkius.com/mcp/givewp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GiveWP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `givewp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GiveWP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "givewp": {
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
