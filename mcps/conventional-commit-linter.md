# Conventional Commit Linter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/conventional-commit-linter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Validate commit messages against Conventional Commates spec and determine SemVer impact.

## Description
The Conventional Commit Linter connects AI agents to your git workflow. It uses tools like `verify_commit_structure`, `analyze_breaking_change_presence`, `evaluate_subject_semantics`, and `classify_release_impact` to ensure every commit follows the standard, enabling automated changelogs and predictable versioning.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conventional Commit Linter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this commit is valid: 'feat(ui): add button'"

**🤖 AI Agent:**
> The commit structure is valid with type 'feat' and scope 'ui'.

---

**👤 You:**
> "Does 'fix: bug' contain a breaking change?"

**🤖 AI Agent:**
> No, no breaking change was detected in the message.

---

**👤 You:**
> "What is the SemVer impact of 'feat: add user profile'?"

**🤖 AI Agent:**
> The impact level is minor.


## ❓ FAQ

**Q: How does the linter validate a commit?**
It analyzes the message structure using `verify_commit_structure` to check for type, scope, and description. Tools available: `your_tool_name`.

**Q: Can it identify breaking changes?**
Yes, `analyze_breaking_change_presence` detects exclamation marks or BREAKING CHANGE footers.

**Q: How is the version impact determined?**
The `classify_release_impact` tool calculates if the change requires a major, minor, or patch update.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conventional-commit-linter](https://vinkius.com/mcp/conventional-commit-linter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Conventional Commit Linter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `conventional-commit-linter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Conventional Commit Linter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "conventional-commit-linter": {
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
