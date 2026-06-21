# Dot Object Transformer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dot-object-transformer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Flatten deeply nested JSON objects into dot-notation keys, or reconstruct nested objects from flat dictionaries.

## Description
When an AI Agent needs to export nested API data to a CSV spreadsheet or rebuild a nested payload from flat form fields, it shouldn't guess the dot-notation mapping. This MCP handles it deterministically.

### The Superpowers

- **Bidirectional:** Flatten nested JSON to `{"user.name": "John"}` or unflatten it back.
- **Lossless:** Preserves arrays, nulls, and complex nested structures perfectly.


## Available Tools (1)
- **transform_dot_object**: g. {"user.name": "John", "user.address.city": "NYC"}) for spreadsheet exports, or unflatten a flat dictionary back into a nested JSON structure for API payloads.

Flattens deeply nested JSON objects into single-level dot-notation keys, or reconstructs nested objects from flat dictionaries. Essential for CSV exports and API integrations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dot Object Transformer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Flatten this nested user profile JSON for CSV export."

**🤖 AI Agent:**
> Dot Object Result: 8 keys flattened.


## ❓ FAQ

**Q: Does it preserve arrays?**
Yes, arrays are flattened with numeric indices (e.g. "items.0.name") and restored perfectly on unflatten.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dot-object-transformer](https://vinkius.com/mcp/dot-object-transformer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dot Object Transformer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dot-object-transformer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dot Object Transformer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dot-object-transformer": {
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
