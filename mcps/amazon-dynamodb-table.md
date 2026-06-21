# Amazon DynamoDB Table MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-dynamodb-table)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it manages items in a single Amazon DynamoDB Table. That's its only function, and nothing else. Incredible for giving your AI a secure NoSQL database.

## Description
This server strips away dangerous global AWS permissions. It gives your AI agent one surgical superpower: **the ability to query, insert, and update items inside one specific DynamoDB Table.**

By strictly scoping access, your AI can safely manage structured data, store chat histories, and process complex NoSQL queries without ever touching your critical cloud databases.

### The Superpowers

- **Absolute Containment:** The agent is locked to a single table. It cannot list other tables or drop your production data.
- **Native DynamoDB Integration:** Direct interactions with DynamoDB, supporting complex queries and indexes.
- **Plug & Play Database:** Instantly gives your agent a scalable NoSQL database to store structured memories and application state.


## Available Tools
- **delete_item**: Delete an item from the DynamoDB table
- **get_item**: Get an item from the DynamoDB table
- **put_item**: Put an item into the DynamoDB table
- **query_table**: Query the DynamoDB table
- **scan_table**: Scan the DynamoDB table


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amazon DynamoDB Table** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the user with ID '123' from the table."

**🤖 AI Agent:**
> I've fetched the user. Here are the details: Name is John Doe, and the account status is 'Active'.

---

**👤 You:**
> "Add a new record for order 'ORD-999'."

**🤖 AI Agent:**
> Done! I've inserted the new order record 'ORD-999' into the DynamoDB table successfully.

---

**👤 You:**
> "Scan the table for all inactive users."

**🤖 AI Agent:**
> I've scanned the table and applied the filter. I found 15 users marked as inactive. Would you like me to delete them or just list their IDs?


## ❓ FAQ

**Q: Why limit the agent to a single table?**
To enforce the principle of least privilege and zero-trust architecture. An autonomous agent shouldn't have the power to alter global cloud databases, which prevents accidental corruption of critical systems.

**Q: Can my agent access multiple tables?**
Each instance of this server is scoped to exactly one table. If your agent needs access to multiple tables, you can subscribe to this server multiple times — each with a different table configuration. This maintains strict isolation.

**Q: Can I query using secondary indexes (GSI)?**
Yes, you can specify the 'IndexName' inside your expression parameters when using the query tool, allowing the agent to perform efficient lookups on Global Secondary Indexes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-dynamodb-table](https://vinkius.com/mcp/amazon-dynamodb-table)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amazon DynamoDB Table** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `amazon-dynamodb-table` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amazon DynamoDB Table** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amazon-dynamodb-table": {
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
