# Claude Commit Diff Reviewer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/claude-commit-diff-reviewer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Analyzes git diffs against task descriptions to detect scope creep and unwanted patterns.

## Description
This MCP server provides tools to verify that AI-generated code changes align with the original user intent. It parses git diffs into individual hunks and uses keyword matching to classify changes as intended, cascading, or unrelated. It also scans for unwanted patterns like debug statements or TODOs. Use `analyze_diff_relevance` to check for scope creep, `summarize_change_distribution` for statistical impact, and `identify_file_scope` to see which files were modified.


## Available Tools (3)
- **analyze_diff_relevance**: 
- **summarize_change_distribution**: 
- **identify_file_scope**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claude Commit Diff Reviewer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this diff to see if it matches the task: 'Update the user authentication logic'"

**🤖 AI Agent:**
> The diff contains 3 intended changes and 0 unrelated changes. No flagged patterns were detected.

---

**👤 You:**
> "Check the distribution of changes in this git diff."

**🤖 AI Agent:**
> The changes affect 4 files with a total of 45 lines modified. The intended ratio is 0.85.

---

**👤 You:**
> "Which files were modified in this diff?"

**🤖 AI Agent:**
> The modified files are src/auth.ts, src/utils.ts, and tests/auth.test.ts. The changes are concentrated.


## ❓ FAQ

**Q: How does the tool determine if a change is intended?**
The tool uses deterministic keyword matching to compare the content of each diff hunk against the keywords provided in the task description.

**Q: What are 'unrelated changes'?**
Unrelated changes are modifications in the git diff that have no keyword overlap with the original task description, indicating potential scope creep.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, VS Code, Claude Desktop, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/claude-commit-diff-reviewer](https://vinkius.com/ai-agent-connect/claude-commit-diff-reviewer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claude Commit Diff Reviewer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claude-commit-diff-reviewer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claude Commit Diff Reviewer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claude-commit-diff-reviewer": {
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
