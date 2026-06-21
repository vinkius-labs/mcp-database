# Builder.io (Visual CMS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/builderio-visual-cms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Builder.io content, assets, and models via AI — fetch entries, update data, and query GraphQL APIs directly.

## Description
Connect your **Builder.io** space to any AI agent and take full control of your visual CMS and headless content through natural conversation.

### What you can do

- **Content Management** — Fetch entries from any model using `get_content` or retrieve pre-rendered HTML for components with `get_html`.
- **Write Operations** — Create, update, or delete content entries programmatically using the Write API tools like `create_content` and `update_content`.
- **Advanced Querying** — Execute complex GraphQL queries against the Content API or perform administrative tasks using `admin_graphql`.
- **Asset Handling** — Upload new media assets or remove existing ones by URL to maintain your digital asset library.
- **Targeting & Personalization** — Use user attributes and MongoDB-style queries to fetch specific content variants.

### How it works

1. Subscribe to this server
2. Enter your Builder.io Public Key (and Private Key for write access)
3. Start managing your digital experience from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — query and update CMS content directly from your IDE without switching to the Builder dashboard
- **Content Managers** — automate bulk updates or content migrations using natural language instructions
- **Marketing Teams** — quickly inspect content targeting and pre-rendered HTML outputs for SEO checks


## Available Tools (9)
- **admin_graphql**: Requires Private API Key.

Execute an Admin API GraphQL query/mutation
- **create_content**: Requires Private API Key.

Create a new content entry
- **delete_asset_by_url**: Delete an asset by its URL
- **delete_content**: Requires Private API Key.

Delete a content entry
- **get_content**: Get content from a Builder.io model
- **get_html**: Get pre-rendered HTML for a Builder.io model
- **query_graphql**: Query Builder.io content using GraphQL
- **update_content**: Requires Private API Key.

Update an existing content entry
- **upload_asset**: Requires Private API Key.

Upload an asset (image, video, document)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Builder.io (Visual CMS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the latest 5 entries from the 'page' model in Builder.io."

**🤖 AI Agent:**
> I've retrieved the 5 most recent entries from your 'page' model. They include 'Home Page' (ID: abc-123), 'About Us' (ID: def-456), and three others. Would you like to see the full data for any of these?

---

**👤 You:**
> "Update the 'announcement-bar' entry with ID 'entry-888' to change the text to 'Sale ends tonight!'."

**🤖 AI Agent:**
> I've updated the 'announcement-bar' entry (ID: entry-888). The data field has been patched with the new text. The change is now live in your Builder space.

---

**👤 You:**
> "Upload this image URL to my Builder assets: https://example.com/hero.jpg"

**🤖 AI Agent:**
> The asset has been successfully uploaded to Builder.io. You can now reference it in your content using the new Builder CDN URL: https://cdn.builder.io/api/v1/image/assets/...


## ❓ FAQ

**Q: Can I fetch pre-rendered HTML for my components instead of raw JSON?**
Yes! Use the `get_html` tool. It returns pre-rendered HTML for a specific model and URL, which is perfect for quick inspections or server-side integrations.

**Q: Do I need a Private API Key to use this server?**
A Public Key is required for all read operations (`get_content`, `query_graphql`). However, a Private Key is mandatory for write operations like `create_content`, `update_content`, or `admin_graphql`.

**Q: Can I perform administrative tasks like managing Spaces or Models?**
Yes, the `admin_graphql` tool allows you to execute administrative queries and mutations against the Builder Admin API, provided you have supplied a Private API Key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/builderio-visual-cms](https://vinkius.com/mcp/builderio-visual-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Builder.io (Visual CMS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `builderio-visual-cms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Builder.io (Visual CMS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "builderio-visual-cms": {
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
