# Tencent Yuanqi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-yuanqi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate Tencent Yuanqi AI Agents — manage assistants, trigger conversations, and handle RAG documents directly from any AI agent.

## Description
Connect your AI agents to **Tencent Yuanqi** (腾讯元器), the official intelligent agent platform powered by the Hunyuan large model. This MCP provides 9 tools for comprehensive agent management and high-performance RAG operations.

### What you can do

- **Agent Interaction** — Chat with published agents using persistent sessions and context tracking
- **Document Lifecycle** — Upload, list, and delete documents for agent knowledge bases with real-time status tracking
- **Assistant Profiling** — Retrieve metadata and configuration for any assistant in your workspace
- **Usage Analysis** — Monitor token consumption and remaining quota programmatically

### How it works

1. Subscribe to this server
2. Log in to [**Tencent Yuanqi**](https://yuanqi.tencent.com/)
3. Navigate to **My Creations** and select a published agent
4. Under the **Publish** tab, enable **API** and generate an **API Key**
5. Insert your **API Key** and **Assistant ID** into the fields below

### Who is this for?

- **AI Developers** — automate document ingestion and test agent responses programmatically
- **Knowledge Managers** — maintain dynamic knowledge bases across multiple specialized agents
- **Product Teams** — integrate high-performance Chinese-native agents into custom applications


## Available Tools
- **chat**: Requires assistant_id and user_id.

Chat with a Tencent Yuanqi assistant
- **get_file_status**: Check file processing status
- **list_files**: List uploaded files
- **upload_file**: ) to the Yuanqi platform for use in assistant knowledge bases.

Upload a document for assistant context
- **delete_file**: Delete an uploaded file
- **get_assistant_info**: Get details about a specific assistant
- **get_file_info**: Get metadata for a specific file


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tencent Yuanqi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Chat with assistant 'assistant_123' and ask 'Explain the concept of deep learning'."

**🤖 AI Agent:**
> I'm connecting to the Yuanqi engine... Assistant 'assistant_123' responded: 'Deep learning is a subset of machine learning based on artificial neural networks...' Would you like me to save this response to your notes?

---

**👤 You:**
> "Upload the file 'specs.pdf' to my Yuanqi account."

**🤖 AI Agent:**
> Uploading 'specs.pdf'... Successfully uploaded! File ID: `file_xyz789`. The document is now being processed for the knowledge base. I'll let you know when it's ready.

---

**👤 You:**
> "List all assistants in my account."

**🤖 AI Agent:**
> Fetching your assistant list... I found 2 assistants: 1. ResearchBot (ID: asst_1), 2. CodeHelper (ID: asst_2). Which one would you like to interact with?


## ❓ FAQ

**Q: Can my AI automatically find the details of an assistant just by providing its ID?**
Yes! Use the `get_assistant_info` tool with the Assistant ID. Your agent will respond with complete metadata, configuration, and capabilities connected to that specific agent in seconds.

**Q: How do I check the remaining token quota for my account?**
Simply ask the agent to run the `get_usage` action. It will retrieve the current token consumption statistics and the remaining quota provided by the Yuanqi platform.

**Q: Can I upload multiple files for my assistant's knowledge base?**
Yes! Use the `upload_file` tool for each document you want to add. After uploading, use the `list_files` tool to verify they are processed and available for RAG operations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-yuanqi](https://vinkius.com/mcp/tencent-yuanqi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tencent Yuanqi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tencent-yuanqi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tencent Yuanqi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tencent-yuanqi": {
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
