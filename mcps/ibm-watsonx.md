# IBM watsonx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibm-watsonx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect IBM watsonx to any AI agent via MCP.



## Available Tools (10)
- **create_prompt**: Create a new prompt in watsonx
- **generate_chat**: Use this for multi-turn conversational AI applications.

Generate chat completions using a watsonx chat model
- **generate_embeddings**: Useful for similarity search, clustering, and semantic analysis.

Generate vector embeddings for input texts
- **generate_text**: Use this for single-turn text generation tasks like content creation, summarization, or analysis.

Generate text using a watsonx foundation model
- **get_model_details**: Get detailed specifications for a specific foundation model
- **get_tuning_status**: Get the status of a prompt tuning job
- **list_models**: ai, including model IDs, families, capabilities, and lifecycle states.

List available foundation models in watsonx
- **list_projects**: List watsonx projects in your account
- **list_prompts**: List saved prompts in the watsonx project
- **start_model_tuning**: Requires a URL pointing to the training data in cloud storage.

Start a prompt tuning job for a foundation model






## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibm-watsonx](https://vinkius.com/mcp/ibm-watsonx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IBM watsonx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ibm-watsonx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IBM watsonx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ibm-watsonx": {
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
