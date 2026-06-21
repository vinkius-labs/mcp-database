# Deta Space (Serverless Personal Cloud API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deta-space-serverless-personal-cloud-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your personal cloud via Deta Space — store data in Deta Base and files in Deta Drive directly from any AI agent.

## Description
Connect your **Deta Space** personal cloud to any AI agent and manage your serverless data and files through natural conversation.

### What you can do

- **Deta Base (NoSQL)** — Store, retrieve, and query JSON data with high performance using tools like `base_put_items` and `base_query_items`.
- **Deta Drive (Storage)** — Upload, download, and list files in your personal cloud drives using `drive_upload_file` and `drive_list_files`.
- **Atomic Updates** — Modify specific attributes of your database items without overwriting the entire object via `base_update_item`.
- **Data Management** — Insert new items safely with `base_insert_item` or delete existing ones by their unique keys.

### How it works

1. Subscribe to this server
2. Enter your Deta Space App Key and Project ID
3. Start managing your serverless infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — build and manage serverless backends directly from your IDE.
- **Data Engineers** — quickly query and inspect NoSQL collections without leaving the chat interface.
- **Power Users** — automate personal file storage and data logging in a private, serverless environment.


## Available Tools
- **base_delete_item**: Delete an item from Deta Base by its key
- **base_get_item**: Retrieve a single item from Deta Base by its key
- **base_insert_item**: Store an item in Deta Base only if the key does not already exist
- **base_put_items**: Provide items as a JSON array string.

Store one or more items in Deta Base
- **base_query_items**: Query should be a JSON array of query objects (OR logic between objects, AND logic within).

Search for items in Deta Base based on queries
- **base_update_item**: Update specific attributes of an existing item in Deta Base
- **drive_delete_files**: Delete one or more files from Deta Drive
- **drive_download_file**: Download a file from Deta Drive by its name
- **drive_list_files**: List files in a Deta Drive
- **drive_upload_file**: Upload a file to Deta Drive


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deta Space (Serverless Personal Cloud API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files in my 'backups' drive on Deta."

**🤖 AI Agent:**
> I've listed the files in 'backups'. I found 3 files: 'db_dump.json', 'config.yaml', and 'logs.txt'. Would you like to download any of them?

---

**👤 You:**
> "Get the item with key 'user_88' from the 'profiles' base."

**🤖 AI Agent:**
> Retrieved profile for 'user_88': { "name": "Alice", "role": "admin", "status": "active" }. Do you need to update any of these fields?

---

**👤 You:**
> "Increment the 'login_count' by 1 for key 'user_88' in 'profiles'."

**🤖 AI Agent:**
> Successfully updated 'user_88'. The 'login_count' attribute has been incremented by 1.


## ❓ FAQ

**Q: How can I search for specific records in a Deta Base?**
Use the `base_query_items` tool. You can provide a JSON array of query objects to filter items by their attributes, and even handle pagination using the `limit` and `last` parameters.

**Q: Can I update just one field in a database item without sending the whole object?**
Yes! The `base_update_item` tool allows you to perform atomic updates. You can use the `set` parameter to update fields, `increment` for numbers, or `append` for arrays.

**Q: How do I upload a text file or document to Deta Drive?**
Use the `drive_upload_file` tool. Provide the `drive_name`, the desired file `name` (path), and the `content` of the file. The agent will handle the storage process for you.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deta-space-serverless-personal-cloud-api](https://vinkius.com/mcp/deta-space-serverless-personal-cloud-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deta Space (Serverless Personal Cloud API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deta-space-serverless-personal-cloud-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deta Space (Serverless Personal Cloud API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deta-space-serverless-personal-cloud-api": {
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
