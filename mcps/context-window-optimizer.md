# Context Window Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/context-window-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Optimally selects and orders context items to maximize relevance within token limits.

## Description
The Context Window Optimizer solves the problem of context overflow and relevance decay in LLM applications. It uses a deterministic greedy selection algorithm to pick the most important information based on relevance scores and recency. By using tools like `select_optimal_context`, `evaluate_context_efficiency`, and `filter_by_recency`, AI agents can ensure they always operate within their token budget while maintaining the highest possible information density. This is essential for complex workflows in LangChain and CrewAI where managing the attention mechanism is critical.


## Available Tools (3)
- **evaluate_context_efficiency**: Analyzes a selection of context to determine if it was optimized effectively
- **filter_by_recency**: Removes outdated information from the candidate pool based on a specific time horizon
- **select_optimal_context**: Determines which pieces of information should be included in the LLM prompt to maximize relevance without exceeding the token limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Context Window Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Select the best context from these items with a 500 token limit."

**🤖 AI Agent:**
> The selected items are: [Item A (200 tokens, score 0.9), Item B (250 tokens, score 0.8)]. Total tokens used: 450.

---

**👤 You:**
> "Filter out all context items older than 3600 seconds."

**🤖 AI Agent:**
> 3 items were removed, and 5 items remain within the time horizon.

---

**👤 You:**
> "What is the efficiency of this context selection?"

**🤖 AI Agent:**
> The utilization ratio is 0.92 and the density score is 0.85.


## ❓ FAQ

**Q: How does the selection process work?**
The process uses `select_optimal_context` to sort items by relevance score and recency, then greedily adds them until the token limit is reached.

**Q: Can I reserve specific messages?**
Yes, you can use the reservation rules in `select_optimal_context` to ensure the system prompt and the last user message are always included.

**Q: How do I measure if my context is efficient?**
You can use the `evaluate_context_efficiency` tool to get a report on utilization ratio, density score, and coverage gap.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/context-window-optimizer](https://vinkius.com/mcp/context-window-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Context Window Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `context-window-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Context Window Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "context-window-optimizer": {
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
