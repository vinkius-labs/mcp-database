# emfluence Marketing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emfluence-marketing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage marketing emails, track contact groups, and monitor performance via the emfluence API.

## Description
Integrate **emfluence**, the intuitive marketing automation platform, directly into your AI workflow. Manage your marketing emails and contact groups, track individual subscriber profiles, monitor real-time email performance statistics, and oversee your automated marketing operations using natural language.

### What you can do

- **Email Oversight** — List and retrieve detailed information, subject lines, and content for all your marketing emails.
- **Contact Intelligence** — Monitor contact groups and individual profiles, resolving subscription statuses and custom field values.
- **Performance Monitoring** — Access real-time email telemetry, resolving sent, open, click, and bounce metrics via chat.
- **Marketing Auditing** — Retrieve high-level summaries of group volumes, email activity, and organizational marketing health instantly.

### How it works

1. Connect the emfluence integration to your AI assistant.
2. Authorize using your emfluence API Key (found in your account settings).
3. Orchestrate your marketing automation and subscriber management through intuitive conversation.

### Who is this for?

- **Email Marketers** — Quickly check email open rates and group subscriber counts on the go.
- **Campaign Managers** — Research contact profiles and target groups via chat during planning.
- **Operations Teams** — Monitor marketing volumes and organizational emfluence metadata instantly.


## Available Tools (10)
- **get_email_performance_stats**: Get performance statistics for a specific marketing email
- **get_contact_profile**: Get full profile and history for a specific contact
- **get_email_details**: Get detailed settings and content for a specific marketing email
- **get_group_details**: Get detailed settings and counts for a specific contact group
- **quick_marketing_volume_audit**: Retrieve a high-level summary of email and group activity
- **list_contact_target_groups**: List all contact groups (lists) configured in your account
- **list_marketing_contacts**: List all contacts registered in your organization
- **list_marketing_emails**: List all marketing emails in your emfluence account
- **search_contacts_by_email**: Search for a contact using their email address
- **get_emfluence_account_metadata**: Retrieve metadata and settings for your emfluence account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **emfluence Marketing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my contact target groups."

**🤖 AI Agent:**
> I've found 4 groups, including 'VIP Customers' (1,250 members) and 'Lead Gen List' (3,400 members). Would you like to see the detailed settings for VIP Customers?

---

**👤 You:**
> "Show me the performance stats for email ID 12345."

**🤖 AI Agent:**
> Email ID 12345 ('March Newsletter') has been sent to 3,400 recipients. Performance: 850 opens (25%), 240 clicks (7.1%), and 15 bounces. Status is 'Sent'. Should I check the click breakdown?

---

**👤 You:**
> "Search for contact 'alex@example.com'."

**🤖 AI Agent:**
> Alex is a member of the 'Lead Gen' group and is currently 'Active'. Their last recorded activity was a click on March 15th. Should I pull their full custom field history?


## ❓ FAQ

**Q: How do I get an emfluence API Key?**
Log in to your emfluence account, navigate to **Settings > API**, and you can generate or retrieve your unique API Key from there. Ensure the key has the necessary permissions for your marketing resources.

**Q: Can the agent send new marketing emails?**
This integration currently focuses on listing and auditing emails, groups, and contacts. Creating or sending new marketing campaigns should be managed via the emfluence platform dashboard.

**Q: Does the integration show bounce rates?**
Yes, you can use the get_email_performance_stats tool to retrieve specific bounce metrics along with open and click rates for any email.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emfluence-marketing](https://vinkius.com/mcp/emfluence-marketing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **emfluence Marketing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emfluence-marketing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **emfluence Marketing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emfluence-marketing": {
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
