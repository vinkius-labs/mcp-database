# Paperless Parts MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paperless-parts)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Quote custom manufacturing jobs faster with automated pricing, 3D model analysis, and quoting workflows for machine shops.

## Description
Connect your **Paperless Parts** manufacturing platform to any AI agent and take full control of your quoting, order management, and customer accounts through natural conversation.

### What you can do

- **Quotes & Orders** — List all manufacturing quotes, fetch specific order details, and instantly change quote statuses directly from your agent
- **Account Management** — Query the complete customer directory, create new buyer accounts on the fly, and verify CRM metadata
- **Contact Directory** — Retrieve detailed contact profiles and establish new communication channels to streamline sales
- **Custom Tables** — Access and list specialized custom tables used in your distinct manufacturing routing process

### How it works

1. Subscribe to this server
2. Enter your Paperless Parts API Token
3. Start managing your entire manufacturing pipeline from Claude, Cursor, or any MCP-compatible client

No more wrestling with multiple browser windows to verify an order's status. Your AI acts as a dedicated production manager.

### Who is this for?

- **Estimators & Quoting Engineers** — instantly retrieve quote calculations, list stale quotes, and update status parameters without leaving your workflow
- **Shop Floor Managers** — check order requirements and metadata straight from your daily dashboard
- **Sales & Operations Leads** — automate CRM inquiries and quickly register new contacts and customer accounts to close deals faster


## Available Tools
- **create_account**: Requires a JSON string containing the account details.

Create a new account
- **create_contact**: Requires a JSON string containing the contact details.

Create a new contact
- **get_account**: Get a specific account by ID
- **get_contact**: Get a specific contact by ID
- **get_order**: Get a specific order by ID
- **get_quote**: Get a specific quote by ID
- **list_accounts**: List accounts from Paperless Parts
- **list_contacts**: List contacts from Paperless Parts
- **list_custom_tables**: List custom tables from Paperless Parts
- **list_orders**: List orders from Paperless Parts
- **list_quotes**: List quotes from Paperless Parts
- **update_quote_status**: Update the status of a specific quote


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paperless Parts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our active manufacturing orders on Paperless Parts."

**🤖 AI Agent:**
> I've fetched your environments. You currently have several ongoing orders including 'Aerospace Bracket Q3' (ID: ORD-934) and 'CNC Panel Batch' (ID: ORD-021). Which order would you like to drill into?

---

**👤 You:**
> "Can you update the status of quote QTE-1205934 to 'Approved'?"

**🤖 AI Agent:**
> Executing the status change logic... Quote QTE-1205934 has been successfully marked as 'Approved' and locked into your main production pipeline.

---

**👤 You:**
> "Provide the details and metadata for account ID 120394."

**🤖 AI Agent:**
> Let's inspect it... Account 'Northwest Defense Systems' is categorized as a primary supplier. Their active billing cycle is set to Net 30, and the primary contact is marked as Amanda T.


## ❓ FAQ

**Q: Can my AI automatically find the details of a specific order just by providing the Order ID?**
Yes! Use the `get_order` tool with exactly the Order ID. Your agent will respond with complete metadata and the precise operational notes connected to that order in seconds.

**Q: How do I update the status of a quote during my workflow?**
Simply ask the agent to run the `update_quote_status` action on the target Quote ID and specify the new status. The platform will automatically register the change.

**Q: Does the integration permit creating new customer accounts?**
Yes. The tools include `create_account` and `create_contact` operations, empowering your agent to expand your CRM pipeline dynamically without ever opening the web application.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paperless-parts](https://vinkius.com/mcp/paperless-parts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paperless Parts** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `paperless-parts` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paperless Parts** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paperless-parts": {
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
