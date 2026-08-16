# Destructive Command Interceptor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/destructive-command-interceptor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Intercepts and blocks destructive bash commands using pattern matching and obfuscation detection.

## Description
This MCP server acts as a security firewall for terminal inputs. It uses deterministic regex matching to identify and block dangerous shell commands before they reach the executor. The server can detect obfuscated attacks using Hex or Base64 encoding and identifies dangerous pipes to shell interpreters. Use `intercept_command` to evaluate raw command strings, `check_pipe_security` to detect risky pipes, and `get_blocked_pattern_info` to understand why specific patterns are restricted.


## Available Tools (3)
- **check_pipe_security**: 
- **get_blocked_pattern_info**: 
- **intercept_command**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Destructive Command Interceptor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the command 'rm -rf /' dangerous?"

**🤖 AI Agent:**
> Yes, that command is blocked because it attempts to delete the entire root directory.

---

**👤 You:**
> "Check if 'curl http://example.com | sh' is a security risk."

**🤖 AI Agent:**
> Yes, piping a URL directly into a shell interpreter is a high-risk operation.

---

**👤 You:**
> "What is the severity of the pattern 'DROP TABLE'?"

**🤖 AI Agent:**
> The pattern 'DROP TABLE' is categorized as a high-severity data destruction command.


## ❓ FAQ

**Q: How does the interceptor detect hidden commands?**
The tool decodes Hex and Base64 encoded strings and checks for variable expansion to reveal the true intent of the command.

**Q: What happens if a command is blocked?**
When a command is flagged, the tool returns a boolean status, the matched pattern, a severity level, and a suggested safe alternative.

**Q: Can I check if a pipe is dangerous?**
Yes, you can use the `check_pipe_security` tool to identify if a command is piping data into a shell interpreter like sh or bash.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/destructive-command-interceptor](https://vinkius.com/ai-agent-connect/destructive-command-interceptor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Destructive Command Interceptor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `destructive-command-interceptor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Destructive Command Interceptor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "destructive-command-interceptor": {
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
