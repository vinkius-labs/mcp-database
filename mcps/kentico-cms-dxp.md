# Kentico (CMS & DXP) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kentico-cms-dxp)
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


## ❓ FAQ

**Q: Can I update a specific page property using my agent?**
Yes. Use the `update_site_document` tool. You just need to provide the site name, culture, and alias path, along with a JSON block of the fields you want to mutate. Your agent will process the update through the Kentico REST service instantly.

**Q: How do I list rows from a custom table defined in Kentico?**
The `list_custom_table_rows` tool allows your agent to extract tabular data contents from any custom table item structured within your project. You just need to provide the target table name to retrieve the current entries.

**Q: Can my agent manage system objects like user roles?**
Absolutely. Use tools like `list_system_objects` and `update_system_object` with the object type `cms.role`. Your agent can help you audit current roles and mutate their properties through natural conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kentico-cms-dxp](https://vinkius.com/mcp/kentico-cms-dxp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kentico (CMS & DXP)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `kentico-cms-dxp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kentico (CMS & DXP)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kentico-cms-dxp": {
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
