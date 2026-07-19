# Dead Code & Export Auditor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dead-code-export-auditor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Identify unused exports and unreachable code paths using deterministic AST-driven reference counting.

## Description
The Dead Code & Export Auditor connects AI agents to your codebase's structural integrity. By parsing files into an Abstract Syntax Tree (AST), it builds a precise symbol table and performs deterministic reference counting to find unused exports and unreachable code blocks. Use `audit_file` to inspect specific files, `audit_project` for global dependency analysis across directories, or `get_symbol_manifest` to check the usage statistics of a specific identifier.


## Available Tools (3)
- **get_symbol_metadata**: Retrieves usage statistics for a specific identifier
- **audit_file**: Analyzes a single file for unused exports and unreachable code
- **audit_project**: Performs a global audit across an entire directory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dead Code & Export Auditor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if there is any dead code in my current directory."

**🤖 AI Agent:**
> The audit of the current directory found 3 unused exports and 2 unreachable blocks, resulting in a dead code density ratio of 0.05.

---

**👤 You:**
> "Analyze src/utils/math.ts for unused symbols."

**🤖 AI Agent:**
> In src/utils/math.ts, the symbol `calculateInternalSum` is unused (line 42) and there is an unreachable block starting at line 55.

---

**👤 You:**
> "What is the reference count for the 'Config' class in src/config.ts?"

**🤖 AI Agent:**
> The symbol `Config` in src/config.ts has a reference count of 12 and is not marked as an entry point.


## ❓ FAQ

**Q: How does the auditor detect unused exports?**
The tool performs an AST traversal to build a symbol table and increments reference counts whenever a symbol is encountered. If `audit_project` finds a symbol with zero references, it is flagged as unused.

**Q: Can I audit specific file extensions?**
Yes, when using `audit_project`, you can provide an optional list of extensions like ['.ts', '.js'] to narrow the scope of the scan.

**Q: Does it identify unreachable code?**
Yes, the `audit_file` tool identifies code blocks located after terminal statements like return, throw, or break.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dead-code-export-auditor](https://vinkius.com/mcp/dead-code-export-auditor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dead Code & Export Auditor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dead-code-export-auditor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dead Code & Export Auditor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dead-code-export-auditor": {
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
