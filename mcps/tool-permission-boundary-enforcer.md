# Tool Permission Boundary Enforcer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tool-permission-boundary-enforcer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Enforces deterministic permission boundaries for tool execution to prevent unbounded access.

## Description
The Tool Permission Boundary Enforcer provides a deterministic security layer for LLM agents. It prevents unbounded execution by maintaining a strict permission matrix that maps tool names to allowed operations and specific constraint patterns. Using `check_permission`, agents can verify if a requested action is permitted before execution. The `list_boundaries` tool allows for inspection of active rules, while `validate_resource_pattern` provides a way to test resource paths or URLs against constraints. This ensures that tools like file writers or network clients operate only within predefined, safe boundaries.


## Available Tools (3)
- **check_permission**: Determines if a specific tool operation is permitted under current boundary rules
- **list_boundaries**: Retrieves the current active permission boundaries for inspection
- **validate_resource_pattern**: Tests a specific resource string against the regex or exact match rules of a given tool/operation pair


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tool Permission Boundary Enforcer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it okay to write a file to /home/user/config.json using the file_write operation?"

**🤖 AI Agent:**
> The `check_permission` tool would evaluate this against the permission matrix to determine if the path is within the allowed boundaries.

---

**👤 You:**
> "What are the current boundaries for the network tool?"

**🤖 AI Agent:**
> You can call `list_boundaries` with the filter for the network tool to see its specific allowed operations and regex patterns.

---

**👤 You:**
> "Can I validate if 'https://api.example.com' is a permitted URL?"

**🤖 AI Agent:**
> You can use `validate_resource_pattern` to check if that specific URL matches the regex patterns defined for the network tool.


## ❓ FAQ

**Q: How does the enforcer prevent unauthorized tool access?**
It uses `check_permission` to validate every requested operation against a predefined permission matrix. If the operation or the target resource does not match the allowed patterns, the request is blocked.

**Q: Can I see what tools are currently restricted?**
Yes, you can use the `list_boundaries` tool to retrieve the current active permission boundaries and inspect the allowed operations and patterns.

**Q: How do I test a path before using it?**
You can use `validate_resource_pattern` to test a specific resource string against the regex or exact match rules of a tool/operation pair without actually executing the tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tool-permission-boundary-enforcer](https://vinkius.com/mcp/tool-permission-boundary-enforcer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tool Permission Boundary Enforcer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tool-permission-boundary-enforcer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tool Permission Boundary Enforcer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tool-permission-boundary-enforcer": {
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
