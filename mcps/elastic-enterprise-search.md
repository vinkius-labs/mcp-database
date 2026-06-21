# Elastic Enterprise Search MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elastic-enterprise-search)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage enterprise search via Elastic — search engines and documents, handle indexing, and monitor search analytics directly from any AI agent.

## Description
Connect your **Elastic Enterprise Search** deployment to any AI agent and take full control of your application search engines and workplace discovery through natural conversation.

### What you can do

- **Engine Orchestration** — Iterate through explicit engine containers managing logical indexing schemas and search spaces completely
- **Search & Discovery** — Resolve semantic or literal queries enforcing deep contextual matches against structured enterprise scopes seamlessly
- **Document Indexing** — Command explicit bulk payload ingestions triggering native pipeline mappings to store and update document collections synchronously
- **Metadata Inspection** — Analyze specific global bounds fetching discrete index layouts and extracting linguistic configuration nodes cleanly
- **Analytics Auditing** — Generate precise internal metric tracking isolating usage insights and calculating exact click log data to monitor performance
- **Catalog Retrieval** — Extract explicitly attached REST arrays mapping exact document payloads fetching physical raw records flawlessly

### How it works

1. Subscribe to this server
2. Enter your Elastic Enterprise Search URL and API Key (found in Kibana > Stack Management > Security > API Keys)
3. Start managing your search engines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Search Engineers** — monitor engine configurations and test search relevance without manual API testing
- **Software Developers** — index documents and verify search results directly from the IDE or chat
- **Data Analysts** — audit search analytics and monitor click logs using natural language conversation
- **Ops Teams** — verify engine health and manage document indexing pipelines in real-time


## Available Tools
- **list_engines**: List engines
- **get_engine**: Get engine
- **search**: Search documents within an engine
- **list_documents**: List indexed documents in an engine
- **index_documents**: Index newly created JSON documents targeting specific schemas
- **analytics**: Get search analytics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elastic Enterprise Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all search engines in my Elastic deployment"

**🤖 AI Agent:**
> I found 3 engines: 'e-commerce-products', 'help-center-docs', and 'blog-posts'. Would you like to see the configuration or search documents in any of these?

---

**👤 You:**
> "Search for 'api integration' in engine 'help-center-docs'"

**🤖 AI Agent:**
> Searching 'help-center-docs'... I found 5 matching documents. The most relevant is 'REST API Authentication Guide' (Score: 12.5). I can retrieve the full text or metadata for you.

---

**👤 You:**
> "Show me search analytics for engine 'e-commerce-products'"

**🤖 AI Agent:**
> Retrieving analytics for 'e-commerce-products'... In the last 7 days, there were 5,000 queries with an 8% click-through rate. Top queries: 'shoes', 'backpack', 't-shirt'. Would you like a more detailed breakdown?


## ❓ FAQ

**Q: Can my agent list all available search engines in Elastic?**
Yes. Use the 'list_engines' tool. The agent iterates through your engine containers, managing logical indexing schemas and providing a complete map of your search spaces.

**Q: How do I index a batch of JSON documents via chat?**
Use the 'index_documents' tool. Provide the engine name and a JSON array of your documents. The agent will command the bulk payload ingestion, triggering native pipeline mappings to store your data synchronously.

**Q: Can I check the search analytics for a specific engine through the agent?**
Absolutely. The 'analytics' tool generates precise internal metric tracking for your engine. It will isolate usage insights and calculate click log data, allowing you to monitor search performance natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elastic-enterprise-search](https://vinkius.com/mcp/elastic-enterprise-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elastic Enterprise Search** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `elastic-enterprise-search` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elastic Enterprise Search** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elastic-enterprise-search": {
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
