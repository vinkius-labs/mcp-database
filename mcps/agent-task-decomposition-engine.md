# Agent Task Decomposition Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-task-decomposition-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Break complex goals into structured subtasks with deterministic complexity scoring.

## Description
This MCP server provides precise tools for breaking down high-level objectives into actionable hierarchies. Use `decompose_task` to generate a structured tree of subtasks, `analyze_complexity` to calculate metrics like parallelism potential and optimal subtask counts, and `validate_dependencies` to detect circular references. It is designed to help AI agents plan effectively by quantifying task difficulty and ensuring logical task flow.


## Available Tools (3)
- **analyze_complexity**: Calculate the structural metrics of a previously decomposed task tree
- **decompose_task**: Break a high-level task into a hierarchical structure of subtasks and leaf actions
- **validate_dependencies**: Ensure the task decomposition does not contain logical loops


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Task Decomposition Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Decompose the task: 'Build a complete marketing campaign for a new eco-friendly water bottle'."

**🤖 AI Agent:**
> The task has been decomposed into: 1. Market Research, 2. Creative Asset Production, 3. Channel Selection, and 4. Campaign Launch.

---

**👤 You:**
> "Analyze the complexity of this task tree: {"root": "Plan Trip"}"

**🤖 AI Agent:**
> The complexity score is 1.5 with a parallelism potential of 1.0.

---

**👤 You:**
> "Check if these subtasks have circular dependencies: [Task A, Task B]"

**🤖 AI Agent:**
> The task structure is valid with no circular dependencies detected.


## ❓ FAQ

**Q: How is task complexity calculated?**
Complexity is a weighted sum of word count, domain specificity, and ambiguity, which is then scaled by the decomposition depth.

**Q: What happens if a task is too ambiguous?**
If the ambiguity score exceeds 0.8, the `decompose_task` tool will flag the task as too vague for reliable decomposition.

**Q: Can I detect circular dependencies between tasks?**
Yes, you can use the `validate_dependencies` tool to ensure your task hierarchy does not contain logical loops.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-task-decomposition-engine](https://vinkius.com/ai-agent-connect/agent-task-decomposition-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Task Decomposition Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-task-decomposition-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Task Decomposition Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-task-decomposition-engine": {
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
