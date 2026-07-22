# SSE Event Reassembler & Gap Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sse-event-reassembler-gap-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Detect packet loss and reconstruct fragmented SSE streams.

## Description
This MCP server provides specialized tools to ensure the integrity of Server-Sent Events (SSE) streams. It allows AI agents to identify gaps in sequential data, specifically detecting when packets are lost during transmission. Use `check_stream_continuity` to verify if a sequence is unbroken, `reconstruct_message_payload` to merge fragmented text into a single coherent message, and `enumerate_missing_identifiers` to pinpoint exactly which event IDs were missed. This is essential for preventing silent data drops in streaming LLM responses.


## Available Tools (3)
- **check_stream_continuity**: Check if a sequence of SSE events arrived without any missing packets
- **enumerate_missing_identifiers**: Identify exactly which specific event IDs were lost during transmission
- **reconstruct_message_payload**: Extract and merge all text fragments into a single unified message string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SSE Event Reassembler & Gap Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this stream of events is complete: [{'event_id': 1, 'data': 'Hello', 'timestamp': '2024-01-01T10:00:00Z'}, {'event_id': 3, 'data': 'World', 'timestamp': '2024-01-01T10:00:02Z'}]"

**🤖 AI Agent:**
> The stream is incomplete. A gap was detected because event ID 2 is missing.

---

**👤 You:**
> "Reconstruct the message from these fragments: [{'event_id': 10, 'data': 'Part A ', 'timestamp': '...'}, {'event_id': 11, 'data': 'Part B', 'timestamp': '...'}]"

**🤖 AI Agent:**
> The reassembled payload is: Part A Part B

---

**👤 You:**
> "Which IDs are missing from this list: [{'event_id': 5, 'data': 'x', 'timestamp': '...'}, {'event_id': 8, 'data': 'y', 'timestamp': '...'}]"

**🤖 AI Agent:**
> The missing IDs are: [6, 7]


## ❓ FAQ

**Q: How does the server detect gaps in a stream?**
The server sorts all received events by their ID and checks if any integer in the sequence is missing. If the difference between two consecutive IDs is greater than one, a gap is flagged.

**Q: Can I use this to fix broken LLM responses?**
Yes. By using `reconstruct_message_payload`, you can take fragmented chunks and merge them into a single, complete string, ensuring no part of the response is lost.

**Q: What format should the input data be in?**
The tools expect a JSON array of objects, where each object contains an `event_id` (integer), `data` (string), and `timestamp` (string).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sse-event-reassembler-gap-detector](https://vinkius.com/mcp/sse-event-reassembler-gap-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SSE Event Reassembler & Gap Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sse-event-reassembler-gap-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SSE Event Reassembler & Gap Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sse-event-reassembler-gap-detector": {
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
