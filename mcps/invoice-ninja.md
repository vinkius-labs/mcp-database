# Invoice Ninja MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/invoice-ninja)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage clients, invoices, and products directly through AI.

## Description
### What you can do
- **List and retrieve clients:** Instantly access client details, contacts, and custom fields.
- **Create and manage invoices:** Generate invoices, fetch specific invoice details, and streamline your billing process.
- **Handle products and payments:** Track your products, record payments, and manage financial operations seamlessly via AI.

### How it works
1. Sign up for Invoice Ninja or use your self-hosted instance.
2. Generate an API Token in Settings > Advanced Settings > API Tokens.
3. Enter the token (and optional custom Base URL) in the agent setup, and start managing your billing operations.

### Who is it for?
Freelancers, small businesses, and agencies who need a powerful, automated way to handle invoicing and client management directly from their AI assistant.


## Available Tools (11)
- **create_client**: Create a new client
- **create_invoice**: Create a new invoice
- **create_product**: Create a new product
- **get_client**: Get details for a specific client
- **get_invoice**: Get an invoice by ID
- **get_payment**: Get a payment by ID
- **get_product**: Get a product by ID
- **list_clients**: List clients in Invoice Ninja
- **list_invoices**: List invoices
- **list_payments**: List payments
- **list_products**: List products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Invoice Ninja** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my latest clients."

**🤖 AI Agent:**
> I've fetched your clients. You have Acme Corp, Globex, and Initech.

---

**👤 You:**
> "Create a new product called 'Consulting Hours' with a price of 150."

**🤖 AI Agent:**
> The product 'Consulting Hours' has been successfully created with a price of 150.

---

**👤 You:**
> "Get the details for invoice ID 12345."

**🤖 AI Agent:**
> Invoice 12345 is for $500, assigned to Acme Corp, and is currently marked as 'Sent'.


## ❓ FAQ

**Q: Can I use this with a self-hosted Invoice Ninja instance?**
Yes! You can provide a custom Base URL in the authentication settings to connect to your own server.

**Q: Does the AI Agent handle recurring invoices?**
Currently, the agent focuses on creating and fetching standard invoices, clients, products, and payments. You can use the Invoice Ninja dashboard for recurring settings.

**Q: Can I process credit card payments through this agent?**
No, the agent can list and retrieve payment records, but it does not act as a payment gateway to process actual credit card transactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/invoice-ninja](https://vinkius.com/mcp/invoice-ninja)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Invoice Ninja** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `invoice-ninja` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Invoice Ninja** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "invoice-ninja": {
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
