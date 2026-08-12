# Agent Role Conflict Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agent-role-conflict-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Detects overlapping responsibilities and role conflicts in multi-agent teams.

## Description
This MCP server identifies friction within multi-agent orchestration systems like CrewAI. It detects redundant responsibilities by calculating overlap scores for agent goals, toolsets, and backstories. Use `analyze_agent_team` to scan an entire group, `check_agent_pair_conflict` to compare two specific agents, or `get_tool_redundancy_map` to find which tools are causing the most overlap. It helps prevent wasted tokens and conflicting outputs by suggesting whether to merge or differentiate agent roles.


## Available Tools (3)
- **analyze_agent_team**: Performs a comprehensive conflict analysis across an entire group of agents
- **check_agent_pair_conflict**: Investigates the relationship between exactly two agents to determine if they are redundant
- **get_tool_redundancy_map**: Identifies which specific tools are causing the most overlap within a team


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Role Conflict Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this team for conflicts: [{'agentId': 'researcher', 'role': 'Researcher', 'goal': 'Find facts', 'backstory': 'Expert in data', 'allowedTools': ['search']}, {'agentId': 'analyst', 'role': 'Analyst', 'goal': 'Find facts', 'backstory': 'Expert in data', 'allowedTools': ['search']}]"

**🤖 AI Agent:**
> {"hasConflicts": true, "conflictPairs": [{"agentIdA": "researcher", "agentIdB": "analyst", "goalOverlap": 1.0, "toolOverlap": 1.0, "backstoryOverlap": 1.0}], "resolutionSuggestions": ["Merge these agents"]}

---

**👤 You:**
> "Check if these two agents are redundant: Agent A (Goal: 'Write code', Tools: ['python']) and Agent B (Goal: 'Write code', Tools: ['python'])"

**🤖 AI Agent:**
> {"isConflicting": true, "scores": {"goalOverlap": 1.0, "toolOverlap": 1.0, "backstoryOverlap": 0.0}, "suggestion": "Merge these agents"}

---

**👤 You:**
> "Which tools are causing overlap in my agent team?"

**🤖 AI Agent:**
> {"redundantTools": [{"toolName": "web_search", "agentCount": 3, "agentIds": ["agent_1", "agent_2", "agent_3"]}]}


## ❓ FAQ

**Q: How does the conflict detection work?**
The server uses deterministic set math to calculate Jaccard similarity for agent goals, toolsets, and backstories. If any score exceeds your defined threshold, a conflict is flagged.

**Q: What is the default conflict threshold?**
The default threshold is 0.6. You can adjust this value using the `threshold` parameter in the `analyze_agent_team` or `check_agent_pair_conflict` tools.

**Q: Can I use this with CrewAI?**
Yes, this tool is specifically designed to solve design ambiguity in multi-agent frameworks like CrewAI by identifying redundant agent definitions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agent-role-conflict-detector](https://vinkius.com/mcp/agent-role-conflict-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Role Conflict Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-role-conflict-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Role Conflict Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-role-conflict-detector": {
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
