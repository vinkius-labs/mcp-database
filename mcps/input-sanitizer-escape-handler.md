# Input Sanitizer & Escape Handler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/input-sanitizer-escape-handler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Protects AI agents from shell injection, path traversal, and payload vulnerabilities.

## Description
This MCP server provides a deterministic defense layer between untrusted LLM-generated strings and sensitive execution environments. It prevents common vulnerabilities like shell injection, path traversal, and structural payload corruption. Use `sanitize_shell_command` to strip dangerous metacharacters, `sanitize_file_path` to neutralize directory navigation, `sanitize_structured_payload` for JSON/XML integrity, and `sanitize_strict_whitelist` for pattern-based restrictions.


## Available Tools (4)
- **sanitize_file_path**: 
- **sanitize_shell_command**: 
- **sanitize_strict_whitelist**: 
- **sanitize_structured_payload**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Input Sanitizer & Escape Handler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Sanitize this shell command input: 'cat /etc/passwd; rm -rf /'"

**🤖 AI Agent:**
> cat /etc/passwd rm -rf /

---

**👤 You:**
> "Clean this file path: '../../etc/shadow'"

**🤖 AI Agent:**
> etc/shadow

---

**👤 You:**
> "Sanitize this string for a JSON payload: 'User "admin" logged in'"

**🤖 AI Agent:**
> User \"admin\" logged in


## ❓ FAQ

**Q: How does this protect against shell injection?**
The `sanitize_shell_command` tool identifies and strips shell metacharacters like semicolons, pipes, and backticks, ensuring the string cannot be used to chain unauthorized commands.

**Q: Can I use this to secure JSON payloads?**
Yes, use `sanitize_structured_payload` with the 'json' target format to escape quotes and maintain structural integrity.

**Q: How do I prevent path traversal attacks?**
The `sanitize_file_path` tool detects and removes parent directory navigation sequences like '../' to prevent unauthorized file system access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/input-sanitizer-escape-handler](https://vinkius.com/mcp/input-sanitizer-escape-handler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Input Sanitizer & Escape Handler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `input-sanitizer-escape-handler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Input Sanitizer & Escape Handler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "input-sanitizer-escape-handler": {
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
