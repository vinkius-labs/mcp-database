# GraphQL Fragment Merger MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/graphql-fragment-merger)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deterministically inlines GraphQL fragments into a single query string.

## Description
The GraphQL Fragment Merger solves the problem of AI agents sending fragmented queries to servers that do not support fragment spreads. By using `merge_graphql_fragments`, you can provide a raw GraphQL query containing spread operators (...FragmentName) and fragment definitions. The tool recursively identifies these fragments and replaces every spread with its exact body fields using deterministic string manipulation. This ensures the resulting `merged_query_string` is a single, valid, and complete GraphQL operation, making it compatible with any standard GraphQL endpoint.


## Available Tools (1)
- **merge_graphql_fragments**: Inlines GraphQL fragments into the main query deterministically


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GraphQL Fragment Merger** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Merge this GraphQL query: 'query { user { ...UserFields } } fragment UserFields on User { id name }'"

**🤖 AI Agent:**
> query { user { id name } }

---

**👤 You:**
> "Can you inline fragments for this query?"

**🤖 AI Agent:**
> Please provide the GraphQL query string you would like me to process using `merge_graphql_fragments`.

---

**👤 You:**
> "Check if these fragments are correctly merged: 'query { node { ...Node } } fragment Node on Node { id }'"

**🤖 AI Agent:**
> The merged query is: query { node { id } }


## ❓ FAQ

**Q: What does the `merge_graphql_fragments` tool actually do?**
It takes a GraphQL query string with fragments and returns a single, flattened query string where all fragment spreads have been replaced by their actual field definitions.

**Q: Does it support nested fragments?**
Yes, the tool recursively processes fragment definitions to ensure all levels of nesting are resolved into the final query string.

**Q: What happens if a fragment is not defined?**
The tool will return the `merged_query_string` as processed so far, along with an `unresolved_fragments` list containing the names of the missing fragments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/graphql-fragment-merger](https://vinkius.com/mcp/graphql-fragment-merger)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GraphQL Fragment Merger** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `graphql-fragment-merger` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GraphQL Fragment Merger** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "graphql-fragment-merger": {
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
