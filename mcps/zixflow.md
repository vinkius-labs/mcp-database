# Zixflow MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zixflow)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zixflow-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zixflow-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Zixflow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zixflow](https://vinkius.com/mcp/zixflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
