# claude-task-completion-verifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/claude-task-completion-verifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

A deterministic verification engine that validates task fulfillment by checking files, content, and command execution.

## Description
This MCP server provides a deterministic verification engine to ensure AI agents have truly completed their tasks. Instead of relying on intuition, it uses objective evidence by checking for file existence, matching regex patterns, and executing shell commands like tests or builds. Use `verify_task_completion` to perform a full audit, `check_file_integrity` for quick file and pattern checks, or `execute_environment_check` to run technical health commands. It bridges the gap between task description and verifiable reality.


## Available Tools (3)
- **check_file_integrity**: Verifies that specific files exist and contain expected content patterns
- **verify_task_completion**: Performs a full audit of a task by evaluating all provided criteria
- **execute_environment_check**: Runs shell commands to verify the technical health of the workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **claude-task-completion-verifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify if the file 'src/engine/index.ts' exists and contains the word 'verify_task_completion'."

**🤖 AI Agent:**
> The file exists and the pattern matches successfully.

---

**👤 You:**
> "Run the tests in the workspace to see if they pass."

**🤖 AI Agent:**
> Tests passed successfully with exit code 0.

---

**👤 You:**
> "Perform a full audit of the task: 'Implement the verification engine'."

**🤖 AI Agent:**
> Task is 100% complete based on all provided criteria.


## ❓ FAQ

**Q: How does the verification work?**
The engine uses `verify_task_completion` to evaluate specific criteria such as file existence, content matching, or command exit codes to provide a mathematical completion percentage.

**Q: Can I run shell commands?**
Yes, you can use `execute_environment_check` to run any shell command and verify its exit code.

**Q: What is the difference between the tools?**
Use `check_file_integrity` for simple file/pattern checks, `execute_environment_check` for running commands, and `verify_task_completion` for a comprehensive multi-criteria audit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/claude-task-completion-verifier](https://vinkius.com/ai-agent-connect/claude-task-completion-verifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **claude-task-completion-verifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claude-task-completion-verifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **claude-task-completion-verifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claude-task-completion-verifier": {
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
