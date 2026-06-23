# LlamaIndex (AI Data Framework & RAG) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/llamaindex-ai-data-framework-rag)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Query and manage RAG pipelines via LlamaIndex — execute natural language searches, audit indexed files, and monitor data pipelines.

## Description
Connect your **LlamaIndex (LlamaCloud)** account to any AI agent and take full control of your RAG data framework and semantic search orchestration through natural conversation.

### What you can do

- **RAG Orchestration** — Execute structural natural language queries directly against your data pipelines to retrieve synthesized answers grounded in your source documents
- **Index Visibility** — List managed active indices wrapping your semantic stores and verify how your data is distributed across indexed databases
- **File Audit** — Retrieve explicit metadata for raw source files currently ingested by your pipelines to verify document tracking and ingestion limits
- **Pipeline Management** — List deployed data pipelines and retrieve detailed configurations including connected sources and embedding settings directly from your agent
- **Project CRM** — Navigate across high-level LlamaIndex projects managing collections of pipelines and queryable semantic search boundaries securely
- **Real-time Synthesis** — Use your agent to perform real-time RAG extraction, ensuring your AI workflows are powered by accurate, indexed enterprise knowledge

### How it works

1. Subscribe to this server
2. Enter your LlamaCloud API Key
3. Start querying your enterprise knowledge from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **RAG Developers** — test semantic search relevancy and query RAG pipelines through natural conversation without writing manual Python boilerplate
- **AI Engineers** — monitor document ingestion statuses and verify indexed file metadata to ensure high-quality fact-grounding for AI agents
- **Data Scientists** — audit semantic index structures and manage data pipeline configurations across multiple enterprise AI projects efficiently


## Available Tools (6)
- **list_pipelines**: List LlamaCloud deployed data pipelines
- **get_pipeline**: Get configuration details for a specific pipeline
- **list_indexes**: List LlamaCloud active indexes
- **query_pipeline**: Execute a natural language query against a specific Pipeline
- **list_files**: List raw source files currently ingested by a pipeline
- **list_projects**: List active LlamaCloud projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LlamaIndex (AI Data Framework & RAG)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Query the 'Product-Docs' pipeline about 'multi-tenant security architecture'"

**🤖 AI Agent:**
> Querying RAG pipeline… Based on your indexed documentation, the multi-tenant architecture uses isolated logical schemas per tenant and mandatory JWT-based attribute filtering at the gateway level. I've found 3 source documents explaining the row-level security implementation. Would you like the links?

---

**👤 You:**
> "List all files ingested by the 'Engineering-Handbook' pipeline (ID: pipe-123)"

**🤖 AI Agent:**
> I've retrieved 15 files from the 'Engineering-Handbook' pipeline. Highlights include 'coding_standards.md', 'deployment_workflow.pdf', and 'api_best_practices.txt'. All files show a status of 'Ingested'. Would you like me to fetch the metadata for 'coding_standards.md'?

---

**👤 You:**
> "What are the active LlamaCloud projects in our organization?"

**🤖 AI Agent:**
> I've identified 3 active LlamaCloud projects: 'Customer-Service-RAG' (ID: proj-001), 'Internal-Knowledge-Base' (ID: proj-005), and 'Market-Analysis-Tools' (ID: proj-008). Each project manages its own set of pipelines and indices. Which one would you like to explore?


## ❓ FAQ

**Q: Can I query my indexed documents using natural language through my agent?**
Yes. Use the `query_pipeline` tool by providing the Pipeline ID and your natural language question. Your agent will trigger a real-time RAG extraction and return a synthesized answer based on the relevant source documents found in the index.

**Q: How do I check which files have been successfully ingested into a pipeline?**
The `list_files` tool allows your agent to retrieve explicit metadata for all physical documents attached to a pipeline. This is perfect for auditing your data source boundaries and ensuring all required documents are correctly indexed.

**Q: Can my agent manage multiple semantic indices?**
Absolutely. Use the `list_indexes` tool to see all active semantic stores managed by LlamaCloud. Your agent will report the index names and types, making it easy to identify the correct target for your search or ingestion workflows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/llamaindex-ai-data-framework-rag](https://vinkius.com/mcp/llamaindex-ai-data-framework-rag)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LlamaIndex (AI Data Framework & RAG)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `llamaindex-ai-data-framework-rag` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LlamaIndex (AI Data Framework & RAG)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "llamaindex-ai-data-framework-rag": {
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
