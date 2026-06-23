# R2R MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/r2r)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Equip your AI with direct access to your R2R engine — execute vector searches, run precise RAG queries, and manage your documents.

## Description
Connect your **R2R (Rag to Riches)** deployment to an AI agent, bringing your RAG infrastructure inside your chat interface. By linking this server, the AI can query its own constructed knowledge base on demand.

### What you can do

- **Vector Search** — Perform semantic similarity queries across your document database to retrieve contextually relevant chunks of information.
- **Execute RAG Queries** — Use the 'rag_query' endpoint to have the R2R server directly summarize information based on vector data.
- **Knowledge Management** — Call the API to list ingested documents, read metadata attributes, and filter logical collections.
- **Instance Health Monitoring** — Quickly ping the connection using health checks to verify your system is responsive.

### How it works

1. Enable the server integration.
2. Provide your active R2R Base URL and Auth Key (if applicable).
3. Trigger RAG requests natively within your supported chat interfaces.

### Who is this for?

- **AI & ML Engineers** — Query your vector instances locally without needing Postman or external scripts.
- **Data Custodians** — Quickly verify document ingestions and browse metadata directly inside the terminal.
- **Backend Developers** — Audit engine responses and fine-tune semantic retrieval limits easily.


## Available Tools (6)
- **search**: Performs a vector search across ingested documents
- **rag_query**: Executes a RAG (Retrieval-Augmented Generation) query
- **list_documents**: Lists all ingested documents in the R2R system
- **get_document**: Retrieves details for a specific document
- **list_collections**: Lists all document collections
- **get_health**: Checks the health status of the R2R server


## 💬 Prompt Examples

Here are some examples of how you can interact with the **R2R** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Perform a vector search for 'Company Holiday Policy 2026'."

**🤖 AI Agent:**
> Using the R2R server, I found 3 highly relevant snippets. The top hit from document `doc_7712a` states: 'In 2026, employees are granted 21 flexible floating days, bypassing old blackout windows.'

---

**👤 You:**
> "Query the RAG engine to summarize known advanced RAG chunking strategies."

**🤖 AI Agent:**
> I requested the summary directly from R2R via `rag_query`. The engine replied: 'Advanced strategies focus on semantic segmentation rather than standard character limits, utilizing markdown structure, sentence boundaries, and logical overlaps to retain context.'

---

**👤 You:**
> "Verify the operational health of the R2R server."

**🤖 AI Agent:**
> I executed the `get_health` probe. The R2R server replied with `status: ok` and is primed to accept vector operations.


## ❓ FAQ

**Q: What URL should I use for the R2R API URL?**
If you are running R2R locally via Docker, it's typically `http://localhost:7272`. If you are using SciPhi Cloud or have it deployed on your own infrastructure, provide the exact public or private endpoint.

**Q: Do I need an R2R API Key?**
It depends on your deployment. Open deployments for local testing may not require a key. Production deployments or SciPhi Cloud environments require you to provide the generated key.

**Q: What is the difference between RAG and Search?**
The `search` tool issues a standard vector similarity match—it returns relevant raw snippets from your database. The `rag_query` tool asks the R2R server to perform the search and compute an intelligent answer wrapping those snippets using an LLM.

**Q: Are document ingestions possible via chat?**
No. This integration is designed for observational toolsets (listing documents, inspecting states, querying the index). Heavy ingestions of PDFs or websites should be handled through scripts or the dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/r2r](https://vinkius.com/mcp/r2r)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **R2R** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `r2r` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **R2R** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "r2r": {
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
