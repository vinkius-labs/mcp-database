# VectorShift (AI Workflow & RAG Automation) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vectorshift-ai-workflow-rag-automation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Automate AI workflows and RAG via VectorShift — manage pipelines, query knowledge bases, and deploy chatbots directly from any AI agent.

## Description
Connect your **VectorShift** account to any AI agent and take full control of your AI automation and RAG (Retrieval-Augmented Generation) workflows through natural conversation.

### What you can do

- **AI Pipelines** — List, create, and run complex multi-step workflows. Manage execution with pause, resume, and terminate controls.
- **Knowledge Management** — Create vector-based knowledge bases, index documents (files/URLs), and perform semantic searches to ground your AI.
- **Chatbot Orchestration** — Deploy chatbots, upload context files, and run conversational instances directly.
- **Data Transformations** — Execute custom data transformations and logic as part of your automated processes.

### How it works

1. Subscribe to this server
2. Enter your VectorShift API Key
3. Start building and running AI automations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — trigger and test RAG pipelines or knowledge base indexing straight from your coding environment
- **Operations Teams** — automate repetitive data processing tasks using pre-built AI pipelines
- **Product Teams** — quickly query internal knowledge bases to retrieve technical or product documentation via AI


## Available Tools (29)
- **bulk_run_pipeline**: Execute multiple instances of a pipeline in parallel
- **create_chatbot**: Create a new chatbot
- **create_knowledge_base**: Create a new knowledge base
- **create_pipeline**: Create a new pipeline
- **create_transformation**: Create a new transformation (Python/JS)
- **delete_chatbot**: Delete a chatbot
- **delete_knowledge_base_documents**: Delete specific documents by ID from a knowledge base
- **delete_knowledge_base**: Delete a knowledge base
- **delete_pipeline**: Delete a pipeline by ID
- **delete_transformation**: Delete a transformation
- **get_chatbot**: Fetch a chatbot by id or name
- **get_knowledge_base**: Fetch a knowledge base by id or name
- **get_pipeline**: Fetch a pipeline by id or name
- **get_transformation**: Fetch a transformation by id or name
- **index_knowledge_base**: Add data (files, URLs, etc.) to a knowledge base
- **list_chatbots**: List all available chatbots
- **list_knowledge_base_documents**: Find documents within a knowledge base
- **list_knowledge_bases**: List all available knowledge bases
- **list_pipelines**: List all available pipelines
- **list_transformations**: List all available transformations
- **pause_pipeline**: Pause a currently running pipeline instance
- **query_knowledge_base**: Query a knowledge base with semantic search
- **resume_pipeline**: Resume one or more paused pipeline instances
- **run_chatbot**: Send a message to a chatbot and get a response
- **run_pipeline**: Execute a pipeline with specified inputs
- **run_transformation**: Execute a transformation with inputs
- **terminate_chatbot**: Terminate an active chatbot session
- **terminate_pipeline**: Stop a currently running pipeline instance
- **upload_chatbot_files**: Upload files to a chatbot session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VectorShift (AI Workflow & RAG Automation)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available VectorShift pipelines."

**🤖 AI Agent:**
> I've retrieved your pipelines. You have 3 active workflows: 'Customer Support Bot' (ID: pipe_1), 'Data Extractor' (ID: pipe_2), and 'Lead Scraper' (ID: pipe_3).

---

**👤 You:**
> "Search the 'Company Wiki' knowledge base (ID: kb_99) for 'remote work policy'."

**🤖 AI Agent:**
> Searching... I found relevant sections: 'Employees can work remotely up to 3 days a week' and 'Home office stipends are processed monthly'. Would you like more details?

---

**👤 You:**
> "Run the 'Data Extractor' pipeline (ID: pipe_2) with the input 'url: https://example.com'."

**🤖 AI Agent:**
> Pipeline 'Data Extractor' started. The execution is in progress. I will notify you once the data extraction from example.com is complete.


## ❓ FAQ

**Q: How do I search for specific information within my VectorShift knowledge base?**
Use the `query_knowledge_base` tool with your Knowledge Base ID and the search query. The agent will perform a semantic search and return the most relevant data chunks.

**Q: Can I trigger a specific AI workflow with custom parameters?**
Yes! Use the `run_pipeline` tool. Provide the Pipeline ID and a JSON object mapping your input names to their respective values to start the execution.

**Q: Is it possible to add new documents to a knowledge base through the agent?**
Absolutely. Use the `index_knowledge_base` tool to add data (such as URLs or file content) to an existing knowledge base for real-time RAG updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vectorshift-ai-workflow-rag-automation](https://vinkius.com/mcp/vectorshift-ai-workflow-rag-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VectorShift (AI Workflow & RAG Automation)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vectorshift-ai-workflow-rag-automation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VectorShift (AI Workflow & RAG Automation)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vectorshift-ai-workflow-rag-automation": {
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
