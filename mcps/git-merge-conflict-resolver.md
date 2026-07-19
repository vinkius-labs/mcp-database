# Git Merge Conflict Resolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/git-merge-conflict-resolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automatically identify and resolve Git merge conflict markers using deterministic strategies.

## Description
This MCP server provides a deterministic engine for handling Git merge conflicts. It allows AI agents to locate conflict regions with `identify_conflicts`, apply specific resolution logic via `resolve_conflicts` (including strategies like union or prioritizing changes), and audit the final result using `verify_integrity`. This ensures that files are cleaned of all structural markers without manual intervention.


## Available Tools (3)
- **identify_conflicts**: Locate Git merge conflict markers in a file
- **resolve_conflicts**: Resolve Git merge conflicts using a specific strategy
- **verify_integrity**: Verify that no Git conflict markers remain in a text block


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Git Merge Conflict Resolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all merge conflicts in this file content."

**🤖 AI Agent:**
> I have identified 2 conflict zones in the provided text, located at indices 145-320 and 560-785.

---

**👤 You:**
> "Resolve the conflicts in this text using the union strategy."

**🤖 AI Agent:**
> The conflicts have been resolved. The resulting content now contains both segments merged into a single continuous block without any markers.

---

**👤 You:**
> "Check if this file is clean of merge markers."

**🤖 AI Agent:**
> The integrity check passed. No Git conflict markers were found in the provided content.


## ❓ FAQ

**Q: What strategies can I use to resolve conflicts?**
You can use 'accept_current', 'accept_incoming', 'union', or 'prioritize_claude_changes' via the `resolve_conflicts` tool.

**Q: How do I know if a file is still conflicted?**
Use the `verify_integrity` tool to scan for any remaining Git markers like <<<<<<<, =======, or >>>>>>>.

**Q: Can this tool find all conflict zones in a file?**
Yes, the `identify_conflicts` tool scans the entire provided content and returns the exact start and end indices of every detected conflict zone.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/git-merge-conflict-resolver](https://vinkius.com/mcp/git-merge-conflict-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Git Merge Conflict Resolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `git-merge-conflict-resolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Git Merge Conflict Resolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "git-merge-conflict-resolver": {
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
