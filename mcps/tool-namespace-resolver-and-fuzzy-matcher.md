# Tool Namespace Resolver and Fuzzy Matcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tool-namespace-resolver-and-fuzzy-matcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Resolves tool name hallucinations and misspellings using hierarchical matching logic.

## Description
This MCP server provides advanced tool resolution capabilities to prevent LLM hallucinations. It uses a strict hierarchy of matching: Exact Match, Case-Insensitive Match, Namespace Match, and finally Fuzzy Matching via Levenshtein distance. It is designed to fix 'tool not found' errors in frameworks like LangChain and CrewAI by mapping misspelled or partial names to valid identifiers. Use `resolve_tool_name` for single queries, `get_matching_tools_bulk` for batch processing, or `validate_tool_namespace` to verify functional groups.


## Available Tools (3)
- **get_matching_tools_bulk**: Processes a batch of requested tool names to identify multiple valid targets simultaneously
- **resolve_tool_name**: Resolves a single potentially misspelled or partial tool name into a valid identifier from a known list
- **validate_tool_namespace**: Determines if a requested string belongs to a specific functional group or namespace within the toolset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tool Namespace Resolver and Fuzzy Matcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Resolve the tool name 'pythn' from the list ['code_execution_python', 'search_web']"

**🤖 AI Agent:**
> The tool name 'pythn' has been resolved to 'code_execution_python' with a fuzzy match.

---

**👤 You:**
> "Check if 'search' belongs to the 'web_' namespace in ['web_search', 'web_map', 'file_read']"

**🤖 AI Agent:**
> Yes, 'search' matches the 'web_' namespace, which contains 2 tools.

---

**👤 You:**
> "Find all matches for ['search_web', 'pythn'] in ['search_web', 'code_execution_python']"

**🤖 AI Agent:**
> Matches found: 'search_web' (exact) and 'code_execution_python' (fuzzy).


## ❓ FAQ

**Q: How does the resolution hierarchy work?**
The engine follows a strict priority: it first looks for an exact match, then a case-insensitive match, then a namespace match, and finally a fuzzy match using Levenshtein distance. Once a higher-priority match is found, the search stops.

**Q: What is the purpose of `resolve_tool_name`?**
The `resolve_tool_name` tool is used to take a single potentially misspelled or partial tool name and map it to a valid identifier from a provided list of available tools.

**Q: Can I process multiple tool names at once?**
Yes, you can use `get_matching_tools_bulk` to process a list of requested tool names simultaneously against a known registry.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tool-namespace-resolver-and-fuzzy-matcher](https://vinkius.com/mcp/tool-namespace-resolver-and-fuzzy-matcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tool Namespace Resolver and Fuzzy Matcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tool-namespace-resolver-and-fuzzy-matcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tool Namespace Resolver and Fuzzy Matcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tool-namespace-resolver-and-fuzzy-matcher": {
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
