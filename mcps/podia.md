# Podia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/podia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your Podia store — list customers, track sales, and oversee products and subscriptions directly from any AI agent.

## Description
Connect your **Podia** account to any AI agent to streamline your digital storefront management. This server allows you to handle customers, products, and sales data through natural conversation.

### What you can do

- **Customer Management** — List all customers, fetch specific profiles, or create and update customer records instantly.
- **Product Insights** — Retrieve lists of your digital products, courses, and webinars, including deep dives into specific product metadata.
- **Sales & Revenue Tracking** — Monitor your transactions by listing all sales or inspecting individual sale details.
- **Memberships & Subscriptions** — Access your membership plans and track active subscriptions to understand your recurring revenue.

### How it works

1. Subscribe to this server
2. Enter your Podia API Key
3. Start managing your digital business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Course Creators** — quickly check who recently joined a course or update student information without leaving your workflow.
- **Digital Entrepreneurs** — monitor sales performance and product availability through simple voice or text queries.
- **Support Teams** — look up customer details and subscription statuses to provide faster assistance.


## Available Tools
- **create_customer**: Create a new Podia customer
- **get_customer**: Get details for a specific Podia customer
- **get_product**: Get details for a specific Podia product
- **get_sale**: Get details for a specific Podia sale
- **list_customers**: List Podia customers
- **list_plans**: List Podia membership plans
- **list_products**: List Podia products
- **list_sales**: List Podia sales
- **list_subscriptions**: List Podia subscriptions
- **update_customer**: Update an existing Podia customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Podia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Podia customers and show their emails."

**🤖 AI Agent:**
> I've retrieved your customer list. You have 150 customers. Some recent ones include: 'Alice Smith (alice@example.com)' and 'Bob Jones (bob@example.com)'. Would you like details on a specific customer?

---

**👤 You:**
> "What are the details for product ID 98765?"

**🤖 AI Agent:**
> Inspecting product 98765... This is your 'Mastering MCP' course. It is currently active, priced at $99, and has 45 enrolled students.

---

**👤 You:**
> "Show me my membership plans and active subscriptions."

**🤖 AI Agent:**
> I've fetched your membership data. You have 3 plans: 'Basic', 'Pro', and 'Elite'. There are currently 12 active subscriptions across these plans.


## ❓ FAQ

**Q: Can I update a customer's email or name directly through the AI?**
Yes, you can use the `update_customer` tool. Just provide the Customer ID and the new details you wish to change, and the agent will process the update in your Podia account.

**Q: How do I see a list of all my digital products and courses?**
Simply ask the agent to run the `list_products` tool. It will return a comprehensive list of your available products, courses, and webinars hosted on Podia.

**Q: Can I track my recent sales and transaction details?**
Absolutely. Use `list_sales` to see recent transactions or `get_sale` with a specific ID to inspect the financial details of a particular purchase.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/podia](https://vinkius.com/mcp/podia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Podia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `podia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Podia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "podia": {
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
