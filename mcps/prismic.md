# Prismic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prismic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Query and manage your Prismic headless CMS content — search documents, list custom types, and retrieve specific content directly from any AI agent.

## Description
Connect your **Prismic** headless CMS to any AI agent and integrate content querying directly into your conversation workflow.

### What you can do

- **Search Documents** — Perform advanced searches using Prismic predicates, filter by tags, locales, and custom types
- **Retrieve Content** — Fetch full document data by their unique IDs to immediately get component architecture and copy
- **Explore Schema** — List all available custom types, tags, and languages defined in your repository
- **Analyze Structure** — Retrieve repository metadata including master refs and view specific query form schemas

### How it works

1. Subscribe to this server
2. Enter your Prismic Repository Name and optional Access Token
3. Start fetching and analyzing your CMS content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — query documents and components exactly as they return from the API directly inside your IDE without context switching
- **Content Managers** — quickly audit tags, find specific document IDs, and verify translations without opening the Prismic dashboard
- **SEO Specialists** — inspect live structured data, slugs, and copy for specific pages in seconds


## Available Tools (10)
- **list_i18n_languages**: Lists the languages (locales) configured in the repository
- **list_global_tags**: Lists all tags used across the Prismic repository
- **list_custom_types**: Lists all Custom Types defined in the Prismic repository
- **list_documents_by_tag**: Lists all Prismic documents that have a specific tag
- **list_documents_by_type**: Lists all Prismic documents of a specific Custom Type
- **query_prismic_documents**: This is the most powerful tool for finding content. It supports pagination and locale filtering internally.

Queries the Prismic API for documents using raw Predicates
- **search_filtered_locale**: g., "en-us" or "fr-fr").

Performs a filtered search for documents within a specific locale
- **get_repo_metadata**: Retrieves metadata about the Prismic repository, including master refs, types, and languages
- **get_document_by_id**: g., from a search result or relationship field) and need to retrieve its full content.

Fetches a specific Prismic document by its unique ID
- **get_query_form_schema**: Retrieves the schema for a specific query form (e.g., "everything")


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prismic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all custom types available in my Prismic repository."

**🤖 AI Agent:**
> I found 4 custom types in your repository: 'homepage', 'blog_post', 'author', and 'navigation'. Would you like me to fetch a few documents of type 'blog_post' to check out the structure?

---

**👤 You:**
> "Can you fetch the document JSON for the ID 'ZbHwWxEAACUAx9'?"

**🤖 AI Agent:**
> Here is the full JSON payload for document 'ZbHwWxEAACUAx9'. It is a 'page' type with the slug 'about-us'. I can generate a Next.js component to map this slice structure if you'd like.

---

**👤 You:**
> "Search for all documents tagged with 'seo' and 'landing'."

**🤖 AI Agent:**
> I performed a search using Prismic predicates for the tags 'seo' and 'landing'. The API returned 12 documents. They are mostly of type 'article'. Want to see the titles of the first 5 results?


## ❓ FAQ

**Q: How do I start extracting content from my Prismic repository?**
Subscribe, enter your Prismic Repository Name, and if your repository is private, grab an Access Token from **Settings → API & Security**. No manual SDK setups or GraphQL integrations — just connect and start querying your custom types and documents directly through your AI agent.

**Q: Can my AI agent help me build Next.js components matching my Custom Types?**
Yes! Ask your agent to query a specific document ID or list custom types. It will retrieve the exact JSON payload returned by the Prismic API. Based on that structure, the agent can instantly generate your Next.js/React component props, mock data, and TS interfaces natively inside Cursor.

**Q: What happens when I need to find all blog posts tagged with 'announcement' in French?**
Just ask your AI agent. It uses the `search_filtered_locale` tool and Prismic predicates to filter documents precisely by type, tag, and language code without requiring you to manually craft complex API query strings or write ad-hoc fetch scripts.

**Q: Does it support deep repository insights for large content websites?**
Absolutely. You can list all custom types, pull an array of all global tags, and verify all configured languages for multi-lingual websites. It acts as an instant audit tool for publishers, content operations teams, and architects managing extensive CMS architectures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prismic](https://vinkius.com/mcp/prismic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prismic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prismic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prismic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prismic": {
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
