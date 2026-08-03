# Langfuse Trace URL Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/langfuse-trace-url-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Extract trace IDs and construct observability URLs from Langfuse payloads.

## Description
The Langfuse Trace URL Extractor automates the process of finding execution traces within large JSON logs. By using `extract_trace_identifiers`, you can pull the exact trace and project IDs from a raw payload. Then, use `construct_langfuse_url` to generate a direct link to the Langfuse Cloud dashboard. You can also use `validate_payload_schema` to ensure your data is ready for processing.


## Available Tools (3)
- **extract_trace_identifiers**: Extracts trace and project IDs from a Langfuse payload JSON
- **validate_payload_schema**: Validates if a JSON payload contains required Langfuse fields
- **construct_langfuse_url**: Constructs a direct Langfuse trace URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Langfuse Trace URL Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract IDs from this payload: {"id": "trace-123", "project_id": "proj-456"}"

**🤖 AI Agent:**
> {"traceId": "trace-123", "projectId": "proj-456"}

---

**👤 You:**
> "Construct a URL for trace 'abc' and project 'xyz'."

**🤖 AI Agent:**
> https://cloud.langfuse.com/project/xyz/traces/abc

---

**👤 You:**
> "Is this payload valid: {"id": "trace-789"}"

**🤖 AI Agent:**
> {"isValidPayload": false, "missingFields": ["project_id"]}


## ❓ FAQ

**Q: What does `extract_trace_identifiers` do?**
It parses a Langfuse payload JSON to extract the root `id` and `project_id` fields.

**Q: How do I generate a clickable link?**
Use the `construct_langfuse_url` tool with the extracted trace ID and project ID.

**Q: Can I verify if a payload is valid before processing?**
Yes, the `validate_payload_schema` tool checks for the presence of required keys.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/langfuse-trace-url-extractor](https://vinkius.com/mcp/langfuse-trace-url-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Langfuse Trace URL Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `langfuse-trace-url-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Langfuse Trace URL Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "langfuse-trace-url-extractor": {
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
