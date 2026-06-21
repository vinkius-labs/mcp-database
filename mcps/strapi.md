# Strapi MCP Server

Connect your AI to Strapi. Fully orchestrate your headless CMS — create entries, manage content types, and upload media assets naturally.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/strapi)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Integrate the robust headless architecture of **Strapi** seamlessly into your conversational LLM workflows. By linking your AI securely to the Strapi REST ecosystem, engineering and content teams can effortlessly design schema types, interact with entries, and orchestrate media libraries directly from the terminal.

### What you can do

- **Architecture Discovery** — Quickly evaluate top-level content structures invoking `list_content_types` and systematically paginate underlying rows executing `list_entries`.
- **Content Construction** — Drive agile content updates creating new JSON-formatted parameters natively by calling `create_entry` or updating existing rows via `update_entry`.
- **Asset Orchestration** — Monitor uploaded visual data traversing the Media Library securely with `list_assets` or uploading remote dependencies instantly using `upload_media_asset`.
- **Audit & Clearance** — Protect production integrity by securely tracking and listing authorized active members leveraging `list_cms_users`.

### How it works

1. Define the Strapi MCP as an active integration inside your configuration environment.
2. In the parameter matrix, bind your deployed `STRAPI_BASE_URL` alongside a verified `STRAPI_API_KEY` created via your admin panel.
3. State your objective: "Fetch the properties of my 'articles' content type, and construct a newly formatted post containing the latest system update metrics."

### Who is this for?

- **Backend Architects** — Validate structure configurations and JSON payloads instantly across components without context-switching into the Strapi interface.
- **Technical Marketers** — Manage and formulate textual entries programmatically, scaling updates securely across the platform instantly.
- **Development Operations** — Automate tedious metadata adjustments and audit structural dependencies rapidly within safe, isolated loops.


## Available Tools
- **create_entry**: Provide the plural ID and a JSON string of fields.

Creates a new entry for a specific content type
- **delete_entry**: This action is irreversible.

Permanently deletes a content entry
- **get_entry_details**: Retrieves details for a specific content entry
- **list_assets**: Lists media assets stored in the Strapi Media Library
- **list_content_types**: Lists all content types (collections and single types) defined in Strapi
- **list_entries**: Provide the plural ID of the content type (e.g., "articles").

Lists entries for a specific content type
- **list_cms_users**: Lists all registered CMS users
- **update_entry**: Provide the plural ID, entry ID, and field updates.

Updates fields of an existing content entry
- **upload_media_asset**: Provide the public file URL to be fetched and uploaded.

Uploads a new file to the Media Library


## Installation & Usage

To install and use the **Strapi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/strapi](https://vinkius.com/mcp/strapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
