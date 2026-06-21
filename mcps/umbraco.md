# Umbraco MCP Server

Automate content workflows via Umbraco — retrieve delivery content, execute backoffice CRUD, and browse media assets directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/umbraco)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Umbraco CMS** backend to any AI agent and take full autonomous control bridging the powerful Delivery and Management APIs purely through natural conversation.

### What you can do

- **Delivery API Traversing** — Instantly list public pages, query by content type, or securely fetch structured fields by their exact domain paths organically
- **Backoffice Document Control** — Push new document permutations natively adhering to your configured schemas without opening a single GUI panel
- **Site Mutations** — Command the targeted removal of any outdated published nodes or force updates to internal fields seamlessly via `update_cms_document`
- **Schema & Media Insight** — Grab absolute lists tracking your stored binary media files alongside the global Document Types blueprints mapped out natively

### How it works

1. Subscribe manually to this connected MCP server
2. Inject your active Umbraco Base URL mapping and your Management/Delivery Bearer Auth Token
3. Engage directly your preferred AI model (Claude or Cursor) asking it to index pages natively

Eliminate messy IDE switching while structuring robust Headless projects. Let the AI prototype content inside Umbraco dynamically utilizing REST interfaces.

### Who is this for?

- **CMS Platform Engineers** — automate routine headless content extractions requesting schema structures from the LLM avoiding UI switch delays 
- **Digital Editors** — prompt the agent to bulk-view lists of raw content items skipping complicated table drill-downs natively 
- **Frontend Architects** — rapidly confirm internal content API stability extracting pure JSON payloads mapping to visual interfaces directly


## Available Tools
- **create_cms_document**: Provide the document data as a JSON object adhering to the schema.

Creates a new document in the Umbraco CMS
- **delete_cms_document**: This action is irreversible.

Permanently deletes a document from the Umbraco CMS
- **get_delivery_content_by_id**: Retrieves a specific content item by its GUID or numeric ID via Delivery API
- **get_delivery_content_by_path**: g., "/home/about").

Retrieves a specific content item by its URL path
- **get_management_document**: Retrieves a specific document via the Umbraco Management API (Drafts/Backoffice)
- **list_delivery_content**: Supports pagination via take and skip.

Lists content available via the Umbraco Delivery API
- **list_document_types**: Lists all document types (schemas) defined in Umbraco
- **list_media_assets**: Lists media assets (images, files) from the Umbraco Media library
- **query_delivery_content**: g., "contentType:blogPost").

Filters content items using the Umbraco Delivery API query syntax
- **update_cms_document**: Provide the document ID and JSON updates.

Updates fields of an existing document in Umbraco


## Installation & Usage

To install and use the **Umbraco** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/umbraco](https://vinkius.com/mcp/umbraco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
