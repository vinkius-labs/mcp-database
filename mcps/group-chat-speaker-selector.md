# Group Chat Speaker Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/group-chat-speaker-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Deterministic speaker selection engine for multi-agent group chats.

## Description
This MCP server provides a deterministic selection engine for multi-agent orchestrations. It replaces non-deterministic agent rotation with predictable, rule-based scheduling logic. Use `select_next_speaker` to choose the next participant using strategies like round_robin, priority_based, relevance_based, or token_budget_aware. The engine enforces a fairness constraint to ensure no single agent dominates the conversation, and provides tools like `get_agent_eligibility` and `update_speaker_history` to manage the conversation state accurately.


## Available Tools (3)
- **get_agent_eligibility**: Checks if a specific agent is currently permitted to speak based on the conversation fairness rules
- **select_next_speaker**: Determines which agent should speak next based on a specific strategy and current conversation state
- **update_speaker_history**: Records a completed turn to update the historical participation data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Group Chat Speaker Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who should speak next in my group chat using round_robin?"

**🤖 AI Agent:**
> The next speaker will be Agent_B.

---

**👤 You:**
> "Which agent is most relevant to a message about 'Python programming'?"

**🤖 AI Agent:**
> The Python Expert agent is the most relevant choice.

---

**👤 You:**
> "Check if Agent_A is allowed to speak."

**🤖 AI Agent:**
> Agent_A is currently eligible to speak.


## ❓ FAQ

**Q: How does the fairness constraint work?**
The engine ensures no agent speaks more than the ceiling of the average turns per agent plus one, preventing any single agent from dominating the dialogue.

**Q: What selection strategies are available?**
Available strategies include round_robin for cyclic order, priority_based for importance ranking, relevance_based for keyword matching, and token_budget_aware for resource management.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/group-chat-speaker-selector](https://vinkius.com/mcp/group-chat-speaker-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Group Chat Speaker Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `group-chat-speaker-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Group Chat Speaker Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "group-chat-speaker-selector": {
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
