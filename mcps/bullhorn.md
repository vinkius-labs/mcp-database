# Bullhorn MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bullhorn)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage recruitment workflows and ATS data via Bullhorn — retrieve, create, update, and delete entities, notes, and associations directly from any AI agent.

## Description
Connect your **Bullhorn** ATS and CRM account to any AI agent to manage candidates, job orders, client contacts, and corporate notes through natural conversation.

### What you can do

- **Entity Management** — Retrieve, create, update, or delete single or multiple Bullhorn entities (like Candidates, JobOrders, or ClientContacts) by ID.
- **To-Many Associations** — Fetch associated records for to-many relationships such as client contacts for a client corporation.
- **Corporate Notes** — Retrieve all notes associated with a specific ClientCorporation to track communication history.
- **Bulk Associations** — Retrieve associated entity IDs for multiple parent entities in bulk.

### How it works

1. Subscribe to this server
2. Enter your Bullhorn REST URL and REST Token
3. Start managing your recruitment pipeline from Claude, Cursor, or any MCP-compatible client

No more manual searching through complex ATS interfaces. Your AI acts as a dedicated recruiting assistant.

### Who is this for?

- **Recruiters** — Instantly retrieve candidate details, update job orders, and check notes without leaving your workspace.
- **HR Managers** — Keep track of client contacts and corporate relationships seamlessly.
- **Operations Leads** — Automate ATS querying to orchestrate staffing workflows smoothly.


## Available Tools
- **create_entity**: The data must be a valid JSON string representing the entity properties.

Create a new Bullhorn entity
- **create_event_subscription**: Create an event subscription
- **delete_entity**: Delete a Bullhorn entity
- **delete_event_subscription**: Delete an event subscription
- **find_data_hub_records**: Provide the criteria as a JSON string.

Find records in Bullhorn Data Hub
- **get_all_corp_notes**: Get all notes for a ClientCorporation
- **get_associations**: Requires a JSON string for the request body containing ids, start, count, etc.

Retrieve associated entity IDs for multiple parent entities
- **get_entities**: Get multiple Bullhorn entities by IDs
- **get_entitlements**: Get entity entitlements for the current user
- **get_entity**: g., Candidate, JobOrder) by its ID. You must specify the fields to return.

Get a single Bullhorn entity by ID
- **get_events**: Note: Consuming events purges them from the subscription queue.

Retrieve and consume events from a subscription
- **get_to_many**: g., clientContacts for a ClientCorporation).

Get to-many associations for an entity
- **update_entity**: The data must be a valid JSON string containing the fields to update.

Update an existing Bullhorn entity
- **upsert_data_hub_records**: Provide the payload as a JSON string.

Upsert records into Bullhorn Data Hub


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bullhorn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the candidate with ID 12345 showing their first name, last name, and email."

**🤖 AI Agent:**
> I've retrieved the candidate details using `get_entity`:
- **First Name**: John
- **Last Name**: Doe
- **Email**: john.doe@example.com

---

**👤 You:**
> "Get all corporate notes for ClientCorporation ID 98765."

**🤖 AI Agent:**
> Using `get_all_corp_notes`, I found 2 notes for ClientCorporation 98765:
1. 'Discussed contract renewal terms.' (Action: Client Call)
2. 'Follow-up scheduled for next Tuesday.' (Action: Email)

---

**👤 You:**
> "Update candidate 12345's status to 'Placed'."

**🤖 AI Agent:**
> I've updated the candidate's status to 'Placed' using `update_entity`.


## ❓ FAQ

**Q: Can I retrieve a single candidate or job order details using this integration?**
Yes! Use the `get_entity` tool by specifying the entity type (e.g., 'Candidate' or 'JobOrder'), the target ID, and the fields you want to return.

**Q: How do I fetch all notes associated with a specific ClientCorporation?**
You can use the `get_all_corp_notes` tool. Provide the `client_corp_id` and the fields you want to retrieve to get a complete history of notes.

**Q: Is it possible to update an existing candidate's information?**
Yes, you can use the `update_entity` tool. Pass the entity type, the target ID, and a JSON string containing the updated fields in the `data` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bullhorn](https://vinkius.com/mcp/bullhorn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bullhorn** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bullhorn` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bullhorn** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bullhorn": {
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
