# Bullhorn MCP Server

Manage recruitment workflows and ATS data via Bullhorn — retrieve, create, update, and delete entities, notes, and associations directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bullhorn)

## Overview
**Category:** human-resources
**Tools Count:** 14

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


## Installation & Usage

To install and use the **Bullhorn** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bullhorn](https://vinkius.com/mcp/bullhorn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
