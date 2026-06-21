# Writer (AI Enterprise LLM) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/writer-ai-enterprise-llm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Writer's enterprise-grade LLMs and Knowledge Graph capabilities to generate content, manage files, and query RAG-based data.

## Description
Connect to **Writer**, the full-stack generative AI platform for the enterprise. This MCP server allows your AI agent to leverage the Palmyra family of models, manage complex Knowledge Graphs for RAG, and handle enterprise document processing.

### What you can do

- **Enterprise LLMs** — Generate chat and text completions using high-performance models like Palmyra-X5.
- **Knowledge Graphs** — Create and manage Knowledge Graphs to power Retrieval-Augmented Generation (RAG) workflows.
- **File Management** — Upload, list, and delete documents used for model training or graph context.
- **Model Discovery** — Dynamically list available models to ensure you are using the latest enterprise capabilities.

### How it works

1. Subscribe to this server
2. Enter your Writer API Key
3. Start generating enterprise-ready content and querying your internal knowledge bases.

### Who is this for?

- **Enterprise Developers** — Build RAG-powered applications with secure, compliant LLMs.
- **Content Teams** — Automate high-quality content generation using custom-trained enterprise models.
- **Data Engineers** — Manage document pipelines and knowledge graphs directly through AI conversation.


## Available Tools
- **add_file_to_graph**: Add an uploaded file to a Knowledge Graph
- **analyze_vision**: Analyze images or documents using a prompt
- **ask_question**: Ask a question against one or more Knowledge Graphs (RAG)
- **chat_completion**: Generate a chat completion using Writer models
- **create_graph**: Create a new Knowledge Graph
- **delete_file**: Permanently delete a file
- **download_file**: Download the binary content of a file
- **generate_application_content_async**: Asynchronous generation using a no-code application (returns job_id)
- **generate_application_content**: Synchronous generation using a no-code application
- **get_application_job**: Retrieve job status and result for an application job
- **get_application**: Get configuration and inputs for a specific application
- **get_file**: Get metadata for a specific file
- **list_application_jobs**: List jobs for a specific application
- **list_applications**: List deployed no-code agents (applications)
- **list_files**: Retrieve a paginated list of uploaded files
- **list_graphs**: List all Knowledge Graphs
- **list_models**: Retrieve available Writer models
- **parse_pdf**: Convert PDF to text or markdown (Deprecated)
- **remove_file_from_graph**: Remove a file from a Knowledge Graph
- **retry_application_job**: Retry a failed application job
- **text_completion**: Generate text completions for a single prompt
- **translate_text**: Translate text between supported languages
- **upload_file**: Upload a file for Knowledge Graphs or Vision tasks
- **web_search**: Search the web for a query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Writer (AI Enterprise LLM)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available Writer models."

**🤖 AI Agent:**
> I've retrieved the models. You have access to palmyra-x5, palmyra-x5-32k, and palmyra-med. Which one would you like to use for your task?

---

**👤 You:**
> "Create a new Knowledge Graph named 'Q4 Strategy'."

**🤖 AI Agent:**
> I have successfully created the 'Q4 Strategy' Knowledge Graph. You can now use `add_file_to_graph` to include documents for RAG analysis.

---

**👤 You:**
> "Upload 'report.pdf' and list all my files."

**🤖 AI Agent:**
> File 'report.pdf' has been uploaded successfully. Your current file list includes: 'report.pdf' (ID: file-123) and 'budget.xlsx' (ID: file-456).


## ❓ FAQ

**Q: How do I see which Palmyra models are available in my account?**
Use the `list_models` tool. It will return a list of all active models in your Writer account, such as palmyra-x5 or palmyra-med.

**Q: Can I use my own documents for AI responses?**
Yes. First, use `upload_file` to add your documents, then `create_graph` and `add_file_to_graph` to build a Knowledge Graph for RAG-based querying.

**Q: Does this support conversational history?**
Yes, the `chat_completion` tool accepts a `messages` array, allowing you to maintain full context for multi-turn dialogues with the model.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/writer-ai-enterprise-llm](https://vinkius.com/mcp/writer-ai-enterprise-llm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Writer (AI Enterprise LLM)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `writer-ai-enterprise-llm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Writer (AI Enterprise LLM)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "writer-ai-enterprise-llm": {
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
