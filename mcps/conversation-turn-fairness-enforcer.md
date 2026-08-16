# Conversation Turn Fairness Enforcer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/conversation-turn-fairness-enforcer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [monitoring](../categories/monitoring.md)

Prevents agent domination in multi-agent conversations by monitoring turn frequency.

## Description
This MCP server provides monitoring and enforcement tools to ensure equitable speaking time in multi-agent environments. It prevents individual agents from dominating discussions by tracking turn counts and identifying statistical deviations. Use `analyze_turn_distribution` to identify dominating agents, `get_agent_participation_metrics` for high-level activity summaries, and `validate_turn_eligibility` to check if a specific agent is permitted to speak based on current fairness constraints.


## Available Tools (3)
- **analyze_turn_distribution**: 
- **get_agent_participation_metrics**: 
- **validate_turn_eligibility**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conversation Turn Fairness Enforcer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the current conversation is fair with a tolerance of 0.2."

**🤖 AI Agent:**
> The conversation is fair. No agents are currently exceeding the threshold.

---

**👤 You:**
> "Is agent 'researcher_01' allowed to take the next turn?"

**🤖 AI Agent:**
> No, 'researcher_01' is not eligible because they have already exceeded the allowed turn limit.

---

**👤 You:**
> "Give me a summary of the participation metrics."

**🤖 AI Agent:**
> The conversation has had 12 total turns across 3 agents, with an average of 4 turns per agent.


## ❓ FAQ

**Q: How does the enforcer detect domination?**
It calculates the expected fair share by dividing total turns by the number of agents. An agent is flagged as dominating if their turn count exceeds this share plus a configurable tolerance factor.

**Q: Can I adjust the sensitivity of the fairness check?**
Yes, you can provide a `toleranceFactor` to the tools to define the allowed deviation from the expected fair share.

**Q: What tools are available in this MCP?**
The server provides `analyze_turn_distribution` for fairness reports, `get_agent_participation_metrics` for activity summaries, and `validate_turn_eligibility` for turn permission checks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/conversation-turn-fairness-enforcer](https://vinkius.com/ai-agent-connect/conversation-turn-fairness-enforcer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Conversation Turn Fairness Enforcer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `conversation-turn-fairness-enforcer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Conversation Turn Fairness Enforcer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "conversation-turn-fairness-enforcer": {
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
