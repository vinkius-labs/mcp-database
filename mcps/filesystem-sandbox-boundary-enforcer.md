# Filesystem Sandbox Boundary Enforcer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/filesystem-sandbox-boundary-enforcer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Enforces strict path boundaries and prevents traversal attacks.

## Description
This MCP server provides a security engine to prevent path traversal and unauthorized file system access. It uses deterministic string manipulation to resolve paths, expanding `..` segments and removing redundant slashes. Use `validate_path_access` to check if a requested path is permitted within your allowed roots, or use `preview_path_expansion` to see how a complex path will be normalized before validation.


## Available Tools (3)
- **analyze_root_integrity**: Audits a list of potentially allowed directories to ensure the configuration itself does not contain forbidden zones
- **preview_path_expansion**: segments and redundant slashes in the input path.

Demonstrates how a messy or complex path will be cleaned and resolved before any permission checks are applied
- **validate_path_access**: Returns permission status, resolved path, and violation reason if denied.

Determines if a specific file system request is safe and permitted under current security policies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Filesystem Sandbox Boundary Enforcer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the path '/var/www/html/../etc/passwd' allowed if my root is '/var/www/html'?"

**🤖 AI Agent:**
> No, the resolved path is `/etc/passwd`, which triggers a blocklist violation.

---

**👤 You:**
> "Show me how the path '///home//user/./docs/../config' will look after expansion."

**🤖 AI Agent:**
> /home/user/config

---

**👤 You:**
> "Check if '/mnt/data' is a safe root directory."

**🤖 AI Agent:**
> The directory `/mnt/data` is safe and does not match any forbidden patterns in the blocklist.


## ❓ FAQ

**Q: How does the server prevent path traversal attacks?**
The server resolves all `..` segments and redundant slashes using deterministic string manipulation before checking if the resulting path starts with an allowed root or matches a forbidden blocklist.

**Q: What directories are blocked by default?**
The server blocks access to sensitive system paths including `/etc`, `/root`, and `~/.ssh` via a hardcoded blocklist.

**Q: Can I use this to audit my existing configuration?**
Yes, you can use the `analyze_root_integrity` tool to check if any of your provided root directories overlap with forbidden system paths.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/filesystem-sandbox-boundary-enforcer](https://vinkius.com/mcp/filesystem-sandbox-boundary-enforcer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Filesystem Sandbox Boundary Enforcer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `filesystem-sandbox-boundary-enforcer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Filesystem Sandbox Boundary Enforcer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "filesystem-sandbox-boundary-enforcer": {
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
