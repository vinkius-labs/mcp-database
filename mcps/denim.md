# Denim MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/denim)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage marketing campaigns, track contacts, and monitor analytics via the Denim API.

## Description
Integrate **Denim**, the specialized marketing automation platform for financial services, directly into your AI workflow. Manage your multi-channel marketing campaigns, track subscriber profiles and segments, and monitor real-time performance analytics using natural language.

### What you can do

- **Campaign Oversight** — List and retrieve detailed settings and performance metrics for all your marketing campaigns.
- **Contact Management** — Access subscriber profiles, behavioral metadata, and opt-in statuses in your core contact database.
- **Automation Monitoring** — Track active automated workflows and drip sequences to ensure consistent customer engagement.
- **Audience Segments** — List and explore configured audience groups based on structural definitions and filtering criteria.

### How it works

1. Connect the Denim integration to your AI assistant.
2. Authorize using your Denim API Key (found in your account settings).
3. Orchestrate your financial services marketing through intuitive conversation.

### Who is this for?

- **Marketing Directors** — Quickly check campaign delivery and overall engagement on the go.
- **Sales & CRM Teams** — Research contact profiles and behavioral trends via chat.
- **Digital Marketers** — Audit marketing automations and target segments during campaign planning.


## Available Tools
- **add_new_contact**: Add a new contact to your Denim database
- **get_account_metadata**: Retrieve settings and limits for your Denim account
- **get_campaign_analytics**: Retrieve performance metrics for a specific campaign
- **get_campaign_details**: Get detailed settings for a specific campaign
- **list_active_automations**: List active automated marketing workflows
- **list_marketing_campaigns**: List all marketing campaigns in your Denim account
- **list_crm_contacts**: List all contacts and leads in the system
- **list_audience_segments**: List configured audience segments for targeting
- **list_email_templates**: List all available marketing templates
- **search_active_campaigns**: Search for running campaigns by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Denim** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns."

**🤖 AI Agent:**
> I've found 4 active campaigns, including 'Mortgage Refinance 2024' and 'Wealth Management Newsletter'. Would you like to see the performance metrics for the largest one?

---

**👤 You:**
> "Show me the engagement stats for the 'Summer Savings' campaign."

**🤖 AI Agent:**
> The 'Summer Savings' campaign has an open rate of 28% and a click-through rate of 4.5%. A total of 1,200 unique clicks were recorded. Should I list the top links clicked?

---

**👤 You:**
> "Find contact profile for 'user@example.com'."

**🤖 AI Agent:**
> I've retrieved the profile for 'user@example.com'. They are currently 'Subscribed' and part of the 'High Net Worth' segment. Their last interaction was with the 'Q2 Investment Update' email. Would you like to see their full behavioral history?


## ❓ FAQ

**Q: How do I get a Denim API Key?**
Log in to your Denim account, navigate to **Settings > API**, and you can generate or retrieve your unique API Key from that section.

**Q: Can the agent send new campaigns?**
This integration currently focuses on monitoring existing campaigns, segments, and analytics. Creating or launching new campaigns should be handled via the Denim dashboard.

**Q: Does the integration show real-time engagement?**
Yes, you can use the get_campaign_analytics tool to retrieve the latest reported engagement metrics for any of your active campaigns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/denim](https://vinkius.com/mcp/denim)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Denim** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `denim` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Denim** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "denim": {
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
