# Strapi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/strapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect your AI to Strapi. Fully orchestrate your headless CMS — create entries, manage content types, and upload media assets naturally.

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


## Available Tools (9)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Strapi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Review my Strapi content types and show the schema for 'product'."

**🤖 AI Agent:**
> Connected to Strapi.
**Content Types (`list_content_types`)**:
- `api::user.user`
- `api::product.product`

Schema for `api::product.product`:
- `title` (string), `price_tag` (decimal), `sku_code` (string), `available_inventory` (integer).

---

**👤 You:**
> "Construct a newly formatted post about system updates in the 'articles' content type."

**🤖 AI Agent:**
> Building JSON parameters...

**Executing Task (`create_entry`)**:
Successfully created entry ID: `402` in the `api::article.article` collection. Title set to 'System Updates V2', formatted correctly.

---

**👤 You:**
> "Upload a new promotional image dependency securely into the Media Library."

**🤖 AI Agent:**
> Accessing the Strapi Media Library securely...

**Asset Deployed (`upload_media_asset`)**:
The image `promo_banner_spring.jpg` has been successfully uploaded and is assigned the dynamic referential ID: `1005`. It's ready to be bound to your entries.


## ❓ FAQ

**Q: How does the AI know the correct JSON format for new entries?**
The agent calls `list_content_types` first to read each collection's field names and types. It then builds a compliant JSON payload matching the schema before calling `create_entry`.

**Q: Can the agent delete content types or schemas?**
No. `delete_entry` only removes individual data rows within a collection. It cannot alter, drop, or modify content type schemas or structural CMS settings.

**Q: Can I upload media files through the integration?**
Yes. Use `upload_media_asset` to add images, videos, or documents to the Strapi Media Library. You can also browse existing assets with `list_assets`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/strapi](https://vinkius.com/mcp/strapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Strapi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `strapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Strapi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "strapi": {
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
