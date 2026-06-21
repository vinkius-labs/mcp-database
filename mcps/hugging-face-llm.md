# Hugging Face LLM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hugging-face-llm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Connect Hugging Face LLM to any AI agent via MCP.



## Available Tools (8)
- **classify_text**: No training required.

Classify text into custom categories using Zero-Shot Classification
- **text_generation**: Useful for creative writing, code completion, or chatting with an LLM.

Generate text completions using open-source LLMs (Mistral, Zephyr, etc)
- **fill_mask**: Fill in the blanks in a text using a masked language model
- **extract_entities**: Extract named entities (People, Organizations, Locations) from text
- **answer_question**: Provide a context (text) and a question, and it extracts the answer.

Answer a question based on a given context
- **sentiment_analysis**: Analyze the sentiment of a text (Positive/Negative)
- **summarize_text**: Good for articles, reports, or long messages.

Summarize a long text into a concise version
- **translate_text**: The specific languages depend on the chosen model.

Translate text from one language to another






## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hugging-face-llm](https://vinkius.com/mcp/hugging-face-llm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hugging Face LLM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hugging-face-llm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hugging Face LLM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hugging-face-llm": {
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
