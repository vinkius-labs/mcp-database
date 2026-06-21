# Campaign Monitor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/campaign-monitor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing via Campaign Monitor — track campaigns, manage subscribers, and monitor performance directly from any AI agent.

## Description
Connect your **Campaign Monitor** account to any AI agent and orchestrate your email marketing, subscriber management, and multi-channel campaigns through natural conversation.

### What you can do

- **Subscriber Oversight** — List all your active subscribers and retrieve detailed profiles, including contact information and history.
- **Campaign Management** — List all email campaigns and retrieve detailed metadata, including subjects and statuses.
- **Performance Tracking** — Retrieve real-time statistics for specific campaigns to monitor engagement, ROI, and delivery rates.
- **List Coordination** — Access and list your contact lists and segments to ensure your audience is properly managed.
- **Client & account Monitoring** — Access core client information and templates managed within the platform.
- **Subscriber Growth** — Add new subscribers directly from your workspace with custom names and automated consent tracking.

### How it works

1. Subscribe to this server
2. Enter your Campaign Monitor API Key
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — quickly check campaign performance or subscriber details without manual dashboard exports.
- **Digital Strategists** — retrieve campaign stats and segment data straight from their planning tools.
- **Developers** — integrate email workflow and subscriber management into their environment using natural language.


## Available Tools
- **add_subscriber**: Add a new subscriber to a list
- **get_account_info**: Retrieve core account information
- **get_campaign_performance**: Retrieve performance summary for a specific campaign
- **get_client_details**: Get details of a specific client
- **get_contact_list**: Get details of a specific contact list
- **list_campaigns**: List all campaigns for a client
- **list_clients**: List all client accounts
- **list_contact_lists**: List all contact lists for a specific client
- **list_subscribers**: List active subscribers in a list
- **list_email_templates**: List all templates for a client


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Campaign Monitor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my clients in Campaign Monitor."

**🤖 AI Agent:**
> I've retrieved your clients. You have 3 clients managed: 'Vinkius North' (ID: cli_1), 'Global Solutions' (ID: cli_2), and 'Tech Corp' (ID: cli_3).

---

**👤 You:**
> "Show the lists for client cli_123."

**🤖 AI Agent:**
> Retrieving lists for client cli_123... You have 2 lists: 'Weekly Newsletter' (ID: list_1) and 'Event Attendees' (ID: list_2).

---

**👤 You:**
> "Add Jane Smith (jane@example.com) to the 'Weekly Newsletter' list."

**🤖 AI Agent:**
> Jane Smith has been successfully added to the 'Weekly Newsletter' list in your Campaign Monitor account.


## ❓ FAQ

**Q: Can I check the statistics for a specific campaign using the agent?**
Yes! Use the `get_campaign_performance` tool with the Campaign ID. Your agent will fetch the detailed performance data, including open rates, clicks, and bounces, directly from Campaign Monitor.

**Q: How do I add a new subscriber to a list?**
Simply ask the agent to `add_subscriber` and provide the List ID, name, and email address. The subscriber will be added to your Campaign Monitor list with consent tracking enabled automatically.

**Q: Does the integration allow listing all my clients?**
Yes. Use the `list_clients` tool. It will retrieve all the client accounts managed under your Campaign Monitor account, making it easy to find the IDs needed for other operations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/campaign-monitor](https://vinkius.com/mcp/campaign-monitor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Campaign Monitor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `campaign-monitor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Campaign Monitor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "campaign-monitor": {
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
