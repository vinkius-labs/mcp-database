# Elastic Path MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elastic-path)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage headless commerce workflows via Elastic Path — inspect carts, track purchases, and retrieve store navigation directly from any AI agent.

## Description
Connect your **Elastic Path** commerce engine to any AI agent to streamline your headless commerce operations through natural language.

### What you can do

- **Cart & Profile Management** — Access default carts and user profiles for specific store scopes to understand customer context.
- **Order Tracking** — Retrieve detailed purchase information, including status (COMPLETE/FAILED), totals, and line items using specific IDs.
- **Store Discovery** — Fetch navigation entry points, search configurations, and supported country lists for your storefront.
- **Account Services** — Access registration forms and account-specific metadata to manage user lifecycles.
- **Deep Data Inspection** — Use zoom and format parameters to retrieve linked data and specific response formats directly from the Cortex API.

### How it works

1. Subscribe to this server
2. Enter your Elastic Path Cortex URL and Access Token
3. Start managing your commerce workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — quickly check order statuses and store configurations without logging into multiple dashboards.
- **Developers** — test API responses and inspect cart/navigation structures directly from the code editor.
- **Support Teams** — retrieve account and purchase details instantly to resolve customer inquiries faster.


## Available Tools (9)
- **create_token**: Authenticate and create an OAuth2 token
- **get_searches**: Get searches entry point for a scope
- **get_account**: Read a specific account
- **get_countries**: Get geographies/countries for a scope
- **get_default_cart**: Read the default cart for a scope
- **get_default_profile**: Read the default profile for a scope
- **get_navigations**: Get navigations entry point for a scope
- **get_purchase**: Returns status (COMPLETE, FAILED), totals, and line items.

Read a specific purchase
- **get_registration_form**: Get account registration form for a scope


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elastic Path** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the default cart for the 'mobee' scope."

**🤖 AI Agent:**
> I've retrieved the default cart for 'mobee'. It currently contains 3 items with a total value of $145.00. Would you like to see the specific line items?

---

**👤 You:**
> "What is the status of purchase ID '12345' in the 'mobee' scope?"

**🤖 AI Agent:**
> The purchase '12345' is marked as 'COMPLETE'. The transaction was finalized on Oct 24th for a total of $89.99.

---

**👤 You:**
> "List the available countries for our store scope."

**🤖 AI Agent:**
> I've fetched the supported geographies. Your store currently supports shipping and billing in 5 countries: USA, Canada, UK, Germany, and France.


## ❓ FAQ

**Q: Can I check the status of a specific purchase using its ID?**
Yes! Use the `get_purchase` tool with the store scope and purchase ID. It will return the status (such as COMPLETE or FAILED), order totals, and a list of items.

**Q: How do I retrieve the navigation structure for my storefront?**
Simply use the `get_navigations` tool providing your store scope. This will fetch the entry points for your store's categories and links.

**Q: Is it possible to see the default cart for a specific scope?**
Yes, the `get_default_cart` tool allows you to read the default cart for any specified scope, including optional zoom parameters for linked data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elastic-path](https://vinkius.com/mcp/elastic-path)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elastic Path** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `elastic-path` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elastic Path** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elastic-path": {
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
