# ReadMe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/readme)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI to directly search, read, and manage developer documentation stored in your ReadMe project.

## Description
Connect your **ReadMe** documentation hub directly to your AI agent. Enabling this integration turns your AI into an expert technical writer and reader, capable of instantly scanning your entire developer documentation, changelogs, and custom pages without context switching.

### What you can do

- **Documentation Search** — Perform full-text searches across all your published guides and API references.
- **Content Retrieval** — Fetch the exact Markdown content of any specific documentation page, changelog, or category.
- **Project Analysis** — Understand how your documentation is categorized and structure new content accordingly.
- **Changelog Tracking** — Pull recent product updates and announcements formally published to your users.

### How it works

1. Authorize the ReadMe MCP server in your environment.
2. Provide your ReadMe API Key (found under your project's Configuration settings).
3. Ask your AI to summarize a specific API endpoint's documentation or list recent changelogs directly from your chat.

### Who is this for?

- **Developer Advocates** — Verify the accuracy of published guides and quickly draft new content referencing existing structures.
- **Technical Writers** — Search and audit current documentation for outdated references without leaving your code editor.
- **Software Engineers** — Instantly pull your company's official API documentation into your IDE to ensure your code aligns with published standards.


## Available Tools (10)
- **list_categories**: Lists all documentation categories on ReadMe
- **get_category**: Retrieves details for a specific documentation category
- **get_category_docs**: Lists all documentation pages under a specific category
- **get_doc**: Retrieves the full content of a documentation page
- **search_docs**: Performs a full-text search across all documentation pages
- **list_changelogs**: Lists all changelog posts
- **get_changelog**: Retrieves the full content of a specific changelog post
- **list_custom_pages**: Lists all custom standalone pages
- **get_custom_page**: Retrieves the full content of a custom page
- **get_project**: Retrieves details about the ReadMe project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ReadMe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the documentation for instructions on configuring webhooks."

**🤖 AI Agent:**
> Using the `search_docs` tool, I found several results. The top match is 'Webhook Installation Guide' (Slug: webhook-setup). It provides step-by-step instructions on setting endpoint URLs.

---

**👤 You:**
> "Get the contents of the changelog titled 'v2-api-release'."

**🤖 AI Agent:**
> I requested `get_changelog` for 'v2-api-release'. The post details new rate limits, updated endpoints for user management, and deprecation notices for the v1 metrics paths.

---

**👤 You:**
> "List all main documentation categories."

**🤖 AI Agent:**
> I fetched the configuration using `list_categories`. There are 4 global categories: 'Getting Started', 'Authentication', 'REST API Reference', and 'Webhooks Guide'.


## ❓ FAQ

**Q: Where do I obtain my ReadMe API Key?**
Log into your ReadMe dashboard. Navigate to your specific project, then open 'Configuration' and click on 'API Key'. You will use this key as the authentication parameter (our integration handles it natively as a Basic Auth username).

**Q: Does the server allow me to write or edit documentation?**
Currently, the MCP server is focused on read-only operations. It can query, retrieve, and search changelogs, custom pages, and standard documentation categories, bringing context to the AI securely without risking accidental overwrites.

**Q: In what format is the document content returned?**
All text and page content uses native Markdown format directly fetched from ReadMe's engine. This makes it perfect for the AI to interpret, syntax-highlight, and display naturally within chat or code comments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/readme](https://vinkius.com/mcp/readme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ReadMe** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `readme` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ReadMe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "readme": {
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
