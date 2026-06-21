# DatoCMS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datocms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage headless content via DatoCMS — execute GraphQL queries, handle record CRUD, manage content models, and audit media uploads directly from any AI agent.

## Description
Connect your **DatoCMS** project to any AI agent and take full control of your headless CMS and digital experience platform through natural conversation.

### What you can do

- **GraphQL Discovery** — Identify bounded routing spaces inside the DatoCMS GraphQL tree and extract delivery arrays targeting specific schemas
- **Record Orchestration** — List, retrieve, and create CMS records natively, enforcing JSON:API specifications and item_type validation rules
- **Content Mutation** — Safely update existing records by patching attribute blocks or irreversibly vaporize document nodes to clear internal database limits
- **Media Oversight** — Inspect deep internal arrays of uploaded assets, track Imgix proxy mappings, and verify physical storage identifiers securely
- **Schema Auditing** — Enumerate explicitly registered models and item types defining the structure of your content blocks and editor environments
- **CDA/CMA Integration** — Seamlessly switch between Content Delivery (CDA) for high-performance reading and Content Management (CMA) for structural edits

### How it works

1. Subscribe to this server
2. Enter your DatoCMS Full Access API Token (found in Settings > API Tokens)
3. Start managing your headless content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Editors** — create and update entries or manage media assets without leaving the workspace
- **Front-end Developers** — test GraphQL queries and fetch content model definitions directly from the IDE or chat
- **Product Teams** — monitor content versioning and audit media libraries across different environments
- **Digital Ops** — manage CMS models and verify record consistency through natural language


## Available Tools (10)
- **create_cms_record**: Provision a highly-available JSON Payload generating new content Items
- **wipe_cms_record**: Irreversibly vaporize explicit App nodes dropping live Document rows
- **wipe_media_upload**: Dispatch an automated validation check routing explicit Disk removals
- **get_single_record**: Perform structural extraction of properties driving active Node details
- **get_media_upload**: Retrieve the exact structural matching verifying File blocks
- **execute_graphql_cda**: Identify bounded routing spaces inside the Headless DatoCMS GraphQL tree
- **list_global_models**: Enumerate explicitly attached structured rules exporting Item Types
- **list_cma_records**: Retrieve explicit Cloud logging tracing explicit JSON:API arrays
- **list_media_uploads**: Inspect deep internal arrays mitigating specific Image storage
- **patch_cms_record**: Mutate global Web CRM boundaries substituting Item parameters safely


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DatoCMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all content models in DatoCMS"

**🤖 AI Agent:**
> I found 5 content models: 'Blog Post' (ID: 123), 'Product' (ID: 456), 'Author' (ID: 789), 'Page', and 'Category'. Which model would you like to explore or list records for?

---

**👤 You:**
> "Execute this GraphQL query: '{ allPosts { title } }'"

**🤖 AI Agent:**
> GraphQL query executed! I've retrieved the titles for all posts. Highlights include 'Modern Web Design', 'Intro to DatoCMS', and 'Headless Architecture'.

---

**👤 You:**
> "List the last 5 media uploads"

**🤖 AI Agent:**
> I found 5 recent uploads. The latest is 'hero-banner.jpg' (ID: 999), followed by 'logo-white.png' and 'team-photo.webp'. All assets are being proxied via Imgix for optimization.


## ❓ FAQ

**Q: Can my agent execute custom GraphQL queries against DatoCMS?**
Yes. Use the 'execute_graphql_cda' tool. You can provide any valid GraphQL query string to fetch data from the Content Delivery API (CDA) tree, bypassing rigid limits and retrieving exactly what your agent needs.

**Q: How do I create a new content item using the agent?**
Use the 'create_cms_record' tool. Provide the Item Type ID and a JSON object containing the attributes. The agent will orchestrate the absolute explicit bindings to generate a new record in your DatoCMS project.

**Q: Can I inspect the available content models through chat?**
Absolutely. The 'list_global_models' tool enumerates all registered item types and models. This allows your agent to identify precisely what schemas bind to your editor blocks and which fields are available for data mutations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datocms](https://vinkius.com/mcp/datocms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DatoCMS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `datocms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DatoCMS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "datocms": {
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
