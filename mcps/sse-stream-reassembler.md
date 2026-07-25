# SSE Stream Reassembler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sse-stream-reassembler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-processing](../categories/data-processing.md)

Reassembles fragmented Server-Sent Events (SSE) streams into a single coherent payload.

## Description
The SSE Stream Reassembler is designed to solve the problem of fragmented LLM responses. It takes raw, chunked Server-Sent Events (SSE) streams and reconstructs them into a single, continuous message. By using tools like `reassemble_stream`, `validate_json`, and `extract_field`, you can reliably parse incoming data chunks, verify their JSON integrity, and extract specific information without losing fragments during transport.


## Available Tools (3)
- **extract_field**: Extracts a specific field from a JSON string
- **reassemble_stream**: Reassembles fragmented SSE stream chunks into a single string
- **validate_json**: Validates if a given string is valid JSON


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SSE Stream Reassembler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have these SSE chunks: 'data: {"id": 1}\n\ndata: {"id": 2}'. Reassemble them."

**🤖 AI Agent:**
> {"id": 1}{"id": 2}

---

**👤 You:**
> "Check if this chunk is valid JSON: 'data: {"status": "ok"}'"

**🤖 AI Agent:**
> The chunk is a valid JSON structure.

---

**👤 You:**
> "Extract the 'user' field from this chunk: 'data: {"user": "alice"}'"

**🤖 AI Agent:**
> alice


## ❓ FAQ

**Q: What is the primary use case for this MCP server?**
It is ideal for handling streaming LLM responses where chunks are delivered via SSE and need to be reassembled into a complete payload using `reassemble_stream`.

**Q: How does the tool handle heartbeat signals?**
The `reassemble_stream` tool automatically identifies and ignores keep-alive or heartbeat pings, ensuring only actual data segments are included in the final payload.

**Q: Can I validate individual chunks before reassembling them?**
Yes, you can use the `validate_json` tool to check if a specific chunk contains valid JSON structure before proceeding with full stream reconstruction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sse-stream-reassembler](https://vinkius.com/mcp/sse-stream-reassembler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SSE Stream Reassembler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sse-stream-reassembler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SSE Stream Reassembler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sse-stream-reassembler": {
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
