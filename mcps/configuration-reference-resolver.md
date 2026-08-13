# Configuration Reference Resolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/configuration-reference-resolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

A deterministic engine for resolving template placeholders and cross-references within nested agent configuration dictionaries.

## Description
This MCP server provides a deterministic engine to transform raw configuration objects into fully resolved ones. It identifies and replaces placeholders using both ${KEY} and {{KEY}} syntax by performing a depth-first traversal of the configuration graph. The server includes specialized tools like `resolve_configuration` for full object resolution, `validate_reference_syntax` for pattern checking, and `detect_circularity` to prevent infinite loops in dependency chains. It is designed to manage complex configuration tiers, from static Base Tier values to high-level Agent Tier personas.


## Available Tools (3)
- **detect_circularity**: Inspects a set of dependencies to find infinite loops
- **resolve_configuration**: Performs the full resolution process on a configuration object
- **validate_reference_syntax**: Checks if a given string matches the allowed reference patterns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Configuration Reference Resolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Resolve this configuration: {"name": "${USER.name}"} with context {"USER": {"name": "Alice"}}"

**🤖 AI Agent:**
> {"name": "Alice"}

---

**👤 You:**
> "Check if this string is a valid reference: {{MY_KEY}}"

**🤖 AI Agent:**
> True

---

**👤 You:**
> "Is this configuration valid: {"a": "${b}"} where b is not in context?"

**🤖 AI Agent:**
> The reference '${b}' is unresolved.


## ❓ FAQ

**Q: What does the `resolve_configuration` tool do?**
The `resolve_configuration` tool takes a raw configuration object and a context dictionary, then replaces all valid placeholders with their corresponding values from the context.

**Q: How does the engine handle circular references?**
The engine uses `detect_circularity` to inspect the dependency graph. If a loop is detected during traversal, the engine stops that branch and records the circular path to prevent infinite loops.

**Q: What syntax is supported for placeholders?**
The engine supports two syntax patterns: ${KEY} and {{KEY}}. You can use `validate_reference_syntax` to check if a specific string follows these rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/configuration-reference-resolver](https://vinkius.com/mcp/configuration-reference-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Configuration Reference Resolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `configuration-reference-resolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Configuration Reference Resolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "configuration-reference-resolver": {
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
