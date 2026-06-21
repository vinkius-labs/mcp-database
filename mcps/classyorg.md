# Classy.org MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/classyorg)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage fundraising and donations via Classy (GoFundMe Pro) — track campaigns, monitor transactions, and manage supporters directly from any AI agent.

## Description
Connect your **Classy.org (GoFundMe Pro)** account to any AI agent and take full control of your fundraising operations through natural conversation. Streamline how you manage donor relationships and campaign performance natively.

### What you can do

- **Campaign Oversight** — List and retrieve details for all active and inactive fundraising campaigns natively
- **Transaction Intelligence** — Access recent donation and registration records including amounts and statuses flawlessly
- **Supporter Logistics** — List community members and individual supporters to maintain relationships securely
- **Page & Team Management** — Monitor individual fundraising pages and team-based efforts flawlessly
- **Activity Auditing** — Access a real-time feed of interactions, such as new donations or page creations, flawlessly
- **Organization Visibility** — Retrieve organization settings and high-level data directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Classy Client ID and Client Secret (obtained from Classy Manager > Apps & Integrations)
3. Start managing your fundraising from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Nonprofit Directors** — monitor fundraising goals and campaign success using natural language
- **Development Officers** — audit recent transactions and supporter activity without opening the manager
- **Marketing Teams** — quickly look up campaign details and activity feeds straight from their chat interface
- **Donor Relations** — verify member profiles and individual fundraising progress


## Available Tools
- **get_activity_feed**: Retrieve a feed of recent interactions (donations, registrations)
- **get_campaign_details**: Get detailed information for a specific campaign
- **list_fundraising_campaigns**: List all fundraising campaigns
- **list_individual_fundraising_pages**: List individual supporter fundraising pages
- **list_fundraising_teams**: List team-based fundraising pages
- **list_classy_members**: List community members and supporters
- **list_classy_organizations**: Retrieve organization data and settings
- **list_donation_transactions**: List recent donation and registration transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Classy.org** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active fundraising campaigns in Classy."

**🤖 AI Agent:**
> Retrieving your active campaigns... I found 3: 'Annual Gala 2026', 'Clean Water Initiative', and 'Spring Fundraiser'. Would you like to see the totals for any of these?

---

**👤 You:**
> "Show me the last 5 donations."

**🤖 AI Agent:**
> Checking recent transactions... I found 5 donations ranging from $25.00 to $500.00. The most recent one was from Sarah Smith for $100.00 to the 'Clean Water' campaign.

---

**👤 You:**
> "Who are the top fundraisers in the 'Marathon 2026' team?"

**🤖 AI Agent:**
> Retrieving 'Marathon 2026' team members... The top 3 fundraisers are: John Doe ($1,200), Mike Scott ($950), and Jane Smith ($800).


## ❓ FAQ

**Q: Can I see how much a specific campaign has raised?**
Yes! Use the `get_campaign_details` tool with the campaign ID. The agent will return the total gross amount raised along with other performance metrics.

**Q: How do I check the latest donations through the agent?**
Use the `list_donation_transactions` tool or the `get_activity_feed` tool. Your agent will fetch the most recent records, including the donor's name and the donation amount.

**Q: Where do I find my Classy API Client ID and Secret?**
Log in to your Classy Manager and navigate to **Apps & Integrations > API**. You can create a new API application to generate your Client ID and Client Secret.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/classyorg](https://vinkius.com/mcp/classyorg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Classy.org** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `classyorg` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Classy.org** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "classyorg": {
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
