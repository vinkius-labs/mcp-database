# Ezus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ezus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Streamline travel agency operations via Ezus — manage projects, clients, suppliers, and invoices through your AI agent.

## Description
Connect your **Ezus** travel management account to any AI agent and take full control of your agency's workflows through natural conversation.

### What you can do

- **Project Management** — List, fetch, and upsert travel projects directly from the Ezus cloud
- **Client & Supplier CRM** — Query client details and manage your network of suppliers with ease
- **Product Catalog** — Access and inspect your travel products and packages stored in the Ezus catalog
- **Financial Overview** — List and inspect invoices to keep track of your agency's billing and financial status
- **User Profiling** — Retrieve the underlying credentials and profile information of your agent's API user

### How it works

1. Subscribe to this server
2. Enter your Ezus API Key, Email, and Password
3. Start managing your travel agency from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Agents** — quickly find project details or client info without leaving your communication tools
- **Agency Managers** — monitor billing and project status through simple natural language queries
- **Operations Teams** — sync project and supplier data directly within your AI-powered workflow


## Available Tools (12)
- **list_suppliers**: List all Ezus suppliers
- **get_project**: Get a specific Ezus project by ID
- **get_supplier**: Get a specific Ezus supplier by ID
- **list_clients**: List all Ezus clients
- **list_invoices**: List all Ezus invoices
- **list_products**: List all Ezus products
- **list_projects**: List all Ezus projects
- **upsert_project**: Create or update an Ezus project
- **get_client**: Get a specific Ezus client by ID
- **get_invoice**: Get a specific Ezus invoice by ID
- **get_me**: Get current Ezus user profile
- **get_product**: Get a specific Ezus product by ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ezus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent travel projects on Ezus."

**🤖 AI Agent:**
> I've retrieved your projects. You have 'Summer in Paris' (ID: 789) and 'Tokyo Explorer' (ID: 456) currently active. Would you like to see the details for any of these?

---

**👤 You:**
> "Show me the details for client ID 12345."

**🤖 AI Agent:**
> Inspecting client 12345... This is 'John Doe', a frequent traveler with a preference for luxury stays. They are currently associated with the 'Swiss Alps Adventure' project.

---

**👤 You:**
> "Get all products available in the catalog."

**🤖 AI Agent:**
> Fetching catalog... I found 12 products including 'Safari Package', 'Guided City Tour', and 'Airport Transfer'. Which one should I inspect further?


## ❓ FAQ

**Q: How do I obtain my Ezus API Key?**
You can find your API Key in the Ezus settings under the 'Integrations' or 'API' section. Note that a Premium plan may be required for private API access.

**Q: Can I update existing projects using this integration?**
Yes! Use the `upsert_project` tool. If you provide an existing Project ID, it will update the project; otherwise, it will create a new one.

**Q: Is it possible to list invoices to track payments?**
Absolutely. The `list_invoices` and `get_invoice` tools allow you to retrieve financial records and check their current status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ezus](https://vinkius.com/mcp/ezus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ezus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ezus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ezus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ezus": {
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
