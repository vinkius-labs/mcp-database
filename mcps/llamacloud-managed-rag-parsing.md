# LlamaCloud (Managed RAG & Parsing) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/llamacloud-managed-rag-parsing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage RAG pipelines and document parsing via LlamaCloud — orchestrate LlamaParse jobs and audit data ingestion.

## Description
Connect your **LlamaCloud** account to any AI agent and take full control of your enterprise RAG infrastructure and AI-powered document parsing through natural conversation.

### What you can do

- **Pipeline Orchestration** — List all deployed data pipelines and retrieve detailed configurations including connected sources and index settings directly from your agent
- **AI Document Parsing** — Dispatch complex files (PDFs, docs) to LlamaParse to convert intricate layouts, tables, and handwriting into structured Markdown context
- **Job Monitoring** — Track the status of ongoing parsing jobs and retrieve extraction results once processing is complete to power your AI workflows
- **Project Management** — Navigate high-level LlamaCloud projects managing collections of pipelines and queryable indices securely
- **Unstructured Data Ingestion** — Monitor the flow of raw data into your managed indices and verify processing states for high-quality LLM grounding
- **Diagnostic Audit** — Fetch final parsed outputs and job traces to ensure data integrity and layout accuracy across your RAG pipeline

### How it works

1. Subscribe to this server
2. Enter your LlamaCloud API Key
3. Start managing your RAG infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **RAG Developers** — automate the ingestion of complex enterprise documents and monitor pipeline health through natural conversation
- **AI Engineers** — verify document parsing quality and orchestrate large-scale data extraction jobs without manual Python scripts
- **Data Scientists** — audit managed indices and track parsing statuses to ensure high-quality fact-grounding for AI agents


## Available Tools (6)
- **create_parsing_upload**: Dispatch a file explicitly to LlamaParse
- **get_parsing_result**: Retrieve the final markdown/rich-text extraction from LlamaParse
- **list_pipelines**: List LlamaCloud deployed data pipelines
- **get_pipeline**: Get configuration details for a specific pipeline
- **list_projects**: List active LlamaCloud projects
- **list_parsing_jobs**: List LlamaParse active parsing jobs tracking document ingestion


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LlamaCloud (Managed RAG & Parsing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active data pipelines in my LlamaCloud account"

**🤖 AI Agent:**
> I've found 3 active pipelines: 'Financial-Reports-Index' (ID: pipe-123), 'Technical-Docs-RAG' (ID: pipe-456), and 'Customer-Support-KB' (ID: pipe-789). Which one would you like to check the source configuration for?

---

**👤 You:**
> "Parse this PDF file using LlamaParse: 'annual_report_2024.pdf'"

**🤖 AI Agent:**
> File submitted to LlamaParse. Job ID: 'job-98765'. I'm monitoring the extraction process. LlamaCloud is currently processing complex tables and charts within the report. I'll provide the Markdown result as soon as it's ready.

---

**👤 You:**
> "Show me the configuration for the 'Technical-Docs-RAG' pipeline"

**🤖 AI Agent:**
> Pipeline 'Technical-Docs-RAG' (ID: pipe-456) is configured with 2 sources: a S3 bucket ('s3://docs-bucket') and a Google Drive folder. It uses OpenAI 'text-embedding-3-small' for indexing and is mapped to your 'production-index' in LlamaCloud.


## ❓ FAQ

**Q: Can LlamaParse handle complex tables and layouts in my PDFs?**
Absolutely. LlamaParse uses AI-driven parsing to turn complex PDF layouts, nested tables, and even handwriting into structured Markdown. Use the `create_parsing_upload` tool to start the process and retrieve high-quality context for your agent.

**Q: How do I check if my RAG data pipeline is finished processing?**
Use the `get_parsing_result` tool with your specific Job ID. Your agent will poll the LlamaCloud API and report the current status. Once finished, it will retrieve the final parsed content ready for grounding.

**Q: Can I see all data sources connected to a specific pipeline?**
Yes. The `get_pipeline` tool extracts the full configuration for any pipeline ID, identifying all connected data sources and configured index settings, ensuring you have a complete view of your ingestion flow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/llamacloud-managed-rag-parsing](https://vinkius.com/mcp/llamacloud-managed-rag-parsing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LlamaCloud (Managed RAG & Parsing)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `llamacloud-managed-rag-parsing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LlamaCloud (Managed RAG & Parsing)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "llamacloud-managed-rag-parsing": {
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
