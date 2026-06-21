# Payload CMS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/payload-cms-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your Payload CMS content directly from any AI agent — query collections, update documents, and manage globals via REST API.

## Description
Connect your **Payload CMS** instance to any AI agent and take full control of your headless content management through natural conversation.

### What you can do

- **Collection Management** — Query, filter, and sort documents across any collection using the `find_many` and `find_by_id` tools.
- **Content Operations** — Create, update, or delete documents directly from your chat interface with full JSON support.
- **Global Data** — Access and modify global configurations (like headers, footers, or site settings) using `get_global` and `update_global`.
- **Relationship Control** — Manage data complexity by specifying the `depth` of populated relationships in your queries.
- **Advanced Filtering** — Use the `where` parameter to perform complex queries using Payload's native query language.

### How it works

1. Subscribe to this server
2. Enter your Payload CMS Base URL
3. Provide an optional API Key and Auth Collection slug if your instance is protected
4. Start managing your content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — quickly update site copy or check entry statuses without logging into the admin panel.
- **Developers** — query production or staging data directly from the code editor to verify API responses.
- **Product Teams** — automate content audits and bulk updates through simple natural language commands.


## Available Tools
- **create_document**: Create a new document in a Payload CMS collection
- **delete_document**: Delete a document by ID in a Payload CMS collection
- **delete_preference**: Delete a user preference in Payload CMS
- **find_by_id**: Find a document by ID in a Payload CMS collection
- **find_many**: Find many documents in a Payload CMS collection
- **get_global**: g., Header, Footer).

Get a Payload CMS global
- **get_preference**: Get a user preference in Payload CMS
- **update_document**: Update a document by ID in a Payload CMS collection
- **update_global**: Update a Payload CMS global
- **update_preference**: Update a user preference in Payload CMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Payload CMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the last 3 documents in the 'posts' collection sorted by creation date."

**🤖 AI Agent:**
> I've retrieved the 3 most recent posts from your collection. They include 'New Features in v3', 'Getting Started with MCP', and 'API Best Practices'. Would you like to see the full content of any of these?

---

**👤 You:**
> "Update the document with ID 673c2 in the 'products' collection to set the price to 49.99."

**🤖 AI Agent:**
> I have successfully updated the product (ID: 673c2). The price is now set to 49.99. Is there anything else you'd like to modify in this document?

---

**👤 You:**
> "Get the current data for the 'header' global."

**🤖 AI Agent:**
> I've fetched the 'header' global data. It currently contains the site logo URL, a navigation array with 5 links, and a 'sticky' setting set to true. Do you need to update any of these fields?


## ❓ FAQ

**Q: How can I filter results to find specific documents in a collection?**
You can use the `find_many` tool and provide a JSON string in the `where` parameter. This follows Payload's standard query syntax, allowing you to filter by fields, operators (like `equals`, `contains`), and nested logic.

**Q: Can I control how much related data is returned in a query?**
Yes! Most query tools like `find_many`, `find_by_id`, and `get_global` include a `depth` parameter. Increasing this number will populate more levels of nested relationships.

**Q: Does this server support updating global settings like site headers?**
Absolutely. Use the `get_global` tool to retrieve current data and `update_global` to modify it. This is perfect for managing site-wide configurations without leaving your AI assistant.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/payload-cms-alternative](https://vinkius.com/mcp/payload-cms-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Payload CMS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `payload-cms-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Payload CMS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "payload-cms-alternative": {
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
