# Knack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Knack database — list objects, query records, and perform CRUD operations via natural language.

## Description
Connect your **Knack** application to any AI agent and take full control of your no-code database through natural conversation.

### What you can do

- **Database Schema Discovery** — List all objects and fields to understand your data structure without leaving the chat
- **Record Management** — Create, retrieve, update, and delete records in any object securely
- **Advanced Querying** — Search for specific records using complex filters based on any field criteria
- **Data Auditing** — Get detailed summaries of specific records to verify information or track changes
- **Bulk Operations** — Effortlessly manage multiple records by providing structured data to your agent

### How it works

1. Subscribe to this server
2. Enter your Knack Application ID and REST API Key
3. Start managing your data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — quickly query and update business data without navigating complex dashboards
- **No-Code Developers** — verify data structures and test API interactions through natural language
- **Data Analysts** — extract specific datasets for rapid analysis and reporting


## Available Tools (10)
- **list_objects**: This is the first step to understand the database structure and find the "Object Key" needed for record operations.

List all objects in the Knack application
- **get_object_schema**: Returns metadata including the object name, key, and high-level structure. Use this to verify you are working with the correct database table.

Get the schema of a specific Knack object
- **list_records**: You must provide the object_key. Use this to browse the actual data stored in your database.

List records for a specific Knack object
- **get_record**: Requires both the object_key and the record_id. Use this for detailed auditing of a specific entry.

Get a specific record by ID
- **create_record**: You must provide the data as a JSON string where keys are the field keys (e.g., field_1). Ensure you have checked the object schema first to know which fields are required.

Create a new record in a Knack object
- **update_record**: Provide only the fields you wish to change in the JSON string data. This is a partial update.

Update an existing record in a Knack object
- **delete_record**: Use with caution as this action cannot be undone.

Delete a record from a Knack object
- **list_object_fields**: This is crucial for understanding the data types and identifying the field keys (field_1, field_2, etc.) needed for creating or updating records.

List all fields for a specific Knack object
- **search_records**: The filters must be provided as a JSON string following the Knack Filter format (e.g., "[{\"field\":\"field_1\", \"operator\":\"is\", \"value\":\"test\"}]").

Search for records using filters
- **list_account_applications**: Use this to verify access or discover application IDs.

List all applications in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Knack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all database objects in my Knack app"

**🤖 AI Agent:**
> I've found 5 objects: 'Customers' (object_1), 'Orders' (object_2), 'Products' (object_3), 'Invoices' (object_4), and 'Settings' (object_5). Which one would you like to explore?

---

**👤 You:**
> "Find all premium customers in 'object_1'"

**🤖 AI Agent:**
> Searching 'object_1' for records where 'Status' is 'Premium'… I've found 3 records: 'John Doe', 'Jane Smith', and 'Acme Corp'. Would you like to see the full details for any of these?

---

**👤 You:**
> "Create a new customer in 'object_1' with name 'Sarah' and email 'sarah@example.com'"

**🤖 AI Agent:**
> Successfully created a new record in 'object_1'. Record ID: 65a4b3c2d1e0f. Field 1 (Name): Sarah, Field 2 (Email): sarah@example.com. Is there anything else you'd like to do with this record?


## ❓ FAQ

**Q: How do I find the Object Key for a specific table?**
Use the `list_objects` tool. It will return all data objects in your application along with their names and unique keys (e.g., `object_1`). Use these keys for all subsequent record operations.

**Q: Can I search records using multiple conditions?**
Yes. Use the `search_records` tool and provide a JSON array of filter objects. For example: `[{"field":"field_1", "operator":"is", "value":"active"}, {"field":"field_2", "operator":"contains", "value":"premium"}]`.

**Q: How do I know which fields to use when creating a record?**
Use the `list_object_fields` tool with the target `object_key`. It will list all fields, their types, and their keys (e.g., `field_1`), which you must use as property names in your data JSON.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knack](https://vinkius.com/mcp/knack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Knack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `knack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Knack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "knack": {
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
