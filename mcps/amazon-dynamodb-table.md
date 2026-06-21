# Amazon DynamoDB Table MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-dynamodb-table)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amazon-dynamodb-table-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amazon-dynamodb-table-mcp)
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


## Installation & Usage

To install and use the **Amazon DynamoDB Table** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-dynamodb-table](https://vinkius.com/mcp/amazon-dynamodb-table)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
