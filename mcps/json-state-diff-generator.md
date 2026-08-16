# json-state-diff-generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/json-state-diff-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

High-precision JSON state comparison for debugging agentic workflows.

## Description
This MCP server provides high-precision tools for computing structural and value-based differences between two JSON states. It is specifically optimized for debugging agentic workflows like LangGraph and CrewAI by identifying added, removed, and modified keys through deterministic recursive traversal. Use `compare_json_states` to find deep differences, `get_diff_summary` for statistical overviews, and `flatten_diff_path` to convert nested changes into human-readable dot-notation paths.


## Available Tools (3)
- **compare_json_states**: Performs a deep, recursive comparison between two JSON objects to identify all structural and value changes
- **flatten_diff_path**: Converts complex, nested diff paths into human-readable dot-notation strings
- **get_diff_summary**: Provides a high-level statistical overview of the differences found between two states


## 💬 Prompt Examples

Here are some examples of how you can interact with the **json-state-diff-generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two JSON states: {"a": 1, "b": 2} and {"a": 1, "b": 3, "c": 4}"

**🤖 AI Agent:**
> {"diff": {"b": {"old_value": 2, "new_value": 3}, "c": {"added": true}}, "changesCount": 2, "isUnchanged": false}

---

**👤 You:**
> "Get a summary of the changes for this diff result: {"added": 1, "removed": 0, "modified": 1}"

**🤖 AI Agent:**
> {"totalChanges": 2, "changeTypeCounts": {"added": 1, "removed": 0, "modified": 1}}

---

**👤 You:**
> "Convert this diff into a list of paths: {"user": {"profile": {"id": "changed"}}}"

**🤖 AI Agent:**
> {"paths": ["user.profile.id"]}


## ❓ FAQ

**Q: How does the tool handle array comparisons?**
The tool performs a strict positional comparison. Elements are evaluated based on their exact index; for example, the element at index 0 in the previous state is compared only to the element at index 0 in the current state.

**Q: What is the difference between added and modified keys?**
Added keys are elements present in the current state that were entirely absent in the previous state. Modified keys are elements that exist in both states but contain different values.

**Q: Can I use this to debug LangGraph states?**
Yes, the `compare_json_states` tool is specifically designed to identify how a data structure has evolved, making it ideal for tracking state changes in LangGraph and CrewAI workflows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/json-state-diff-generator](https://vinkius.com/ai-agent-connect/json-state-diff-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **json-state-diff-generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `json-state-diff-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **json-state-diff-generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "json-state-diff-generator": {
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
