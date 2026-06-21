# Keap MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keap)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage CRM contacts, marketing campaigns, and sales automation via Keap.

## Description
Connect your **Keap** (formerly Infusionsoft) account to any AI agent to optimize your CRM and sales workflows. This MCP server enables your agent to interact with contacts, tags, and automation campaigns directly from natural language interfaces.

### What you can do

- **Contact Management** — List, retrieve, and create contact profiles to maintain your lead database
- **Marketing Automation** — List and monitor active campaigns and automation sequences
- **Segmentation** — Manage tags and apply them to contacts to trigger specific workflows
- **Sales Pipeline** — Query opportunities and deals to track your revenue growth
- **Billing Visibility** — Access invoices and orders to stay on top of customer transactions

### How it works

1. Subscribe to this server
2. Enter your Keap Personal Access Token (PAT)
3. Start managing your CRM and marketing from Claude, Cursor, or any MCP client

### Who is this for?

- **Small Business Owners** — Automate lead follow-ups and contact updates via simple commands
- **Marketing Managers** — Monitor campaign performance and segment audiences on the fly
- **Sales Professionals** — Quickly retrieve contact history and update deal statuses during client interactions


## Available Tools (11)
- **apply_tag_to_contact**: Apply a tag to a specific contact
- **list_campaigns**: List all marketing campaigns
- **list_contacts**: Use this to search for leads or customers.

List all contacts in Keap
- **create_contact**: Requires at least a first name or email.

Create a new contact in Keap
- **get_contact**: Get details for a specific contact
- **list_invoices**: List all invoices
- **list_opportunities**: List sales opportunities
- **list_orders**: List ecommerce orders
- **get_business_profile**: Get Keap business profile information
- **list_tags**: List all available tags
- **list_users**: List all application users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Keap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find a contact with email 'john@example.com' in Keap."

**🤖 AI Agent:**
> I've searched your Keap contacts and found 'John Doe' (ID: 12345). Would you like to see his full profile or recent activity?

---

**👤 You:**
> "Show me all my available tags in Keap."

**🤖 AI Agent:**
> I've retrieved 25 tags from your account, including 'New Lead', 'Customer-Tier-1', and 'Webinar-Registered'.

---

**👤 You:**
> "List my recent ecommerce orders."

**🤖 AI Agent:**
> I found 5 recent orders. The latest is Order #9876 for $150.00 from 'Jane Smith', currently marked as 'Paid'.


## ❓ FAQ

**Q: How do I apply a tag to a contact using the agent?**
Use the `apply_tag_to_contact` tool with the specific `tag_id` and `contact_id`. This is great for manual segmentation during a conversation.

**Q: Can I see all my automation campaigns?**
Yes, the `list_campaigns` tool retrieves all campaigns configured in your Keap account, allowing you to monitor active sequences.

**Q: Is it possible to query sales opportunities?**
Absolutely. Use the `list_opportunities` tool to see your current sales pipeline and track potential deals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keap](https://vinkius.com/mcp/keap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Keap** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keap` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Keap** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keap": {
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
