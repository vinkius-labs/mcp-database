# Attio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/attio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage your CRM data with Attio — track objects, records, and relationships via AI.

## Description
The **Attio MCP Server** brings powerful CRM capabilities directly to your AI agent. Seamlessly manage your relationship data, from standard objects like People and Companies to custom entities and complex record attributes using simple natural language.

### Key Features

- **Object Oversight** — List all data objects (tables) in your workspace and retrieve detailed metadata for any specific entity.
- **Record Management** — Query, create, and update records for any object, including people, companies, and deals.
- **Smart Assert (Upsert)** — Use the `assert_record` tool to automatically create or update records based on unique matching attributes (e.g., email).
- **Attribute Intelligence** — Access available fields (attributes) for any object to understand your data structure.
- **Global Search** — Perform fuzzy searches across multiple objects simultaneously to find relevant records instantly.
- **Secure API Integration** — Uses secure Bearer Token authentication with your Attio Personal Access Token (PAT).

### Who is this for?

- **Sales Teams** — Quickly search for prospect details and update deal statuses during conversations.
- **Account Managers** — Retrieve company information and relationship history without manual dashboard navigation.
- **Growth Marketers** — Programmatically assert records from new leads and enrich CRM data using AI-assisted tools.


## Available Tools (9)
- **assert_record**: Upsert a record (update if exists, create otherwise)
- **create_record**: Create a new record in an object
- **get_account_check**: Verify Attio account connection
- **get_object**: Get metadata for a specific object
- **get_record**: Retrieve a specific record by ID
- **list_attributes**: List all attributes (columns) for a specific object
- **list_objects**: List all objects (tables) in the Attio workspace
- **query_records**: Query and filter records for a specific object
- **search_records**: Global fuzzy search across all objects (Beta)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Attio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for any companies named 'Acme' in my CRM."

**🤖 AI Agent:**
> I've found 2 companies matching 'Acme': 'Acme Corp' and 'Acme Logistics'. Would you like to see the details for one of them?

---

**👤 You:**
> "Assert a person record for 'Jane Doe' with email 'jane@example.com'."

**🤖 AI Agent:**
> The record for Jane Doe has been successfully asserted. If she already existed, her information was updated; otherwise, a new person was created.

---

**👤 You:**
> "List all deal stages and attributes for 'Deals'."

**🤖 AI Agent:**
> I've retrieved 12 attributes for the 'Deals' object, including 'Stage' (select), 'Amount' (currency), and 'Closing Date' (date).


## ❓ FAQ

**Q: How do I get my Attio Personal Access Token?**
Log in to your Attio account, go to **Workspace Settings > Developers**, and you can create a new Personal Access Token (PAT) there.

**Q: What are 'Attributes' in Attio?**
Attributes are the columns or fields on an object (e.g., Name, Email, Deal Value). You can list them using the `list_attributes` tool.

**Q: How does 'assert_record' work?**
The `assert_record` tool performs an 'upsert'. It checks if a record with a specific matching attribute (like an email address) already exists. If it does, it updates it; if not, it creates a new record.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/attio](https://vinkius.com/mcp/attio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Attio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `attio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Attio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "attio": {
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
