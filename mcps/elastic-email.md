# Elastic Email MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elastic-email)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Equip your AI agent to manage email campaigns, track contacts, and monitor delivery logs via the Elastic Email API.

## Description
Integrate **Elastic Email**, the powerful email marketing and delivery platform, directly into your AI workflow. Manage your email campaigns and templates, track contact lists and individual profiles, monitor real-time delivery logs and statuses, and oversee your marketing operations using natural language.

### What you can do

- **Campaign Oversight** — List and retrieve detailed information and performance metrics for all your email marketing campaigns.
- **Contact Intelligence** — Monitor contact address lists, individual profile details, and subscription statuses across your organization.
- **Delivery Monitoring** — Track real-time email delivery logs, identifying success rates and recipient timestamps via chat.
- **Marketing Auditing** — Retrieve high-level summaries of list volumes, campaign activity, and account credit balances instantly.

### How it works

1. Connect the Elastic Email integration to your AI assistant.
2. Authorize using your Elastic Email API Key (found in your account settings).
3. Orchestrate your email marketing and contact management through intuitive conversation.

### Who is this for?

- **Email Marketers** — Quickly check campaign open rates and delivery logs on the go.
- **CRM Managers** — Research contact profiles and list memberships via chat during segmentation.
- **Operations Teams** — Monitor credit balances and organizational marketing metadata instantly.


## Available Tools (10)
- **get_elastic_email_metadata**: Retrieve metadata and usage limits for your Elastic Email account
- **get_campaign_performance**: Get detailed performance metrics for a specific email campaign
- **get_contact_profile**: Get full profile and history for a specific contact by email
- **quick_marketing_volume_audit**: Retrieve a high-level summary of campaign activity and contact counts
- **list_contact_address_lists**: List all contact lists configured in your account
- **list_marketing_campaigns**: List all email marketing campaigns in your Elastic Email account
- **list_marketing_contacts**: List all contacts registered in your organization
- **list_delivery_logs**: List recent email delivery logs and statuses
- **list_email_designs**: List all available email message templates and designs
- **search_contacts_by_email**: Search for a contact using their email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elastic Email** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns."

**🤖 AI Agent:**
> I've found several campaigns, including 'Spring Sale 2024' and 'Monthly Newsletter'. Both are currently 'Sending'. Would you like to see the performance metrics for the Spring Sale?

---

**👤 You:**
> "Show me the delivery logs for today."

**🤖 AI Agent:**
> I've retrieved today's logs. Out of 500 emails sent, 485 were 'Delivered' and 15 are 'Pending'. Would you like a list of the recipient addresses for the pending emails?

---

**👤 You:**
> "Search for contact 'john.doe@example.com'."

**🤖 AI Agent:**
> John Doe is a member of the 'Master List' and is currently 'Opted In'. Their last interaction was on March 15th. Should I pull their complete interaction history?


## ❓ FAQ

**Q: How do I get an Elastic Email API Key?**
Log in to your Elastic Email dashboard, navigate to **Settings > API**, and you can generate or retrieve your unique API Key from there. Ensure the key has the necessary permissions for campaigns and contacts.

**Q: Can the agent send new email broadcasts?**
This integration currently focuses on listing and auditing campaigns, lists, and contacts. Scheduling or sending actual email broadcasts should be managed via the Elastic Email campaign builder or SMTP interface.

**Q: Does the integration show real-time delivery status?**
Yes, you can use the list_delivery_logs tool to retrieve the latest transmission events and statuses as reported by the Elastic Email platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elastic-email](https://vinkius.com/mcp/elastic-email)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elastic Email** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `elastic-email` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elastic Email** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elastic-email": {
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
