# Azure Cosmos DB Container MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/azure-cosmos-db-container)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it manages documents in a single Azure Cosmos DB Container. That's its only function, and nothing else. Incredible for giving your AI a secure NoSQL database.

## Description
This server strips away dangerous global Azure permissions. It gives your AI agent one surgical superpower: **the ability to query, insert, and update documents inside one specific Cosmos DB Container.**

By strictly scoping access, your AI can safely manage structured data, store chat histories, and process complex NoSQL queries without ever touching your critical cloud databases.

### The Superpowers

- **Absolute Containment:** The agent is locked to a single container. It cannot list other databases or drop your production data.
- **Native Cosmos DB Integration:** Direct interactions with Cosmos DB, supporting rich SQL queries and partition management.
- **Plug & Play Database:** Instantly gives your agent a scalable NoSQL database to store structured memories and application state.


## Available Tools
- **create_document**: Make sure to provide the ID and Partition Key properties inside the documentJson if required.

Create a new document in the Cosmos DB Container
- **delete_document**: Provide partitionKey if your container requires it.

Delete a document from the Cosmos DB Container
- **get_document**: Provide partitionKey if your container requires it.

Retrieve a specific document by its ID
- **query_documents**: You can optionally provide parameters in JSON format. Do not include the DB or Container name in the query, Cosmos expects queries like "SELECT * FROM c WHERE c.status = @status".

Execute a SQL query against the configured Cosmos DB Container


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Azure Cosmos DB Container** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Query the database for all documents where 'status' is 'pending'."

**🤖 AI Agent:**
> I executed `SELECT * FROM c WHERE c.status = 'pending'`. I found 12 pending documents.

---

**👤 You:**
> "Create a new document with id 'user_123' and name 'John Doe'."

**🤖 AI Agent:**
> The document was successfully created in the Cosmos DB container.

---

**👤 You:**
> "Delete the document with id 'old_report_456'."

**🤖 AI Agent:**
> I have permanently deleted the document 'old_report_456' from the database.


## ❓ FAQ

**Q: Why limit the agent to a single Cosmos Container?**
To enforce zero-trust security. An autonomous AI agent should not have the ability to read or delete data across your entire Cosmos DB Account (which might include user passwords, financial records, etc.). By scoping it to a single container, you eliminate the risk of catastrophic data loss.

**Q: How do I write Cosmos SQL queries here?**
You don't need to specify the database or container in the query. Just use the standard alias `c`. For example: `SELECT * FROM c WHERE c.isComplete = false`. You can also pass parameters securely.

**Q: Do I need to handle Partition Keys?**
The query tool automatically enables cross-partition queries to simplify AI workflows. However, for getting, creating, or deleting specific documents, you should provide the `partitionKey` if your container is configured to require one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/azure-cosmos-db-container](https://vinkius.com/mcp/azure-cosmos-db-container)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Azure Cosmos DB Container** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `azure-cosmos-db-container` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Azure Cosmos DB Container** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "azure-cosmos-db-container": {
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
