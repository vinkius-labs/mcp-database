# Hygraph (Headless CMS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hygraph-headless-cms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage headless content via Hygraph — execute GraphQL queries, introspect schemas, and manage documents.

## Description
Connect your **Hygraph** project to any AI agent and take full control of your federated content and headless CMS architecture through natural conversation.

### What you can do

- **GraphQL Orchestration** — Execute complex nested queries and mutations directly from your agent to fetch or update structured content without manual REST endpoints
- **Schema Introspection** — Discover content models and list available fields to understand your project's data structure and scalar parameters automatically
- **Document Lifecycle** — Create, update, and publish CMS documents, moving content from Draft to Published stages with precise ID targeting
- **Media Management** — Enumerate media assets and retrieve secure handles and cloud URLs required for frontend delivery and display
- **Localization Audit** — List project locales and translation spaces to identify which content stages are mapped to specific internationalization rules
- **Cleanup Operations** — Irreversibly delete specific content nodes and documents to maintain a clean and optimized content repository

### How it works

1. Subscribe to this server
2. Enter your Hygraph API Endpoint and Auth Token
3. Start managing your content architecture from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — test GraphQL queries and introspect content models without leaving your IDE or opening the Hygraph Playground
- **Content Architects** — audit schema definitions and verify field configurations across multiple content models through natural conversation
- **Digital Editors** — create and publish draft content quickly by commanding your AI agent to update specific document fields


## Available Tools
- **create_cms_document**: Dispatch an automated validation check routing Dynamic Model creation
- **wipe_cms_document**: Irreversibly vaporize explicit Content arrays returning clean states
- **list_project_locales**: Identify precise active arrays spanning Translation spaces
- **get_model_fields**: Inspect deep internal arrays mitigating specific Content configurations
- **list_schema_introspection**: types` executing an introspection determining automatically which Models the Project hosts.

Retrieve explicit Cloud logging tracing Model names
- **list_media_assets**: Enumerate explicitly attached structured rules defining Media limits
- **publish_cms_document**: Perform structural extraction of properties driving an explicit Live shift
- **execute_graphql_mutation**: Provision a highly-available JSON Payload resolving direct Schema writes
- **execute_graphql_query**: Identify bounded routing spaces inside the Headless Hygraph limits using pure GraphQL
- **update_cms_document**: Mutate global Web CRM boundaries substituting Draft values safely


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hygraph (Headless CMS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all content models in my project"

**🤖 AI Agent:**
> I've performed a schema introspection. Your project contains 8 content models including 'BlogPost', 'Author', 'Category', 'Product', and 'CustomerReview'. Which one would you like to inspect?

---

**👤 You:**
> "Show me the fields for the 'BlogPost' model"

**🤖 AI Agent:**
> The 'BlogPost' model has the following fields: 'title' (String), 'slug' (String), 'content' (RichText), 'author' (Relation to Author), 'publishedDate' (DateTime), and 'coverImage' (Asset). Would you like to create a new draft post?

---

**👤 You:**
> "Execute a query to get the title and slug of the last 3 published posts"

**🤖 AI Agent:**
> Running GraphQL query… I've retrieved the last 3 posts: 1) 'AI in 2024' (slug: ai-2024), 2) 'Mastering Hygraph' (slug: mastering-hygraph), and 3) 'Headless CMS Trends' (slug: cms-trends). All are currently in the PUBLISHED stage.


## ❓ FAQ

**Q: Can I test complex GraphQL queries through my agent?**
Yes. Use the `execute_graphql_query` tool to run any valid GraphQL query block. Your agent will return the nested document results, making it an ideal way to verify content fetching without using the Hygraph Playground.

**Q: How do I publish a draft document using my agent?**
The `publish_cms_document` tool allows your agent to shift a document's stage from DRAFT to PUBLISHED. You just need to provide the Model Name and the Target UUID to make the content live on your frontend.

**Q: Can I see all available fields for a specific content model?**
Absolutely. Use the `get_model_fields` tool with the name of your Model (e.g., 'Post' or 'Product'). Your agent will perform a schema introspection and list all fields, types, and scalar parameters defined in that model.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hygraph-headless-cms](https://vinkius.com/mcp/hygraph-headless-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hygraph (Headless CMS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hygraph-headless-cms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hygraph (Headless CMS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hygraph-headless-cms": {
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
