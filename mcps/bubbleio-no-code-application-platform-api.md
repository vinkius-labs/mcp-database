# Bubble.io (No-code Application Platform API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bubbleio-no-code-application-platform-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bubbleio-no-code-application-platform-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bubbleio-no-code-application-platform-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Bubble.io application data and trigger backend workflows directly from any AI agent.

## Description
Connect your **Bubble.io** no-code application to your AI agent to perform deep data operations and automate backend logic through natural language.

### What you can do

- **Data Management** — Perform full CRUD (Create, Read, Update, Delete) operations on any exposed data type in your Bubble database.
- **Advanced Search** — Query your database using complex constraints, pagination, and custom sorting to find exactly what you need.
- **Bulk Operations** — Create up to 1,000 records in a single request using the high-performance bulk endpoint.
- **Workflow Automation** — Trigger any backend API workflow by name, allowing your AI to execute complex business logic, send emails, or process payments.
- **Record Inspection** — Fetch detailed metadata for specific 'Things' using their Unique ID (UID).

### How it works

1. Subscribe to this server
2. Provide your Bubble App URL and API Token
3. Start interacting with your app's database and workflows from Claude, Cursor, or any MCP client

### Who is this for?

- **No-code Developers** — Debug data, run migrations, or test backend workflows without leaving your development environment.
- **Product Managers** — Extract quick reports or update application settings via simple chat commands.
- **Operations Teams** — Automate repetitive data entry or trigger maintenance workflows using IA.


## Available Tools
- **bulk_create_things**: Provide a string with one JSON object per line (NDJSON format).

Bulk create multiple Things in the Bubble database
- **create_thing**: Provide fields as a JSON object.

Create a new Thing in the Bubble database
- **delete_thing**: Delete a Thing from the Bubble database
- **get_thing**: Retrieve a specific Bubble Thing by its UID
- **replace_thing**: Missing fields are reset to defaults or cleared.

Replace (Put) an existing Thing in the Bubble database
- **search_things**: Can use constraints (URL-encoded JSON array), cursor, limit, and sorting.

Search, paginate, and sort Things in the Bubble database
- **trigger_workflow**: Trigger a Bubble API Workflow
- **update_thing**: Update (Patch) an existing Thing in the Bubble database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bubble.io (No-code Application Platform API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all 'rentalunit' records where the price is less than 500."

**🤖 AI Agent:**
> I've searched the 'rentalunit' table. I found 3 matches: 'Cozy Studio' (UID: 123), 'Urban Loft' (UID: 456), and 'Garden Room' (UID: 789). Would you like the full details for any of these?

---

**👤 You:**
> "Create a new 'customer' record with the name 'John Doe' and email 'john@example.com'."

**🤖 AI Agent:**
> Successfully created a new 'customer' record. The Unique ID (UID) for John Doe is 1715829304123x456. Is there anything else you'd like to add to this profile?

---

**👤 You:**
> "Trigger the 'process_refund' workflow for transaction UID 987654321."

**🤖 AI Agent:**
> The 'process_refund' backend workflow has been triggered for UID 987654321. The Bubble server has acknowledged the request and is processing the logic now.


## Installation & Usage

To install and use the **Bubble.io (No-code Application Platform API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bubbleio-no-code-application-platform-api](https://vinkius.com/mcp/bubbleio-no-code-application-platform-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
