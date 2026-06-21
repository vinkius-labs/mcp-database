# Wuro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wuro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your business billing, product catalog, and contacts with Wuro.fr through AI.

## Description
Connect your **Wuro.fr** account to any AI agent to automate your business billing and CRM workflows. Manage invoices, quotes, and your customer database through natural conversation.

### What you can do

- **Billing Automation** — Create and manage customer invoices (Factures) and professional quotes (Devis) directly from the AI interface.
- **CRM & Contacts** — Track and manage your database of clients, leads, and suppliers with detailed metadata for each business resource.
- **Catalog Control** — Access and monitor your product catalog and pricing information to streamline sales operations.
- **Expense Monitoring** — Track company purchases and supplier expenses to maintain a clear overview of your firm's finances.
- **HR Management** — Manage firm employee records and leave requests programmatically via natural language commands.
- **Operational Integrity** — Secure authentication using HMAC-SHA1 signatures based on your private API key.

### How it works

1. Subscribe to this server
2. Enter your Wuro Public and Private API Keys from your account settings
3. Start managing your billing and CRM from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **French Businesses** — entrepreneurs and SMEs using Wuro to centralize their administrative tasks.
- **Accountants** — quickly retrieve latest invoices and quote statuses without manual exports.
- **Administrative Managers** — streamline contact management and employee leave requests via natural language.


## Available Tools
- **create_contact**: Create a new contact
- **create_invoice**: Provide contact ID and lines.

Create a new customer invoice
- **create_quote**: Provide contact ID and lines.

Create a new quote/estimate
- **get_contact**: Get details of a specific contact
- **get_invoice**: Get details of a specific invoice
- **get_quote**: Get details of a specific quote
- **list_contacts**: List all contacts
- **list_employees**: List all employees
- **list_invoices**: List all customer invoices
- **list_products**: List all products
- **list_purchases**: List all company purchases
- **list_quotes**: List all quotes/estimates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wuro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent invoices in Wuro."

**🤖 AI Agent:**
> I've retrieved your latest invoices. The most recent is Invoice #F-2024-001 (Total: €1,250.00, Status: Paid). Would you like the details for any other record?

---

**👤 You:**
> "Create a new contact 'Jean Dupont' with email jean@example.com."

**🤖 AI Agent:**
> Successfully created the contact 'Jean Dupont' in Wuro. He has been added to your database as a new client prospect. Would you like to create a quote for him?


## ❓ FAQ

**Q: How do I obtain my Public and Private API Keys?**
Log in to your Wuro account, navigate to **Paramètres** (Settings) > **Intégration** > **API REST**, and generate your set of keys there.

**Q: Is the connection secure?**
Yes. The integration uses HMAC-SHA1 signatures to authenticate every request, ensuring that your Private API Key is used to sign requests without being transmitted directly in every header.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wuro](https://vinkius.com/mcp/wuro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wuro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wuro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wuro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wuro": {
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
