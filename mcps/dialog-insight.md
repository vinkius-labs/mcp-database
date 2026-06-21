# Dialog Insight MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dialog-insight)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage marketing contacts, track campaigns, and monitor engagement via the Dialog Insight API.

## Description
Integrate **Dialog Insight**, the powerful relationship marketing and CRM platform, directly into your AI workflow. Manage your marketing contacts, monitor email and SMS campaign performance, and track automated workflows using natural language.

### What you can do

- **Contact Intelligence** — List and retrieve detailed profiles for your marketing contacts and their subscription preferences.
- **Campaign Performance** — Monitor real-time analytics for email and SMS campaigns, including open and click rates.
- **Automation Oversight** — Track active marketing automation workflows and customer journeys.
- **Audience Segmentation** — List configured audience segments and identify estimated member counts.

### How it works

1. Connect the Dialog Insight integration to your AI assistant.
2. Authorize using your Dialog Insight API Key and Account ID.
3. Orchestrate your relationship marketing and CRM through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check campaign results and audience sizes on the go.
- **CRM Specialists** — Research contact profiles and interaction history via chat.
- **Digital Marketers** — Monitor automated journeys and campaign delivery during planning.


## Available Tools
- **add_new_marketing_contact**: Add a new contact record to the Dialog Insight database
- **get_account_metadata**: Retrieve settings and limits for your Dialog Insight account
- **get_campaign_performance**: Get detailed performance metrics for a specific campaign
- **get_contact_profile**: Get detailed profile and history for a specific contact
- **list_active_automations**: List active marketing automation workflows
- **list_marketing_campaigns**: List all email and SMS marketing campaigns
- **list_marketing_contacts**: List all contacts in your Dialog Insight organization
- **list_audience_segments**: List all configured audience segments for targeting
- **list_high_performing_campaigns**: Identify campaigns with the highest engagement rates (mock logic)
- **search_contacts_by_email**: Search for a contact record by their email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dialog Insight** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns."

**🤖 AI Agent:**
> I've found 4 active campaigns, including 'Spring Promotion 2024' and 'Monthly Newsletter'. Would you like to see the performance metrics for the largest one?

---

**👤 You:**
> "Show me the performance for campaign 'Spring Promotion'."

**🤖 AI Agent:**
> The 'Spring Promotion' campaign has an open rate of 22% and a click-through rate of 3.5%. So far, it has generated 1,200 unique clicks. Should I list the top performing links?

---

**👤 You:**
> "Find contact profile for 'user@example.com'."

**🤖 AI Agent:**
> I've retrieved the profile for 'user@example.com'. They are currently 'Active' and part of the 'VIP Customers' segment. Their last interaction was with the 'June Digest' email. Would you like to see their custom field values?


## ❓ FAQ

**Q: How do I get Dialog Insight API credentials?**
Log in to your Dialog Insight account, navigate to **Configuration > API**, and you will find your API Key (AuthKey) and Account ID (idAccount) there.

**Q: Can the agent see real-time campaign engagement?**
Yes, you can use the get_campaign_performance tool to retrieve the latest reported metrics for any of your active email or SMS campaigns.

**Q: Does the integration support segment searching?**
Yes, you can list all configured audience segments, allowing the agent to provide information on segment definitions and sizes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dialog-insight](https://vinkius.com/mcp/dialog-insight)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dialog Insight** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dialog-insight` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dialog Insight** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dialog-insight": {
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
