# Holded MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/holded-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Run your business in Spain and Latin America with invoicing, accounting, CRM, and inventory that speaks your language natively.

## Description
Connect your **Holded** account to any AI agent and take full control of your business operations and ERP workflows through natural conversation.

### What you can do

- **Sales Lifecycle** — Manage everything from quotes and sales orders to invoices and credit notes programmatically
- **Purchase Tracking** — Monitor supplier relationships and manage purchase orders and invoices with ease
- **CRM & Contacts** — Organize your customer base, inventory products, and business expenses in one centralized hub
- **Treasury & Payments** — Monitor payments, treasury accounts, and financial health directly through your agent
- **Inventory Control** — List and manage products and stock levels to ensure your business never misses a beat

### How it works

1. Subscribe to this server
2. Generate an API Key in your Holded settings (Settings > Developers)
3. Start managing your business accounting and CRM from Claude, Cursor, or any MCP client

No more digging through complex ERP menus to find a customer balance or create a quick invoice. Your AI acts as your dedicated business administrator.

### Who is this for?

- **Small to Medium Businesses** — streamline daily operations and billing without manually entering every record
- **Accountants & Controllers** — quickly retrieve financial reports, unpaid invoices, and expense summaries
- **Operations Managers** — maintain inventory levels and manage supplier relationships through automated queries


## Available Tools (12)
- **create_invoice**: Requires contact ID and items.

Create a new invoice
- **list_contacts**: List CRM contacts
- **list_credit_notes**: List all credit notes
- **list_expenses**: List business expenses
- **list_invoices**: List all sales invoices
- **list_payments**: List recent payments
- **list_products**: List inventory products
- **list_purchase_invoices**: List purchase invoices
- **list_purchase_orders**: List purchase orders
- **list_quotes**: List all quotes
- **list_sales_orders**: List all sales orders
- **list_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Holded** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my unpaid sales invoices from Holded."

**🤖 AI Agent:**
> I've retrieved 8 unpaid invoices. The largest one is for 'Global Tech Solutions' (€1,200.00) and is 5 days overdue. Would you like to see the full list or the details for this specific invoice?

---

**👤 You:**
> "Create a new contact 'John Doe' as a lead with email 'john@example.com'."

**🤖 AI Agent:**
> Contact 'John Doe' has been successfully created as a Lead in your Holded CRM (ID: 654321). I've also mapped their email address. What's the next step for this lead?

---

**👤 You:**
> "Show me the last 5 business expenses."

**🤖 AI Agent:**
> Fetching recent expenses... Here are the last 5: 'Office Supplies' (€45.00), 'Software Subscription' (€29.99), 'Travel' (€120.00), 'Utilities' (€85.50), and 'Marketing' (€200.00). Total for these entries is €480.49.


## ❓ FAQ

**Q: Where do I find my API Key?**
You can generate your API key inside your Holded account under **Settings** > **Developers**.

**Q: Does the integration support inventory management?**
Yes, you can list and manage products, variants, and stock levels using the `list_products` and related tools.

**Q: Can I create invoices automatically with my AI agent?**
Yes, the server includes tools to create sales invoices, quotes, and credit notes by providing the necessary customer and item details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/holded-alternative](https://vinkius.com/mcp/holded-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `holded-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Holded** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "holded-alternative": {
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
