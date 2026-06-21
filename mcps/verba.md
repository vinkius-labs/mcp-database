# Verba MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/verba)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Connect your Verba RAG platform to your AI agent. Search your documents, retrieve semantic answers, and manage your Weaviate knowledge base directly.

## Description
Intertwine the open-source **Verba** (by Weaviate) ecosystem natively into your conversational AI IDE. Execute powerful Retrieval-Augmented Generation processes and manage your localized knowledge bases simply by chatting.

### What you can do

- **Augmented Queries** — Cast a question to your agent and have it retrieve fully synthesized answers from the Verba engine completely backed up by exact document citations.
- **Knowledge Management** — Insert new context text, list all ingested documents, retrieve the deeply embedded raw data of any ID, or remove dead knowledge dynamically without Web UIs.
- **Health Checks** — Request system configurations directly via chat to ensure your local LLM connections, embedding models, and cluster health are firing effectively.

### How it works

1. Ensure your local or cloud Verba instance is running
2. Supply your Verba API URL and API Key (if authenticated)
3. Ask Claude or Cursor to query, retrieve, or insert document structures intuitively.

### Who is this for?

- **RAG Developers** — quickly add or delete text chunks to evaluate changes in embedding fidelity directly inside your IDE coding session.
- **Knowledge Managers** — query your dense technical manuals using semantic search and receive the verified text snippets instantly.
- **Open Source Hobbyists** — orchestrate your personal Weaviate/Verba RAG stacks strictly through the programmatic conversational layer.


## Available Tools
- **add_knowledge_document**: Provide the document content and optional metadata JSON.

Ingests a new document into the Verba knowledge base
- **delete_knowledge_document**: This action is irreversible.

Permanently removes a document from the knowledge base
- **get_document_details**: Retrieves the full content and metadata of a specific document
- **get_system_config**: Retrieves the current Verba system configuration
- **list_knowledge_documents**: Lists all documents indexed in the Verba knowledge base
- **perform_rag_query**: Returns summarized answers with citations.

Executes a RAG (Retrieval Augmented Generation) query against the Verba knowledge base


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Verba** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check Verba's configuration to see which embedding model it is currently using."

**🤖 AI Agent:**
> I've retrieved your Verba system configuration. The engine is properly spun up and indicates that it is currently utilizing the 'MiniLM-v12' embedding model localized naturally. All systems appear nominal for retrieval.

---

**👤 You:**
> "Perform a RAG query asking: 'What are our key deployment steps based on the infrastructure guide?'"

**🤖 AI Agent:**
> Result from Verba Knowledge Base: 

*"According to the 'Infrastructure Deployment v2' document, there are three key steps for deployment: 1) Initiate pre-flight health checks via CI/CD, 2) Provision ephemeral node pods for shadow tests, and 3) Cutover traffic using a blue-green weighting swap mechanism."*

*(Source Citations: DocId: xfA-21v - confidence: 0.96)*

---

**👤 You:**
> "List all documents and output the unique ID of the 'Employee Code of Conduct' file."

**🤖 AI Agent:**
> I've queried the document catalog. You have 15 items overall. The specific 'Employee Code of Conduct' document is indexed under the Document ID `5fcbeb99-xxxx`. Would you like me to delete it or replace its contents with a new updated chunk?


## ❓ FAQ

**Q: Can I query my local Verba instance directly through Cursor?**
Yes! Once you configure `VERBA_API_URL` to point to `http://localhost:8000` (or your host port), you can prompt your AI assistant to execute rigorous `perform_rag_query` instructions without ever breaking your developer focus.

**Q: How do I insert fresh text data into Verba completely using conversational chat?**
Provide the agent with your desired context directly. For example: `Add this chunk of markdown as a new document to Verba: '# Title 
 Content...'`. The agent leverages `addDocumentTool`, serializes the payload, and commits it into Verba's vector store immutably.

**Q: Are the query answers backed by citations from its embedded documents?**
Absolutely. That's the primary benefit of the integration. When you run `perform_rag_query`, Verba utilizes Weaviate's hybrid search mechanics. The output explicitly includes natural language synthesis backed by the unique document IDs and snippet texts it referenced.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/verba](https://vinkius.com/mcp/verba)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Verba** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `verba` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Verba** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "verba": {
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
