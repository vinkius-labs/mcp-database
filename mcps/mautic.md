# Mautic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mautic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Open-source marketing automation via Mautic — manage contacts, campaigns, and emails.

## Description
Connect your **Mautic** marketing automation instance to any AI agent and take full control of your marketing workflows through natural conversation.

### What you can do

- **Contact Management** — Search for contacts, fetch detailed profiles, and create new records on the fly
- **Campaign Tracking** — List and inspect marketing automation campaigns and their configurations
- **Email Marketing** — Manage email templates and retrieve details for specific marketing emails
- **Audience Segmentation** — List contact segments and add contacts to specific lists for targeted marketing
- **Company Data** — Manage company (account) records and their associations within Mautic

### How it works

1. Subscribe to this server
2. Enter your Mautic Base URL, Username, and Password (or API secret)
3. Start managing your marketing automation from Claude, Cursor, or any MCP-compatible client


## Available Tools (11)
- **get_company**: Get company details by ID
- **get_contact**: Get a specific contact by ID
- **get_email**: Get email details by ID
- **list_companies**: List all companies
- **list_contacts**: Supports an optional search query.

List or search contacts
- **list_emails**: List all email templates
- **list_segments**: List all contact segments
- **add_contact_to_segment**: Add a contact to a segment
- **create_contact**: Create a new contact
- **get_campaign**: Get campaign details by ID
- **list_campaigns**: List all campaigns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mautic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find contact info for john.doe@example.com in Mautic."

**🤖 AI Agent:**
> Searching Mautic... I found John Doe (ID: 1234). He is currently in the 'Active Leads' segment.

---

**👤 You:**
> "List all active marketing campaigns."

**🤖 AI Agent:**
> Retrieving campaigns... You have 3 active campaigns: 'Summer Promo', 'Onboarding', and 'Re-engagement'.

---

**👤 You:**
> "Add contact ID 1234 to segment ID 5."

**🤖 AI Agent:**
> Action complete. Contact 1234 has been successfully added to segment 5 ('High Value Customers').


## ❓ FAQ

**Q: How do I enable the Mautic API?**
Go to Mautic Settings > Configuration > API Settings and set 'API Enabled?' to 'Yes'. Also enable 'HTTP Basic Auth' for this integration.

**Q: Can I search for contacts by email?**
Yes! Use the `list_contacts` tool and provide the email address in the search parameter.

**Q: Is my Mautic data secure?**
Absolutely. Your credentials are encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mautic](https://vinkius.com/mcp/mautic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mautic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mautic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mautic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mautic": {
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
