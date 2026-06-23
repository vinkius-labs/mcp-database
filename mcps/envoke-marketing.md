# Envoke Marketing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/envoke-marketing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage email campaigns, track contact lists, and monitor performance via the Envoke API.

## Description
Integrate **Envoke**, the powerful and intuitive email marketing and communication platform, directly into your AI workflow. Manage your email campaigns and contact lists, track individual subscriber profiles and interaction history, monitor real-time performance statistics, and oversee your automated marketing operations using natural language.

### What you can do

- **Campaign Oversight** — List and retrieve detailed information, subject lines, and current statuses for all your email marketing campaigns.
- **Contact Intelligence** — Monitor contact address lists and individual profile details, resolving subscription statuses and custom field values.
- **Performance Monitoring** — Access real-time campaign telemetry, resolving sent, open, and click-through counts via chat.
- **Marketing Auditing** — Retrieve high-level summaries of list volumes, campaign activity, and organizational account health instantly.

### How it works

1. Connect the Envoke integration to your AI assistant.
2. Authorize using your Envoke API ID and API Key (found in your account settings).
3. Orchestrate your email marketing and subscriber management through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check campaign open rates and subscriber counts on the go.
- **Communication Specialists** — Research contact profiles and list memberships via chat during campaign planning.
- **Operations Teams** — Monitor marketing volumes and organizational Envoke metadata instantly.


## Available Tools (10)
- **get_envoke_account_metadata**: Retrieve metadata and limits for your Envoke account
- **get_campaign_performance_stats**: Get performance statistics for a specific email campaign
- **get_campaign_details**: Get detailed settings and status for a specific email campaign
- **get_contact_profile**: Get full profile and history for a specific contact
- **quick_marketing_volume_audit**: Retrieve a high-level summary of campaign activity and list counts
- **list_contact_address_lists**: List all contact lists configured in your account
- **list_email_campaigns**: List all email marketing campaigns in your Envoke account
- **list_marketing_contacts**: List all contacts registered in your organization
- **list_successfully_sent_campaigns**: Identify campaigns that have already been sent to subscribers
- **search_contacts_by_email**: Search for a contact using their email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Envoke Marketing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns."

**🤖 AI Agent:**
> I've found 5 active campaigns, including 'Monthly Newsletter' and 'Q2 Lead Magnet'. The Monthly Newsletter has already been sent to 3,500 contacts. Would you like to see the performance stats?

---

**👤 You:**
> "Show me the performance for campaign ID 12345."

**🤖 AI Agent:**
> Campaign ID 12345 has 3,500 sends, 850 opens (24.3%), and 240 clicks (6.8%). Status is 'Completed'. Should I check for any delivery bounces?

---

**👤 You:**
> "Search for contact 'alex@example.com'."

**🤖 AI Agent:**
> Alex is currently 'Subscribed' and a member of 2 lists: 'General Announcements' and 'Product Beta'. Their last recorded click was on March 15th. Should I pull their full interaction history?


## ❓ FAQ

**Q: How do I get Envoke API credentials?**
Log in to your Envoke account, navigate to **Settings > API Integration**, and you can find your unique **API ID** and **API Key** there. API access is typically included in professional and higher plans.

**Q: Can the agent send new mass emails?**
This integration currently focuses on listing and auditing campaigns, lists, and contacts. Creating or sending new mass emails should be managed via the Envoke platform dashboard or automated API triggers.

**Q: Does the integration show real-time stats?**
Yes, you can use the get_campaign_performance_stats tool to retrieve the latest sent, open, and click counts for any active campaign.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/envoke-marketing](https://vinkius.com/mcp/envoke-marketing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Envoke Marketing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `envoke-marketing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Envoke Marketing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "envoke-marketing": {
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
