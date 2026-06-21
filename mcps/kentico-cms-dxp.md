# Kentico (CMS & DXP) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kentico-cms-dxp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kentico-cms-dxp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kentico-cms-dxp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage content and system objects via Kentico Xperience — retrieve documents, manage users, and audit custom tables.

## Description
Connect your **Kentico Xperience** project to any AI agent and take full control of your digital experience platform (DXP) and enterprise CMS through natural conversation.

### What you can do

- **Document Orchestration** — Retrieve and update site pages and documents based on alias paths, cultures, and site names directly from your agent
- **System Object Management** — Create, list, and mutate general system objects (roles, templates, settings) using structured REST mappings
- **User CRM & Audit** — List global platform users and retrieve detailed account profiles, including roles and metadata securely
- **Custom Table Analytics** — Extract tabular data from Kentico custom tables to monitor internal registries and business-specific data models
- **Schema Visibility** — Discover and inspect Kentico object types and scalar properties to understand your project's underlying data structure
- **Content Lifecycle** — Perform deep property mutations on existing documents or irreversibly delete unused system objects to maintain an optimized repository

### How it works

1. Subscribe to this server
2. Enter your Kentico REST URL and Authentication Header (e.g., Basic base64)
3. Start managing your DXP from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Full-Stack Developers** — test REST service queries and introspect Kentico system objects through natural conversation without manual API tools
- **Content Architects** — audit document properties and custom table schemas across multiple cultures and site environments efficiently
- **System Administrators** — monitor user accounts and manage system-level objects and roles across your entire Kentico instance


## Available Tools
- **create_system_object**: Create a new Kentico system object
- **delete_system_object**: Delete a Kentico system object
- **get_site_document**: Get a document from the Kentico Xperience CMS
- **get_single_object**: Get a specific Kentico system object by ID
- **get_user**: Get details for a specific Kentico user
- **list_custom_table_rows**: List rows from a Kentico custom table
- **list_system_objects**: g., roles provisions, page templates) from Kentico REST.

List Kentico system objects by type
- **list_users**: user in Kentico.

List global Kentico users
- **update_site_document**: Update an existing document in the Kentico CMS
- **update_system_object**: Update an existing Kentico system object


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kentico (CMS & DXP)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the 'Home' page document from site 'CorporateSite' in 'en-us' culture"

**🤖 AI Agent:**
> Retrieving document '/Home'… I've fetched the page structure. It includes properties like DocumentName: 'Home', DocumentMenuCaption: 'Welcome', and the associated page template ID. Would you like to see the full content fields?

---

**👤 You:**
> "Update the DocumentName of '/About-Us' to 'Our Team' on currentsite"

**🤖 AI Agent:**
> Updating document '/About-Us'… The name has been successfully changed to 'Our Team'. I've also updated the associated metadata. This change is now active in the Kentico database.

---

**👤 You:**
> "List all rows from the custom table 'MyCompany.Inventory'"

**🤖 AI Agent:**
> I've retrieved 12 entries from 'MyCompany.Inventory'. Highlights include items 'SKU-101' (Stock: 45), 'SKU-105' (Stock: 12), and 'SKU-108' (Stock: 0). Would you like to see the detailed audit logs for these items?


## Installation & Usage

To install and use the **Kentico (CMS & DXP)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kentico-cms-dxp](https://vinkius.com/mcp/kentico-cms-dxp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
