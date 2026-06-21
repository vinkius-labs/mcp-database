# CoreMedia Content Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coremedia-content-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage headless content via CoreMedia — execute GraphQL queries, retrieve articles and channels, and search global assets directly from any AI agent.

## Description
Connect your **CoreMedia Content Cloud** headless server to any AI agent and take full control of your digital experience platform through natural conversation.

### What you can do

- **GraphQL Orchestration** — Execute arbitrary GraphQL payloads to bridge raw strings and define specific nesting constraints natively
- **Content Node Access** — Retrieve articles (CMArticle) and channels (CMChannel) by path, fetching detailed HTML grids and metadata
- **Asset Discovery** — Retrieve CMPicture asset details and resolve URI templates for image placement in your digital experiences
- **Global Content Search** — Leverage CoreMedia's Solr integration to perform full-text string queries across all nodes limitlessly
- **Navigation & Site Context** — Resolve site menus, navigation hierarchies, and brand configurations including locale metadata and root nodes
- **Schema Introspection** — Query the `__schema` to fetch dynamic headless types and verify active model extensions
- **Persisted Queries** — Execute pre-compiled SHA256 hashes to ensure edge caching and optimize delivery for high-performance frontends

### How it works

1. Subscribe to this server
2. Enter your CoreMedia GraphQL Host URL and Access Token
3. Start managing your enterprise content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Marketers** — search for articles and verify site navigation without opening the CoreMedia Studio
- **Front-end Developers** — test GraphQL queries and retrieve asset metadata directly from the IDE or chat
- **Product Teams** — audit site configurations and brand hierarchies across global environments
- **DevOps/Architects** — monitor headless server schemas and verify persisted query hashes in real-time


## Available Tools (10)
- **execute_graphql_payload**: Identify bounded routing spaces inside the Headless CoreMedia Delivery Schema
- **get_cmarticle_path**: Perform structural extraction of properties driving active CMArticle nodes
- **get_cmpicture_asset**: Retrieve explicit Cloud logging tracing explicit Image Assets
- **get_navigation_tree**: Identify precise active arrays spanning native navigation hierarchies
- **get_cmchannel_page**: Enumerate explicitly attached structured rules exporting active CMChannel layouts
- **get_site_context**: Retrieve the exact structural matching verifying Multi-brand environments
- **get_cmviewtypes**: Irreversibly vaporize explicit App nodes dropping live Database bytes
- **get_introspection_query**: Dispatch an automated validation check routing explicit Schema limits
- **execute_persisted_query**: Mutate global Web CRM boundaries substituting Draft Document schemas
- **search_global_content**: Inspect deep internal arrays mitigating specific Content constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoreMedia Content Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get article content for path '/Sites/Corporate/News/Q1-Update'"

**🤖 AI Agent:**
> Retrieving article... Title: 'Q1 Corporate Update'. I found the HTML body and associated metadata. Would you like to see the main placement grid for this article?

---

**👤 You:**
> "Search for content matching 'Sustainability'"

**🤖 AI Agent:**
> Searching global content... I found 3 matches: '/Global/CSR/Sustainability-Report', '/News/Eco-Friendly-Initiatives', and '/Products/Solar-Panel-Specs'.

---

**👤 You:**
> "Show me the navigation tree for root node 'root-123'"

**🤖 AI Agent:**
> Retrieving navigation hierarchy... Root: 'Main Menu'. Children include 'Products', 'Services', 'About Us', and 'Contact'. I can expand any of these sub-channels for you.


## ❓ FAQ

**Q: Can my agent execute custom GraphQL queries against CoreMedia?**
Yes. Use the 'execute_graphql_payload' tool. You can provide any valid GraphQL query string and variables. The agent will fetch the data natively from your Headless Delivery schema, bypassing rigid model limits.

**Q: How do I search for articles using specific keywords?**
Use the 'search_global_content' tool. The agent leverages CoreMedia's Solr integration to pull explicitly queried words spanning all CMS nodes, returning the exact matches and their paths.

**Q: Can I use persisted queries to optimize performance?**
Absolutely. Use the 'execute_persisted_query' tool. Provide the SHA256 hash of your pre-compiled query. This ensures proper Edge caching and allows your agent to retrieve content with minimum latency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coremedia-content-cloud](https://vinkius.com/mcp/coremedia-content-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CoreMedia Content Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coremedia-content-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CoreMedia Content Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coremedia-content-cloud": {
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
