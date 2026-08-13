# Git Workflow Guardian MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/git-workflow-guardian)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Enforces git workflow rules and repository hygiene.

## Description
Git Workflow Guardian is an enforcement engine that validates git operations against predefined organizational rules. It prevents security breaches and maintains repository hygiene by checking branch naming, commit message formats, and protected branch restrictions. Use `validate_git_action` to verify operations, `check_branch_naming` for branch compliance, and `audit_commit_integrity` to ensure commit messages follow conventional standards and include required issue references.


## Available Tools (3)
- **audit_commit_integrity**: Checks commit integrity
- **check_branch_naming**: Verifies branch naming
- **validate_git_action**: Validates if a git operation complies with rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Git Workflow Guardian** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this git action allowed: a push to the main branch?"

**🤖 AI Agent:**
> No, pushing to the main branch is prohibited by the protected branch rule.

---

**👤 You:**
> "Check if the branch name 'feature/login-fix' is valid."

**🤖 AI Agent:**
> Yes, the branch name 'feature/login-fix' follows the required naming convention.

---

**👤 You:**
> "Validate this commit message: 'feat: add user auth [ISSUE-123]'"

**🤖 AI Agent:**
> The commit message is valid and includes the required issue reference.


## ❓ FAQ

**Q: What does this tool validate?**
It validates git actions like commits and pushes, branch naming conventions, and commit message integrity using `validate_git_action` and `audit_commit_integrity`.

**Q: How can I check if my branch name is valid?**
You can use the `check_branch_naming` tool to verify if your proposed branch name follows the required organizational regex patterns.

**Q: Does it enforce conventional commits?**
Yes, the `audit_commit_integrity` tool ensures that commit messages adhere to conventional commit formats and include necessary issue references.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/git-workflow-guardian](https://vinkius.com/mcp/git-workflow-guardian)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Git Workflow Guardian** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `git-workflow-guardian` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Git Workflow Guardian** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "git-workflow-guardian": {
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
