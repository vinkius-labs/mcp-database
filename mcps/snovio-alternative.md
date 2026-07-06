# Snov.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snovio-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Find business emails, verify deliverability, and run multi-step drip campaigns that fill your outbound sales pipeline.

## Description
Connect your **Snov.io** account to any AI agent and take full control of your lead generation and high-fidelity outreach orchestration through natural conversation.

### What you can do

- **Email Discovery Intelligence** — Find all high-fidelity email addresses for a specific domain to identify key decision makers programmatically
- **Prospect Portfolio Management** — List saved prospect lists, retrieve detailed profile metadata, and add new leads directly through your agent
- **Outreach Campaign Monitoring** — Access your complete directory of high-fidelity marketing campaigns and monitor real-time performance analytics
- **Identity Enrichment** — Retrieve technical profile data for specific prospects using unique IDs or email addresses programmatically
- **Real-time Webhook Access** — Monitor configured high-fidelity notification streams and events directly through your agent for perfectly coordinated outreach
- **Operational Monitoring** — Verify account-level API connectivity and monitor lead orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API User ID** and **API Secret** from your Snov.io account (Settings > API)
3. Start managing your growth metrics from Claude, Cursor, or any MCP client

No more manual lead entry or missing campaign gaps. Your AI acts as your dedicated growth coordinator and outreach architect.

### Who is this for?

- **Sales Managers** — instantly retrieve prospect lists and campaign statuses using natural language commands without leaving your creative workspace
- **Growth Engineers** — automate high-fidelity domain searches and monitor lead verification to ensure healthy outreach operations
- **Marketing Teams** — analyze technical campaign analytics and monitor webhook events through simple AI queries


## Available Tools (10)
- **get_snovio_campaign_analytics**: Get campaign analytics
- **get_snovio_prospect_by_email**: Get prospect details by email
- **get_snovio_prospect_by_id**: Get prospect details by ID
- **list_snovio_campaigns**: List outreach campaigns
- **list_snovio_prospect_lists**: List prospect lists
- **list_snovio_webhooks**: List account webhooks
- **check_snovio_status**: io API credentials.

Check API Status
- **add_snovio_prospect_to_list**: Add prospect to list
- **find_snovio_domain_emails**: Find emails for a domain
- **find_snovio_prospect_by_name**: Find email by name and domain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snov.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all high-fidelity emails for the domain 'vinkius.com'."

**🤖 AI Agent:**
> I've retrieved the domain data. You currently have 12 active high-fidelity profiles for vinkius.com, including 'admin@vinkius.com' and 'tech@vinkius.com'. Would you like the detailed identity metadata for any of them?

---

**👤 You:**
> "Show the last 5 campaigns and their analytics."

**🤖 AI Agent:**
> Growth orchestrated! I've identified 5 active high-fidelity campaigns, including 'Q2 Outreach'. I've retrieved the technical open rates and conversion metadata for your review. Shall I summarize the campaign performance?

---

**👤 You:**
> "Check the team webhooks for lead events."

**🤖 AI Agent:**
> Notification stream orchestrated! You currently have 3 high-fidelity webhook profiles active for account events. Your API connection is healthy. Shall I retrieve the detailed event orchestration metadata for these webhooks?


## ❓ FAQ

**Q: How do I find my Snov.io API Credentials?**
Log in to your account, navigate to **Settings** > **API**, and locate your unique **API User ID** and **API Secret** tokens.

**Q: Can I check campaign analytics via AI?**
Yes! The `get_snovio_campaign_analytics` tool allows your agent to retrieve high-fidelity performance data and conversion metrics for any specific campaign.

**Q: How do I list my prospect lists?**
Use the `list_snovio_prospect_lists` tool to retrieve the complete high-fidelity directory of lists along with their unique identifiers for precise orchestration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snovio-alternative](https://vinkius.com/mcp/snovio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Snov.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `snovio-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Snov.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "snovio-alternative": {
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
