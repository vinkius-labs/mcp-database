# Webiny CMS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webiny-cms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage content models, entries, and GraphQL workflows on Webiny — the enterprise open-source headless CMS.

## Description
Connect your **Webiny CMS** instance to any AI agent and manage your headless content infrastructure through natural conversation.

### What you can do

- **Content Lifecycle** — Create, update, publish, and delete content entries for any model directly from your agent
- **Model Discovery** — List all entries for specific content models and browse available data structures using introspection
- **Advanced GraphQL** — Execute raw GraphQL queries or mutations for custom logic and complex nested data operations
- **Revision Control** — Retrieve specific entry details by ID to inspect metadata and field-level property values
- **API Management** — Discover available types, fields, and models in your current environment through automated introspection
- **Global Config** — Verify high-level tenant settings and configurations to ensure your CMS environment is healthy
- **Multi-Locale Support** — Seamlessly manage content across different language locales (e.g., en-US, pt-BR)

### How it works

1. Subscribe to this server
2. Enter your Webiny API Domain and Access Token
3. Start managing your content models through Claude, Cursor, or any MCP-compatible client

No more manual JSON drafting in GraphQL playgrounds. Your AI agent becomes your content operations manager.

### Who is this for?

- **Content Managers** — update and publish entries across multiple models and locales without manual data entry
- **Headless Developers** — test GraphQL queries and verify content model introspection through chat
- **Marketing Teams** — quickly browse content items and verify publication status for different campaigns
- **CMS Administrators** — monitor tenant settings and audit content revisions through simple commands


## Available Tools
- **create_cms_entry**: Provide the singular model name and field data as a JSON object.

Creates a new draft entry for a content model
- **delete_cms_entry**: This action is irreversible.

Permanently deletes a content entry revision
- **execute_graphql_query**: Specify api_type (manage, read, preview) and locale.

Executes a raw GraphQL query or mutation against the Webiny CMS API
- **get_api_introspection**: Retrieves the GraphQL schema introspection for the Webiny instance
- **get_model_entry_details**: ID refers to the specific revision.

Retrieves details for a specific content model entry
- **get_tenant_config**: Retrieves global settings for the Webiny tenant
- **list_model_entries**: Provide the model plural name (e.g. "Articles"). Specify api_type (manage for drafts, read for live).

Lists all entries for a specific content model in Webiny
- **publish_cms_entry**: Provide the specific revision ID.

Publishes a draft entry, making it available via the "read" API
- **update_cms_entry**: Provide the entry ID and a JSON object containing the field updates.

Updates fields of an existing content entry revision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Webiny CMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all entries for the 'BlogPosts' model in en-US."

**🤖 AI Agent:**
> I found 8 entries in 'BlogPosts': 1. 'Introduction to Headless CMS' (ID: post-1), 2. 'Getting Started with Webiny' (ID: post-2), 3. 'GraphQL Best Practices' (ID: post-3), and 5 others. Which one would you like to see details for?

---

**👤 You:**
> "Create a new 'Author' entry: { 'name': 'John Doe', 'bio': 'Tech Writer' } in en-US."

**🤖 AI Agent:**
> Success! I've created a new draft entry for 'Author' (ID: auth-999) with the provided details. Would you like me to publish it now?

---

**👤 You:**
> "Publish the entry with ID 'post-123' for model 'Article'."

**🤖 AI Agent:**
> I've successfully published the 'Article' entry (ID: post-123). It is now live and accessible via your Read API. Is there anything else you'd like to update?


## ❓ FAQ

**Q: Can I publish a draft content entry via chat?**
Yes. The `publish_cms_entry` tool allows you to take any draft revision live. You just need to provide the entry ID and the model name, and your AI agent will handle the publication through the Webiny 'manage' API.

**Q: Is it possible to see the entire GraphQL schema of my instance?**
Absolutely. Using the `get_api_introspection` tool, your agent can retrieve the full GraphQL schema introspection, giving you a complete overview of all available types, fields, and content models in your environment.

**Q: How do I add a new entry to a content model through conversation?**
Use the `create_cms_entry` tool. Provide the singular model name (e.g., 'Article'), the target locale, and a JSON object containing the field data. Your agent will create the new draft entry instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webiny-cms](https://vinkius.com/mcp/webiny-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Webiny CMS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `webiny-cms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Webiny CMS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "webiny-cms": {
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
