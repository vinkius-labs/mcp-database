# Holded MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/holded)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate business management via Holded — manage invoices, contacts, and projects directly from any AI agent.

## Description
Connect your **Holded** ERP platform to any AI agent and take full control of your invoicing, CRM, and project management through natural conversation.

### What you can do

- **Invoicing Oversight** — List all documents, retrieve detailed invoice data, and monitor payment statuses efficiently.
- **CRM & Contact Management** — Access lists of clients, suppliers, and leads, and retrieve full profile information for better relationship management.
- **Project & Task Tracking** — List active projects and monitor tasks across your entire portfolio to ensure deadlines are met.
- **Inventory & Products** — Access your product catalog and update stock levels directly from the chat interface.
- **Business Intelligence** — Retrieve account and organization metadata to maintain a high-level overview of your business operations.
- **Unified ERP** — Bridge the gap between your accounting and operations using the comprehensive Holded API.

### How it works

1. Subscribe to this server
2. Enter your Holded API Key (found in Settings > Developers)
3. Start managing your business from Claude, Cursor, or any MCP-compatible client

No more manual navigating through complex ERP modules for simple data lookups. Your AI assistant acts as a dedicated Business Operations Manager or Project Coordinator.

### Who is this for?

- **Business Owners** — instantly retrieve invoice statuses and company performance data.
- **Project Managers** — automate the oversight of tasks and project lifecycles across multiple teams.
- **Operations Leads** — maintain a real-time overview of inventory levels and customer contact data.


## Available Tools
- **get_contact_details**: Get detailed profile information for a specific contact
- **get_invoice_details**: Get detailed information about a specific invoice
- **get_api_profile**: Retrieve information about the authenticated account
- **get_product_details**: Get detailed information for a specific product
- **get_project_details**: Get detailed configuration and status for a project
- **list_contacts**: Useful for finding the contact ID required for documents.

List all contacts (clients, suppliers, leads) in Holded
- **list_invoices**: Use this to monitor billing and find IDs for specific document actions.

List all invoices in your Holded account
- **list_products**: List all products and services in your Holded inventory
- **list_projects**: List all active and past projects
- **list_all_tasks**: List tasks across all projects
- **update_product_stock**: Pass details as a JSON string in "body_json" (requires warehouseId and new quantity).

Update the stock level for a specific product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Holded** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects and show the last task for each."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active workflows: 'Website Launch' (ID: proj_102), 'Q2 Campaign', and 'Product Beta'. For the Website Launch, the latest task is 'Final QA Check' (ID: task_992). Would you like to see the details for any of these?

---

**👤 You:**
> "Find contact 'Acme Corp' and show their recent invoices."

**🤖 AI Agent:**
> I've found Acme Corp (ID: contact_552). They have 2 recent invoices: INV-2024-01 ($1,250.00 - Paid) and INV-2024-05 ($3,000.00 - Pending). Would you like to see the items included in the pending invoice?

---

**👤 You:**
> "Show me the details for product ID 'prod_992' and its stock level."

**🤖 AI Agent:**
> Accessing inventory... Product 'prod_992' (Wireless Mouse) currently has 45 units in stock across 2 warehouses. The main warehouse has 30 units and the secondary has 15. Should I update the stock level for any specific location?


## ❓ FAQ

**Q: How do I find my Holded API Key?**
Log in to your Holded account, click on the **Settings** icon (top right), go to **Developers**, and you will find your unique **API Key** listed there. You can create multiple keys for different integrations.

**Q: What document types are supported in the invoicing tools?**
This integration currently focuses on the `invoice` document type. For other types like sales orders or purchase orders, you can use the generic `list_invoices` logic if they are mapped under the same module in your instance.

**Q: Can I update stock levels through this integration?**
Yes! Use the `update_product_stock` tool. You must provide the product ID and a JSON string containing the warehouse ID and the new quantity to update your inventory.

**Q: Is the integration secure for ERP data?**
Absolutely. The integration uses official Holded API keys in the request header over HTTPS. Your credentials and business data are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/holded](https://vinkius.com/mcp/holded)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Holded** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `holded` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Holded** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "holded": {
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
