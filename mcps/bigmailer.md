# BigMailer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bigmailer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing via BigMailer — list brands, contacts, and campaigns directly from any AI agent.

## Description
Connect your **BigMailer** account to any AI agent and orchestrate your email marketing workflows across multiple brands through natural conversation.

### What you can do

- **Brand Management** — List and retrieve details for all brands managed within your BigMailer account.
- **Contact & List Oversight** — Manage your mailing lists and add or update contacts instantly.
- **Bulk Campaign Tracking** — List and inspect all bulk email campaigns to monitor your marketing reach.
- **Template Discovery** — Access and list your saved email templates for consistent brand messaging.
- **Property Management** — Retrieve custom brand properties and merge tags for personalized campaigns.
- **Performance Auditing** — Get detailed status updates for your outgoing marketing efforts.

### How it works

1. Subscribe to this server
2. Enter your BigMailer API Key
3. Start managing your multi-brand marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agency Owners** — manage multiple client brands and lists from a single interface.
- **Marketing Teams** — quickly check campaign statuses and add new subscribers straight from their workflow.
- **Growth Managers** — automate list management and brand auditing using natural language.


## Available Tools (10)
- **add_contact**: Add or update a contact in a brand
- **get_brand_properties**: List custom properties for a brand
- **get_brand**: Get specific brand details
- **get_bulk_campaign**: Get specific bulk campaign details
- **get_contact_list**: Get specific contact list details
- **list_brands**: List all brands in the account
- **list_bulk_campaigns**: List bulk campaigns for a brand
- **list_contact_lists**: List contact lists for a brand
- **list_contacts**: List contacts for a brand
- **list_templates**: List email templates for a brand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BigMailer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all brands in my BigMailer account."

**🤖 AI Agent:**
> I've retrieved your brands. You currently manage 2 brands: 'Tech Gadgets' (ID: b_123) and 'Fitness Pro' (ID: b_456). Which one would you like to manage?

---

**👤 You:**
> "Add a new contact to brand b_123: alice@example.com, Alice Smith."

**🤖 AI Agent:**
> I've successfully added 'Alice Smith' (alice@example.com) as a contact for your 'Tech Gadgets' brand.

---

**👤 You:**
> "Show my recent bulk campaigns for brand b_456."

**🤖 AI Agent:**
> Retrieving bulk campaigns for 'Fitness Pro'... I found 3 recent campaigns, including 'New Year Sale' and 'Weekly Newsletter'. Would you like the full details for any of these?


## ❓ FAQ

**Q: Can I add a new contact to a specific brand using the agent?**
Yes! Use the `add_contact` action with the Brand ID and contact details. Your agent will register or update the subscriber in BigMailer instantly.

**Q: How do I list all the email lists for a particular brand?**
Simply ask the agent to `list_contact_lists` and provide the Brand ID. It will retrieve all the mailing lists associated with that brand.

**Q: Does the integration allow me to see the statistics of my bulk campaigns?**
Yes. Use the `get_bulk_campaign` tool with the Brand ID and Campaign ID to retrieve performance data and metadata for your marketing efforts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bigmailer](https://vinkius.com/mcp/bigmailer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BigMailer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bigmailer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BigMailer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bigmailer": {
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
