# Campaigner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/campaigner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing via Campaigner — track campaigns, manage subscribers, and monitor performance directly from any AI agent.

## Description
Connect your **Campaigner** account to any AI agent and orchestrate your email marketing, subscriber management, and multi-channel campaigns through natural conversation.

### What you can do

- **Subscriber Oversight** — List all your subscribers and retrieve detailed profiles, including contact information and history.
- **Campaign Management** — List all email campaigns and retrieve detailed metadata, including subjects and automated workflows.
- **Performance Tracking** — Retrieve real-time statistics for specific campaigns to monitor engagement and ROI.
- **Publication Coordination** — Access and list your 'Publications' (contact lists) to ensure your audience segments are properly managed.
- **Workflow & Segment Monitoring** — List automated workflows and audience segments directly from your workspace.
- **Subscriber Growth** — Create and add new subscribers to your account using natural language.

### How it works

1. Subscribe to this server
2. Enter your Campaigner API Key
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — quickly check campaign performance or subscriber details without manual dashboard work.
- **Digital Strategists** — retrieve campaign stats and segment data straight from their planning tools.
- **Developers** — integrate email workflow and subscriber management into their environment using natural language.


## Available Tools (10)
- **create_subscriber**: Add a new subscriber to Campaigner
- **get_account_info**: Retrieve core account information
- **get_campaign_stats**: Retrieve performance statistics for a campaign
- **get_campaign**: Get details of a specific campaign
- **get_subscriber**: Get details of a specific subscriber by email
- **list_campaigns**: List all email campaigns
- **list_publications**: List all publications/contact lists
- **list_segments**: List configured audience segments
- **list_subscribers**: List all newsletter subscribers
- **list_workflows**: List automated workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Campaigner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email campaigns in Campaigner."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have several active and draft campaigns, including 'Spring Promo' (ID: camp_1) and 'User Onboarding' (ID: camp_2).

---

**👤 You:**
> "Show the stats for campaign ID 12345."

**🤖 AI Agent:**
> Retrieving stats for campaign 12345... It has a 25% open rate, a 5% click rate, and has been sent to 1,000 subscribers.

---

**👤 You:**
> "Search for subscriber with email john.doe@example.com."

**🤖 AI Agent:**
> I've found the subscriber profile for John Doe. He is currently 'Subscribed' and is associated with the 'Customers' and 'Weekly Update' lists.


## ❓ FAQ

**Q: Can I check the statistics for a specific campaign using the agent?**
Yes! Use the `get_campaign_stats` tool with the Campaign ID. Your agent will fetch the detailed performance data, including open rates, clicks, and bounces, directly from Campaigner.

**Q: How do I list all the subscribers in my account?**
Simply ask the agent to `list_subscribers`. It will retrieve the list of contacts from your Campaigner account, including their status and primary details.

**Q: Does the integration allow adding a new subscriber?**
Yes. Use the `create_subscriber` action and provide the email address. The contact will be added to your Campaigner account immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/campaigner](https://vinkius.com/mcp/campaigner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Campaigner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `campaigner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Campaigner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "campaigner": {
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
