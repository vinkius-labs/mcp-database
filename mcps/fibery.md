# Fibery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fibery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your Fibery workspace to automate work management — query entities, create tasks, and manage comments directly from your AI agent.

## Description
Fibery is a work management platform that adapts to your unique processes. This MCP server allows your AI agent to interact with your Fibery workspace seamlessly.

### Key Features
- **Space & Schema Discovery** — List all your spaces (apps) and retrieve the full schema to understand your custom databases and fields.
- **Entity Management** — Query, create, update, and delete entities across any of your custom databases flawlessly.
- **Comment Integration** — Read and add comments to entities to keep your team in sync natively.
- **Advanced Querying** — Use granular filters and field selections to retrieve exactly the data you need synchronously.
- **Cross-Database Search** — Search for information across your entire workspace flawlessly through the agent.

### How it works
1. Subscribe to this server
2. Enter your Fibery workspace name and API Token
3. Start managing your projects and tasks from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Product Managers** — automate task updates and insight gathering without manual portal navigation
- **Software Teams** — sync development progress and manage bug tracking directly from your chat workflow
- **Operations Teams** — pull structured data and manage custom workflows through simple natural language queries


## Available Tools (11)
- **add_comment**: Add a comment to an entity
- **create_entity**: Create a new entity in a specific database
- **delete_entity**: Delete an entity
- **get_comments**: Retrieve comments for a specific entity
- **get_entity**: Get a specific entity by its UUID
- **get_schema**: Retrieve the full schema of the workspace, including all databases (types) and fields
- **list_apps**: List all Fibery apps (spaces)
- **list_users**: List all users in the Fibery workspace
- **query_entities**: Query entities from a specific database (type)
- **search_entities**: Search for entities by keyword across all databases
- **update_entity**: Update an existing entity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fibery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active spaces in my Fibery account."

**🤖 AI Agent:**
> I've retrieved your spaces. You have 'Product Management', 'Software Development', and 'Marketing Operations' active. Which one would you like to explore further?

---

**👤 You:**
> "Show me the tasks assigned to me in the 'Software Development' space."

**🤖 AI Agent:**
> Inspecting entities... I found 5 tasks assigned to you, including 'Fix Bug #102' and 'Implement API caching'. Would you like the full details for any of these?

---

**👤 You:**
> "Add a comment to task UUID-123 saying 'The client approved the design'."

**🤖 AI Agent:**
> Comment added successfully! Your message has been posted to the task and your team has been notified flawlessly.


## ❓ FAQ

**Q: How do I find my Fibery Workspace name?**
Your workspace name is the subdomain in your Fibery URL. For example, if you access Fibery at `https://my-team.fibery.io`, your workspace name is `my-team`.

**Q: How do I generate a Fibery API Token?**
In your Fibery workspace, go to **Settings > API**, click on **Create New Token**, give it a name, and copy the generated token immediately.

**Q: Can I query custom fields created in my spaces?**
Yes! Use the `get_schema` tool to see the fully qualified names of your custom fields, and then include them in the `select_json` parameter of the `query_entities` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fibery](https://vinkius.com/mcp/fibery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fibery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fibery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fibery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fibery": {
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
