# Claude State Checkpoint Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/claude-state-checkpoint-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create deterministic project snapshots to undo unwanted changes.

## Description
The Claude State Checkpoint Manager provides a way to create deterministic snapshots of your project state. By using `create_checkpoint`, you can capture a point-in-time record of file hashes, git commit history, and environment variables. If unwanted changes occur during a session, you can use `compare_to_checkpoint` to see exactly what changed or `rollback_to_checkpoint` to revert the entire workspace to a previous state. This tool is essential for maintaining stability during long AI-driven development sessions.


## Available Tools (4)
- **compare_to_checkpoint**: Identifies what has changed in the workspace since a specific checkpoint was taken
- **create_checkpoint**: Captures the current state of the workspace to allow for future comparison or rollback
- **list_checkpoints**: Provides an overview of all currently saved project states
- **rollback_to_checkpoint**: This is a destructive action.

Reverts the entire project state to the exact moment a specific checkpoint was created


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claude State Checkpoint Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Save the current state of my project."

**🤖 AI Agent:**
> Checkpoint created successfully with ID: cp_12345.

---

**👤 You:**
> "What files have changed since checkpoint cp_12345?"

**🤖 AI Agent:**
> Since checkpoint cp_12345, the following files have changed: src/main.ts (modified), README.md (modified), and config.json (deleted).

---

**👤 You:**
> "Undo my recent changes and go back to checkpoint cp_12345."

**🤖 AI Agent:**
> Workspace successfully rolled back to checkpoint cp_12345 (commit: a1b2c3d).


## ❓ FAQ

**Q: How do I see what changed since my last snapshot?**
You can use the `compare_to_checkpoint` tool with your specific checkpoint ID to see a detailed diff of added, modified, and deleted files.

**Q: Is the rollback process destructive?**
Yes, `rollback_to_checkpoint` performs a git checkout to revert files to a previous state. Ensure you have committed any important work before rolling back.

**Q: How many checkpoints can I keep?**
By default, the system keeps up to 10 checkpoints using a FIFO (First-In-First-Out) eviction strategy. You can adjust this limit using `create_checkpoint` with the `maxCheckpoints` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/claude-state-checkpoint-manager](https://vinkius.com/mcp/claude-state-checkpoint-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claude State Checkpoint Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claude-state-checkpoint-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claude State Checkpoint Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claude-state-checkpoint-manager": {
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
