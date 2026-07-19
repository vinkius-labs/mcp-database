# Git Branch Naming Linter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/git-branch-naming-linter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Validates git branch names against specific naming conventions and structural patterns.

## Description
This MCP server provides tools to ensure repository cleanliness by enforcing branch naming standards. You can use `check_branch_syntax` to verify character integrity, casing styles like kebab-case or snake_case, and maximum length constraints. The `verify_structural_pattern` tool checks for required segments like type and ticket ID, while `audit_branch_batch` allows you to analyze multiple branches at once to identify non-compliant names in your workflow.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Git Branch Naming Linter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if 'feature/PROJ-123-login' is valid for kebab-case."

**🤖 AI Agent:**
> The branch name 'feature/PROJ-123-login' is valid and follows the kebab-case convention.

---

**👤 You:**
> "Is 'bugfix_task-456' a valid snake_case branch?"

**🤖 AI Agent:**
> No, 'bugfix_task-456' is invalid because it contains a hyphen, which is not allowed in snake_case.

---

**👤 You:**
> "Audit these branches: ['feat/JIRA-1', 'hotfix/fix-it'] using segments type, id, description."

**🤖 AI Agent:**
> The audit found 0% compliance. The branch 'feat/JIRA-1' is missing the description segment.


## ❓ FAQ

**Q: What casing styles are supported?**
The linter supports kebab-case, snake_case, and camelCase. Tools available: `your_tool_name`.

**Q: Can I validate Jira ticket IDs?**
Yes, by using the structural pattern verification tool with a custom regex.

**Q: How does the batch audit work?**
You provide a list of branch names, and the tool returns a compliance rate and a summary of failures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/git-branch-naming-linter](https://vinkius.com/mcp/git-branch-naming-linter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Git Branch Naming Linter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `git-branch-naming-linter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Git Branch Naming Linter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "git-branch-naming-linter": {
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
