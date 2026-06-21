# Contentful MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contentful)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to fetch, create, and manage digital content effortlessly using Contentful's headless architecture.

## Description
Integrate the **Contentful** content management platform directly into your conversational AI. Automate your editorial workflow and manage entries across spaces and environments without modifying code.

### What you can do

- **Content Retrieval** — Retrieve and display existing content entries, assets, and content models efficiently.
- **Entry Creation** — Command the AI to format and draft text content, creating new Contentful entries natively.
- **Space Discovery** — Ask the agent to find specific content types or query the environment architecture intuitively.

### How it works

1. Append this integration into your AI interface.
2. Authorize it using your Contentful Personal Access Token.
3. Request your agent to find entries or manage existing content.

### Who is this for?

- **Content Creators** — Outline an article in the chat and have it automatically pushed into a Contentful entry.
- **Developers** — Query the exact schema details of any content type while writing front-end components.
- **Digital Marketers** — Find and use specific image assets seamlessly without leaving the planning timeline.


## Available Tools
- **get_content_type**: Get details of a specific content type
- **update_entry**: Update an existing entry
- **create_entry**: Create a new entry in draft state
- **get_entry**: Get details of a specific entry
- **list_assets**: List all assets in the current environment
- **list_spaces**: List all Contentful spaces available
- **publish_entry**: Publish a draft entry
- **unpublish_entry**: Unpublish an entry (return to draft)
- **list_content_types**: List all content types in the current environment
- **list_entries**: List entries in the current environment
- **list_environments**: List environments in the current space
- **list_organizations**: List all Contentful organizations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contentful** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the details and full content for the article titled 'AI Best Practices' from space ID 'xvz1'."

**🤖 AI Agent:**
> Content successfully fetched. The article 'AI Best Practices' in space 'xvz1' is currently marked as a 'Draft'. Here's a brief summary of the text: ... Would you like to update the conclusion paragraph natively?

---

**👤 You:**
> "Fetch the structure schema of our 'Blog Post' content model."

**🤖 AI Agent:**
> Here is the content layout details for 'Blog Post': It holds a 'title' string, a unique 'slug', a 'richText' body implementation, an 'author' internal reference link, and an 'asset' featured image ID. Do you want to prepare a new instance using this schema?

---

**👤 You:**
> "List all environments in our current Contentful space."

**🤖 AI Agent:**
> I've retrieved the environments for your space. You have 'master' (Active), 'staging' (Active), and 'development' (Active). Which environment would you like to use for querying entries?


## ❓ FAQ

**Q: How do I generate a Contentful Personal Access Token?**
Log into your Contentful dashboard. Click on your profile picture in the top right corner and navigate to **Account Settings**. Locate **Personal Access Tokens** and click 'Generate Personal Token'. Copy the value provided.

**Q: Do I need the Space ID to use this integration?**
Yes. Most actions the AI performs require your specific Space ID to target the correct content repository effectively.

**Q: Can the agent interact with unpublished draft entries directly?**
Yes, Contentful's Content Management API (CMA) natively handles internal content regardless of publish state. You can command your AI to fetch, check, or structure a draft before hitting the publish flag explicitly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contentful](https://vinkius.com/mcp/contentful)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contentful** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `contentful` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contentful** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contentful": {
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
