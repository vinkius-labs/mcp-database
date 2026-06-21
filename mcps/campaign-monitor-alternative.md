# Campaign Monitor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/campaign-monitor-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Design branded email campaigns, segment subscriber lists, and measure engagement with professional marketing analytics.

## Description
Connect your **Campaign Monitor** account to any AI agent and take full control of your professional email marketing and audience engagement workflows through natural conversation.

### What you can do

- **Audience Orchestration** — List and manage your subscriber lists programmatically, retrieving detailed metadata and health statistics (active, unsubscribed, bounced) in real-time
- **Subscriber Lifecycle** — Programmatically add or update people in your lists, including managing custom fields and re-subscription status directly from your agent
- **Campaign Architecture** — Monitor sent and scheduled email campaigns across multiple clients to maintain high-fidelity oversight of your digital outreach
- **Performance Intelligence** — Access real-time campaign analytics including opens, clicks, and engagement metrics to coordinate your marketing strategy
- **Multi-Tenant Visibility** — Retrieve complete directories of sub-accounts (clients) and their associated lists to perfectly coordinate agency or enterprise environments

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from Campaign Monitor (Account Settings > API Key)
3. Start managing your email marketing pipeline from Claude, Cursor, or any MCP client

No more manual scrubbing through subscriber exports or slow UI navigation. Your AI acts as your dedicated email operations and audience coordinator.

### Who is this for?

- **Marketing Managers** — instantly retrieve campaign results and update subscriber segments using natural language commands
- **Growth Marketers** — automate the ingestion of new leads and monitor list health without leaving your workspace
- **Agency Leads** — orchestrate email operations across multiple client accounts through simple AI queries


## Available Tools (7)
- **add_subscriber**: Create or update a subscriber
- **get_campaign_analytics**: Get campaign performance
- **get_list_statistics**: Get subscriber list health
- **get_subscriber_details**: Get profile for a subscriber
- **list_sent_campaigns**: List recent email campaigns
- **list_clients**: List your account clients
- **list_subscriber_lists**: List lists for a client


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Campaign Monitor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my clients and their associated subscriber lists."

**🤖 AI Agent:**
> I've retrieved your organization's directory. You have 2 main clients: 'Acme Corp' (ID: abc-123) and 'Global Tech'. Acme Corp has 3 lists, including 'Weekly Newsletter' and 'Product Beta'. Which one should we explore?

---

**👤 You:**
> "Add 'John Doe' (john@example.com) to the 'Weekly Newsletter' list (ID: 'l_456')."

**🤖 AI Agent:**
> Subscriber added! I've successfully registered John Doe in the 'Weekly Newsletter' list. His profile is now active and he will receive your next scheduled broadcast.

---

**👤 You:**
> "What is the performance summary for campaign ID 'c_789'?"

**🤖 AI Agent:**
> Fetching analytics... Campaign c_789 ('Holiday Promo') has a 22% open rate and a 4% click-through rate. Total successful deliveries: 5,420. Shall I check for any bounced addresses?


## ❓ FAQ

**Q: How do I find my Campaign Monitor API Key?**
Log in to your account, click on your profile (top right), navigate to **Account Settings** > **API Key**, and copy your unique token.

**Q: Can I manage multiple clients via AI?**
Yes! The `list_clients` tool retrieves all sub-accounts, and you can use their IDs to manage lists and campaigns specifically for each client.

**Q: Does it support real-time campaign analytics?**
The `get_campaign_analytics` tool retrieves the most current engagement metrics (opens, clicks, unsubscribes) directly from the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/campaign-monitor-alternative](https://vinkius.com/mcp/campaign-monitor-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `campaign-monitor-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Campaign Monitor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "campaign-monitor-alternative": {
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
