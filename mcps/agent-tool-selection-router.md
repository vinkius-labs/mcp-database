# Agent Tool Selection Router MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-tool-selection-router)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

A deterministic engine for selecting and sequencing optimal tools for AI agents.

## Description
The Agent Tool Selection Router is a decision-making engine that optimizes how AI agents select and sequence tools. Instead of probabilistic guessing, it uses deterministic scoring based on real-time performance metrics. By using `calculate_tool_scores`, the engine evaluates intent match, success rates, and latency to find the best tool. It also uses `plan_tool_execution_path` to determine fallback chains and tool composition, and `validate_tool_constraints` to ensure no operational rules like mutual exclusivity are violated. This ensures reliable and efficient tool execution for any AI client, including Cursor, VS Code, Claude Desktop, and Windsurf.


## Available Tools (3)
- **calculate_tool_scores**: Calculate deterministic scores for available tools based on intent and environment
- **plan_tool_execution_path**: Determine the sequence of actions, including potential fallbacks and tool chaining
- **validate_tool_constraints**: Ensure proposed tool selection does not violate operational constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Tool Selection Router** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the best tool to use for a web search task with high confidence."

**🤖 AI Agent:**
> The selected tool is `search_web` with a score of 0.85.

---

**👤 You:**
> "Plan an execution path for the primary tool `data_fetcher`."

**🤖 AI Agent:**
> The execution path includes `data_fetcher` followed by `data_processor` with an estimated latency of 450ms.

---

**👤 You:**
> "Check if calling `read_file` and `write_file` simultaneously is allowed."

**🤖 AI Agent:**
> The tool selection is invalid due to a mutual exclusivity violation.


## ❓ FAQ

**Q: How does the tool selection scoring work?**
The engine calculates a score by multiplying intent confidence, historical success rate, the inverse of normalized latency, and the available rate limit headroom.

**Q: Can the router handle tool chaining?**
Yes, the `plan_tool_execution_path` tool identifies tool composition opportunities where the output of one tool can serve as the input for another.

**Q: How are rate limits managed?**
The router calculates rate limit headroom. If a tool's capacity is exhausted, its score drops to zero, and the engine flags a rate limit error.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-tool-selection-router](https://vinkius.com/ai-agent-connect/agent-tool-selection-router)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Tool Selection Router** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-tool-selection-router` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Tool Selection Router** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-tool-selection-router": {
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
