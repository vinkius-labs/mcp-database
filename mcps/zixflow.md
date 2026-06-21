# Zixflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zixflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage sales collections, contacts, and transactions via the Zixflow API.

## Description
Connect your **Zixflow** workspace to any AI agent to automate your sales and CRM operations. This MCP server enables your agent to interact with collections (People, Company, etc.), manage individual records, and track wallet transactions directly from natural language.

### What you can do

- **Collection Oversight** — List all data collections configured in your workspace to understand your CRM structure
- **Contact Management** — List, retrieve, create, and update records within any collection using detailed field mappings
- **Precision Filtering** — Search for specific records using JSON-based filtering and sorting criteria
- **Cleanup Automation** — Delete unnecessary records and maintain your database directly via natural language commands
- **Wallet Tracking** — Access a history of transactions and balance changes within your Zixflow wallet

### How it works

1. Subscribe to this server
2. Enter your Zixflow API Token
3. Start managing your CRM and sales data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — Update lead statuses and company details instantly from your conversation interface
- **Growth Managers** — Automate the creation of new contact records and segment collections on the fly
- **Operations Teams** — Monitor wallet usage and maintain CRM hygiene via simple natural language instructions


## Available Tools (7)
- **list_collections**: List all collections (People, Company, etc.)
- **create_collection_record**: g., a person or company) to a specific Zixflow collection.

Create a new record in a collection
- **delete_collection_record**: Delete a record from a collection
- **get_record_details**: Get details for a specific record
- **list_collection_records**: Requires a JSON body for filtering/sorting.

List records within a specific collection
- **list_wallet_transactions**: List Zixflow wallet transactions
- **update_collection_record**: Update an existing record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zixflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all data collections in my Zixflow workspace."

**🤖 AI Agent:**
> I've retrieved your collections. You have 2 main collections: 'People' (ID: 123) and 'Company' (ID: 456). Which one would you like to explore?

---

**👤 You:**
> "Show details for record with ID '98765'."

**🤖 AI Agent:**
> I've fetched the details for record 98765. It's 'John Smith' from 'Acme Corp'. Current status is 'Warm Lead' and his email is john@acme.com.

---

**👤 You:**
> "List my recent wallet transactions."

**🤖 AI Agent:**
> I found 5 recent transactions. The latest was a deduction of $10.50 for 'Campaign SMS Fees' on June 1st.


## ❓ FAQ

**Q: How do I find my Collection ID?**
Use the `list_collections` tool to see all available data sets (e.g., People, Company) in your workspace along with their unique IDs.

**Q: Can I filter records by specific field values?**
Yes, the `list_collection_records` tool accepts an optional `filter_json` parameter where you can specify your search criteria.

**Q: Is it possible to track my wallet balance?**
Absolutely. Use the `list_wallet_transactions` tool to retrieve a history of all balance changes and transactions in your Zixflow account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zixflow](https://vinkius.com/mcp/zixflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zixflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zixflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zixflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zixflow": {
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
