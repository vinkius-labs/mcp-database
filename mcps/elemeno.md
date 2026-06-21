# Elemeno MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elemeno)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to manage content collections, track singletons, and monitor items via the Elemeno CMS API.

## Description
Integrate **Elemeno**, the headless CMS designed for developers, directly into your AI workflow. Manage your content collections and singletons (global pages), track individual items and their publishing statuses, monitor field schemas, and oversee your entire content library using natural language.

### What you can do

- **Collection Oversight** — List and retrieve detailed information and field schemas for all your content collections.
- **Content Intelligence** — Monitor individual collection items, resolving titles, slugs, and real-time publishing statuses.
- **Singleton Management** — Access and monitor singleton content blocks, resolving global settings and unique page data.
- **Content Auditing** — Retrieve high-level summaries of collection activity, item counts, and organizational CMS health.

### How it works

1. Connect the Elemeno integration to your AI assistant.
2. Authorize using your Elemeno API Key (found in your project settings).
3. Orchestrate your content management and digital assets through intuitive conversation.

### Who is this for?

- **Content Managers** — Quickly check publishing statuses and item volumes on the go.
- **Web Developers** — Audit collection schemas and singleton data via chat during development.
- **Operations Teams** — Monitor content updates and organizational CMS metadata instantly.


## Available Tools
- **get_elemeno_account_metadata**: Retrieve metadata and limits for your Elemeno account
- **get_collection_details**: Get detailed settings and field schema for a specific collection
- **get_collection_item_details**: Get full content and metadata for a specific item in a collection
- **quick_content_volume_audit**: Retrieve a high-level summary of collection and singleton activity
- **get_singleton_content**: Get the full content data for a specific singleton
- **list_content_collections**: List all content collections configured in your Elemeno account
- **list_collection_items**: List all content items within a specific collection
- **list_published_content**: Identify items that are currently in a "Published" status
- **list_content_singletons**: List all singleton content blocks (unique global pages/settings)
- **search_collection_content**: Search for items within a collection using a title or slug keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elemeno** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all content collections in my project."

**🤖 AI Agent:**
> I've found 4 collections, including 'Blog Posts', 'Team Members', and 'Products'. Would you like to see the items within the Blog Posts collection?

---

**👤 You:**
> "Show me the items in the 'Services' collection."

**🤖 AI Agent:**
> The Services collection has 5 items, including 'Web Design' (published), 'SEO Optimization' (published), and 'Mobile App Dev' (draft). Should I pull the full content for Web Design?

---

**👤 You:**
> "What is the content of the 'Contact Page' singleton?"

**🤖 AI Agent:**
> The 'Contact Page' singleton contains fields for 'Hero Title', 'Office Address', and 'Support Email'. The published title is 'Get in Touch with Us'. Would you like the full JSON data for this page?


## ❓ FAQ

**Q: How do I get an Elemeno API Key?**
Log in to your Elemeno dashboard, select your project, navigate to **Settings > API**, and you can retrieve your unique API Key from there.

**Q: Does the integration support draft content?**
Yes, you can use the list_collection_items tool to see all items, including their status (e.g., draft or published). Specific content retrieval depends on your API key permissions.

**Q: Can the agent update content via the API?**
This integration currently focuses on listing and auditing content. Creating or updating items and singletons should be managed via the Elemeno dashboard or specific management API endpoints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elemeno](https://vinkius.com/mcp/elemeno)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elemeno** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `elemeno` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elemeno** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elemeno": {
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
