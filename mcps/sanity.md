# Sanity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sanity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Sanity Content Lake via AI — execute GROQ queries, manage documents, and handle media assets directly from your agent.

## Description
Connect your **Sanity** project to any AI agent and take full control of your Content Lake through natural conversation.

### What you can do

- **GROQ Queries** — Execute powerful Graph-Relational Object Queries to fetch exactly the content you need
- **Document Management** — Create, read, update, patch, and delete documents of any schema type
- **Schema Insights** — List unique schema types and count entity nodes dynamically
- **Media Assets** — Browse and manage images and file assets uploaded to your project
- **Bulk Operations** — Run raw Sanity mutations for complex, multi-document transactions

### How it works

1. Subscribe to this server
2. Enter your Sanity Project ID, Dataset, API Version, and API Token
3. Start managing your content from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a headless CMS power-user, perfectly capable of navigating references and transforming content on the fly.

### Who is this for?

- **Developers** — prototype GROQ queries, audit schema types, and run quick data migrations
- **Content Editors** — bulk edit fields, update taxonomy, and manage assets without leaving your chat
- **Product Managers** — query content stats and generate instant reports on published vs. draft documents


## Available Tools (10)
- **list_typed_documents**: g., "post", "author").

Lists all documents of a specific type
- **count_entity_nodes**: Counts the number of documents of a specific type
- **list_unique_schema_types**: Retrieves a list of all unique document types present in the dataset
- **create_cms_document**: Specify the type and provide attributes as a JSON object.

Creates a new document in the CMS
- **get_document_details**: Retrieves full details for a specific document by ID
- **list_media_assets**: Lists all image and file assets uploaded to Sanity
- **patch_cms_document**: Provide a JSON object of fields to set.

Updates specific fields of an existing document
- **run_groq_query**: Executes a GROQ (Graph-Relational Object Queries) query
- **run_raw_mutation**: Provide a JSON array of mutation objects.

Executes a raw Sanity mutation
- **wipe_cms_document**: This action is irreversible.

Permanently deletes a document from the CMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sanity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all unique schema types in my dataset."

**🤖 AI Agent:**
> I checked your schema types. Your dataset contains the following 5 types: `post`, `author`, `category`, `product`, and `siteSettings`. Would you like to know how many documents exist for a specific type?

---

**👤 You:**
> "Write a GROQ query to find the 3 most recently updated authors."

**🤖 AI Agent:**
> I executed the GROQ query `*[_type == 'author'] | order(_updatedAt desc)[0...3]`. The most recently updated authors are: 1. Sarah Chen, 2. Marcus Rivera, 3. Alex Nguyen. Should I retrieve their full biographical details?

---

**👤 You:**
> "Update the post with ID 'drafts.1234' and set its published state to true."

**🤖 AI Agent:**
> I've successfully patched document 'drafts.1234'. The field `isPublished` is now set to `true`. The change is immediately live in your Content Lake.


## ❓ FAQ

**Q: Can my AI agent write complex GROQ queries for me?**
Yes. If you know what data you want but aren't totally familiar with GROQ syntax, you can simply ask your agent: 'Write and execute a GROQ query to find all author documents where the name starts with John and return just their ID and bio.' The agent will draft the query, execute it via the `run_groq_query` tool, and return the filtered JSON.

**Q: How do I perform a bulk update on my documents?**
You can ask your agent to first fetch the documents (e.g., 'List all posts missing a category'), calculate the changes needed, and then use the `run_raw_mutation` tool or `patch_cms_document` iteratively to apply the updates. This acts as a conversational migration script, updating dozens of documents safely and quickly.

**Q: Can the agent check if media assets are missing from my posts?**
Yes. The agent can use the document querying tools combined with `list_media_assets` to analyze your content. For instance, you can ask it to generate a report of all products that do not have an associated image reference, giving you an exact list of items to fix in the Studio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sanity](https://vinkius.com/mcp/sanity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sanity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sanity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sanity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sanity": {
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
