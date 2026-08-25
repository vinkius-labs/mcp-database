# Token Counter and Budget Enforcer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/token-counter-and-budget-enforcer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Estimates token usage and enforces strict cumulative budget limits for AI agents.

## Description
This MCP server provides precise token estimation and budget management for AI agents. It uses deterministic BPE approximation to calculate token counts for text and code, ensuring predictable resource tracking. The server tracks cumulative usage per agent and per conversation, allowing for strict enforcement of token limits. Use `estimate_tokens` to predict costs, `track_and_enforce_usage` to record consumption and check against limits, or `get_usage_summary` to view current totals. It is ideal for managing LLM costs and preventing budget overruns in multi-agent systems.


## Available Tools (3)
- **estimate_tokens**: Calculates the estimated token count for a provided text string
- **track_and_enforce_usage**: Updates the cumulative usage for an agent and a conversation, then checks against set limits
- **get_usage_summary**: Retrieves current cumulative totals without consuming new tokens


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Token Counter and Budget Enforcer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many tokens will this sentence use: 'Hello, how are you today?'"

**🤖 AI Agent:**
> The estimated token count for that sentence is 6 tokens.

---

**👤 You:**
> "Estimate the tokens for this code: 'print("hello")'"

**🤖 AI Agent:**
> The estimated token count for that code snippet is 4 tokens.

---

**👤 You:**
> "What is the current usage for agent_123?"

**🤖 AI Agent:**
> Agent_123 has consumed a total of 1,250 tokens.


## ❓ FAQ

**Q: How are tokens estimated?**
Tokens are estimated using a deterministic character-to-token ratio: approximately 4 characters per token for English text and 3.5 characters per token for code blocks.

**Q: Can I set different limits for agents and conversations?**
Yes. You can use `track_and_enforce_usage` to apply specific limits for both the unique agent identifier and the specific conversation identifier.

**Q: How do I check my current usage?**
You can use the `get_usage_summary` tool to retrieve the cumulative token totals for a specific agent or conversation without consuming any new tokens.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/token-counter-and-budget-enforcer](https://vinkius.com/ai-agent-connect/token-counter-and-budget-enforcer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Token Counter and Budget Enforcer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `token-counter-and-budget-enforcer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Token Counter and Budget Enforcer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "token-counter-and-budget-enforcer": {
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
