# Agent Capability Matcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-capability-matcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Aligns AI agents to tasks using weighted capability scoring.

## Description
This MCP server provides a deterministic engine to resolve delegation ambiguity in multi-agent frameworks. It calculates a capability score by combining skill keyword overlap and tool coverage. Use `query_agent_matches` to rank all available agents, `verify_capability_gap` to audit specific missing requirements, or `calculate_match_metrics` to retrieve raw mathematical components of a match.


## Available Tools (3)
- **calculate_match_metrics**: Retrieve the raw mathematical components of a match without the final weighted aggregation
- **query_agent_matches**: Rank all available agents against a specific task to find the best candidate
- **verify_capability_gap**: Perform a deep-dive check on a single agent to see exactly what is missing for a specific task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Capability Matcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which agent is best suited for a task requiring 'data analysis' and 'python' tools?"

**🤖 AI Agent:**
> The best match is agent_001 with a capability score of 0.85.

---

**👤 You:**
> "Check the capability gaps for agent_alpha against a task requiring 'web searching'."

**🤖 AI Agent:**
> Agent_alpha is missing the 'web searching' skill.

---

**👤 You:**
> "Get the raw metrics for agent_beta against the current task."

**🤖 AI Agent:**
> The skill overlap ratio is 0.5 and the tool coverage ratio is 1.0.


## ❓ FAQ

**Q: How is the capability score calculated?**
The score is a weighted combination: 60% for skill keyword overlap (Jaccard similarity) and 40% for tool coverage ratio.

**Q: Can I see exactly what an agent is missing?**
Yes, by using the `verify_capability_gap` tool, you can retrieve a list of specific missing skills and tools for a given agent profile.

**Q: What happens if no agents match the task?**
The system handles empty profiles or requirements gracefully, returning empty results or zero scores without errors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-capability-matcher](https://vinkius.com/ai-agent-connect/agent-capability-matcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Capability Matcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-capability-matcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Capability Matcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-capability-matcher": {
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
