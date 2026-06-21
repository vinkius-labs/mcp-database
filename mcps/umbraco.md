# Umbraco MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/umbraco)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate content workflows via Umbraco — retrieve delivery content, execute backoffice CRUD, and browse media assets directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Umbraco** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Use the delivery API to get the content from '/products/new-feature' and list out its properties."

**🤖 AI Agent:**
> I've pulled the content assigned to that path. It's a 'ProductPage' schema. Key properties include 'title' (New Feature Launch!) and strongly typed 'descriptionText'. Everything mapped perfectly fine over the Headless engine.

---

**👤 You:**
> "Look up our Document Types to see the exact schema required for a 'BlogPost'. Then create one JSON draft placeholder payload based on it."

**🤖 AI Agent:**
> A 'BlogPost' document requires 3 fields: `authorName`, `publishDate`, and `bodyText`. I have inherently crafted the JSON payload for this structure matching your schema accurately so we can push it cleanly up the line.

---

**👤 You:**
> "Delete the backoffice document holding ID d6ef43..."

**🤖 AI Agent:**
> Done. The document d6ef43... has been successfully nuked from the active Umbraco Management context.


## ❓ FAQ

**Q: Can it easily retrieve the content of a page assuming I only know its URL path?**
Absolutely. Instruct the agent to 'get_delivery_content_by_path' and supply something like '/home/about'. It traverses the Delivery API native routing map and returns perfectly all inner block grids and content variables attached.

**Q: How do I ensure the JSON payloads for `create_cms_document` are exactly what Umbraco expects?**
Use the agent to first run 'list_document_types'. It pulls down the global schema blueprints. The LLM can explicitly read the allowed field types (like rich text or media pickers) and logically construct the insertion matching it exactly.

**Q: Does it pull media details dynamically?**
Yes. Pinging 'list_media_assets' grants full insight over all stored visuals inside your Umbraco media containers, returning URL addresses alongside fundamental dimension formats so the agent can reference them anywhere.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/umbraco](https://vinkius.com/mcp/umbraco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Umbraco** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `umbraco` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Umbraco** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "umbraco": {
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
