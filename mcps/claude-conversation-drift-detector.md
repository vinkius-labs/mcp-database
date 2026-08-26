# Claude Conversation Drift Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/claude-conversation-drift-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Monitors AI agent focus by detecting task drift and topic shifts.

## Description
This MCP server provides tools to ensure AI agents stay aligned with their primary objectives. It identifies when an agent deviates from the user's intent by analyzing the semantic relevance of recent actions against the original task description. Using `analyze_conversation_drift`, agents can check if their current trajectory is on track. The `detect_topic_shift` tool identifies sudden jumps to unrelated subjects, while `get_task_relevance_summary` provides a percentage of task coverage based on keyword overlap. This is essential for preventing hallucination loops and tangential sub-tasks in complex workflows.


## Available Tools (3)
- **analyze_conversation_drift**: Determines if the current sequence of agent actions is staying aligned with the original user goal
- **get_task_relevance_summary**: Provides a high-level summary of how much of the task has been addressed based on keyword coverage
- **detect_topic_shift**: Identifies if the agent has abruptly switched to a completely unrelated topic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claude Conversation Drift Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my current conversation is still focused on the original task."

**🤖 AI Agent:**
> The agent is currently on track with a relevance score of 0.85.

---

**👤 You:**
> "Has the agent switched to a new topic recently?"

**🤖 AI Agent:**
> No sudden topic shifts have been detected in the recent action history.

---

**👤 You:**
> "How much of the task have I completed so far?"

**🤖 AI Agent:**
> The task coverage is currently at 75%, with the following unaddressed keywords: [keyword1, keyword2].


## ❓ FAQ

**Q: How does the drift detection work?**
It uses Jaccard similarity to compare keywords extracted from the original task with keywords extracted from recent agent actions like `analyze_conversation_drift` or file changes.

**Q: Can I adjust the sensitivity of the drift detection?**
Yes, you can specify a `driftThreshold` in the `analyze_conversation_drift` tool to control how sensitive the rolling average relevance check is.

**Q: What is a topic shift?**
A topic shift is detected when there is a sudden loss of keyword overlap between the current action and the previous one, indicating the agent has jumped to a new subject.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/claude-conversation-drift-detector](https://vinkius.com/ai-agent-connect/claude-conversation-drift-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claude Conversation Drift Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claude-conversation-drift-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claude Conversation Drift Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claude-conversation-drift-detector": {
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
