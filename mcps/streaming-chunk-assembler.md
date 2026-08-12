# Streaming Chunk Assembler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/streaming-chunk-assembler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-processing](../categories/data-processing.md)

Reassembles fragmented LLM response chunks into complete, verified text and JSON.

## Description
This MCP server provides a deterministic state-machine engine to solve the problem of fragmented LLM streaming. It reassembles incoming response chunks into complete text, valid JSON objects, or structured tool calls by tracking sequence integrity and character-level syntax state. Use `append_chunk` to process incoming packets, `get_current_status` to monitor progress, and `finalize_stream` to perform a final structural validation of the assembled content.


## Available Tools (3)
- **append_chunk**: Processes a single incoming chunk and updates the internal assembly state
- **finalize_stream**: Forces the closure of a stream and performs a final validation of structural integrity
- **get_current_status**: Retrieves the current state of an ongoing assembly without adding new data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Streaming Chunk Assembler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Process this new chunk for stream 'abc-123': content='{"name": "test"', sequenceNumber=1, isFinal=false"

**🤖 AI Agent:**
> {"name": "test"

---

**👤 You:**
> "Complete the stream 'abc-123' and validate the JSON."

**🤖 AI Agent:**
> {"name": "test"}

---

**👤 You:**
> "What is the current status of stream 'xyz-789'?"

**🤖 AI Agent:**
> The stream 'xyz-789' has 5 chunks processed and is currently awaiting the final chunk.


## ❓ FAQ

**Q: How does the assembler handle missing chunks?**
The engine tracks sequence numbers for every stream. If a gap is detected, the missing sequence numbers are recorded and returned in the response.

**Q: Can I validate if a JSON object is complete?**
Yes. By using `finalize_stream`, the engine performs a character-level check for balanced braces and brackets to ensure the JSON is structurally sound.

**Q: How do I check the progress of a stream?**
You can use the `get_current_status` tool with the specific `streamId` to retrieve the current buffer and assembly state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/streaming-chunk-assembler](https://vinkius.com/mcp/streaming-chunk-assembler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Streaming Chunk Assembler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `streaming-chunk-assembler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Streaming Chunk Assembler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "streaming-chunk-assembler": {
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
