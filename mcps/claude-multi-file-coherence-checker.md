# Claude Multi-File Coherence Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/claude-multi-file-coherence-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Ensures structural integrity across codebases by auditing imports, signatures, and type consistency.

## Description
This MCP server prevents 'partial updates' where an AI modifies a definition but fails to update its consumers. It provides a deterministic validation engine to ensure that changes to exports, function signatures, and types propagate correctly across the entire project. Use `validate_import_coherence` to find broken imports, `check_signature_consistency` to verify function call sites, and `audit_type_propagation` to ensure type integrity. It is designed to maintain codebase health during complex multi-file modifications.


## Available Tools (3)
- **audit_type_propagation**: Validates that changes to types or interfaces have not broken downstream consumers
- **check_signature_consistency**: Detects if modified function/class signatures still match their call sites
- **validate_import_coherence**: Validates that imports in the project correctly reference existing exports in the changed files


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claude Multi-File Coherence Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just renamed a function in `src/utils.ts`. Can you check if I broke any imports?"

**🤖 AI Agent:**
> I have run `validate_import_coherence` and found 2 broken imports in `src/main.ts` at lines 12 and 45 due to the renamed function.

---

**👤 You:**
> "I added a new required parameter to the `processData` function. Did I miss any call sites?"

**🤖 AI Agent:**
> The `check_signature_consistency` tool identified 1 missing update in `src/processor.ts` at line 82 where the new parameter is required.

---

**👤 You:**
> "I changed the structure of the `User` interface. Is the rest of the code still type-safe?"

**🤖 AI Agent:**
> After running `audit_type_propagation`, I found 1 type mismatch in `src/auth.ts` at line 15 because the `User` interface no longer contains the `email` property.


## ❓ FAQ

**Q: What problem does this tool solve?**
It solves the problem of partial updates, where an AI agent modifies a function or type in one file but misses the corresponding updates in other files that use them.

**Q: How does it detect broken imports?**
By using `validate_import_coherence`, the tool maps exported symbols in changed files and scans the project for import statements that no longer point to valid exports.

**Q: Can it check if function arguments are still correct?**
Yes, the `check_signature_consistency` tool specifically checks if modified function or class signatures still match their call sites, including parameter counts and types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/claude-multi-file-coherence-checker](https://vinkius.com/mcp/claude-multi-file-coherence-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claude Multi-File Coherence Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claude-multi-file-coherence-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claude Multi-File Coherence Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claude-multi-file-coherence-checker": {
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
