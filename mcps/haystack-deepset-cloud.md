# Haystack (deepset Cloud) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/haystack-deepset-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Build and manage AI-powered search and RAG pipelines via deepset Cloud — search documents, run pipelines, and manage workspaces.

## Description
Connect your **deepset Cloud** account to any AI agent and manage your Haystack-powered RAG pipelines through natural conversation.

### What you can do

- **Workspaces** — List and manage isolated environments for different search contexts
- **Pipelines** — Visualize NLP topologies, including embedding nodes and retriever logic
- **Run Search** — Dispatch immediate LLM or Retriever invocations to test RAG pipelines
- **Document Management** — List files and inspect metadata attached to source document embeddings
- **Vector Search** — Trigger dense or sparse vector searches over indexed enterprise knowledge

### How it works

1. Subscribe to this server
2. Enter your deepset Cloud API URL and API Key
3. Start managing your AI pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI/ML Teams** — quickly audit pipeline configurations and test search results
- **RAG Developers** — integrate enterprise knowledge bases with AI agents for contextual answers
- **Product Managers** — monitor search performance and verify document indexing status


## Available Tools
- **list_workspaces**: List workspaces
- **list_pipelines**: List pipelines
- **get_pipeline**: Get pipeline details
- **run_pipeline**: Run a pipeline search
- **list_files**: List uploaded files
- **get_file**: Get file metadata
- **search_documents**: Search documents in index


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Haystack (deepset Cloud)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pipelines in my 'production' workspace"

**🤖 AI Agent:**
> I found 3 pipelines in your production workspace: 'default-rag', 'semantic-search', and 'hybrid-retriever'. Which one would you like to inspect?

---

**👤 You:**
> "Run a search for 'AI security compliance' using the default-rag pipeline"

**🤖 AI Agent:**
> Running search… Based on your indexed documents, I found 5 relevant snippets. The main compliance requirements are… [results summary]. Would you like to see the source file IDs?

---

**👤 You:**
> "List the files in my 'knowledge-base' workspace"

**🤖 AI Agent:**
> You have 12 files in the 'knowledge-base' workspace. Recent uploads include 'q4_report.pdf', 'security_guidelines.md', and 'api_docs.txt'. I can fetch metadata for any of these files.


## ❓ FAQ

**Q: Can I test my RAG pipelines directly via my AI agent?**
Yes. Use the `run_pipeline` tool to dispatch a query to any registered pipeline in your workspace. Your agent will return the response from the NLP topology, allowing you to verify retriever performance and LLM grounding without leaving your workspace.

**Q: How can I audit my document indexing status?**
Ask your agent to list files in your workspace. You can then get specific metadata for any file to ensure embeddings and attributes are correctly attached. This is essential for debugging retrieval issues in production environments.

**Q: Is it possible to manage multiple deepset Cloud workspaces?**
Absolutely. The agent provides high-level workspace listing, allowing you to navigate across tenant boundaries and isolation zones easily. You just need to provide the workspace name to any pipeline or search command.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/haystack-deepset-cloud](https://vinkius.com/mcp/haystack-deepset-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Haystack (deepset Cloud)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `haystack-deepset-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Haystack (deepset Cloud)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "haystack-deepset-cloud": {
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
