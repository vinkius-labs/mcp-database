# Dependency Coupling Fitness Function MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dependency-coupling-fitness-function)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops](../categories/devops.md)

Enforce clean architecture boundaries by validating dependency directions.

## Description
This MCP server acts as an architectural guardrail for your codebase. It allows AI agents to perform automated audits of software dependencies using tools like `audit_imports` and `identify_layer`. By defining prohibited relationships between layers (e.g., 'presentation cannot depend on data'), you can prevent architectural erosion and ensure that your project adheres to clean architecture principles. The server maps file paths to logical layers and checks every import statement against your specified rules.


## Available Tools (3)
- **identify_layer**: Determines which architectural layer a specific file belongs to based on its path
- **audit_imports**: Performs a full architectural audit on a file by checking all its imports
- **check_rule_compliance**: Validates whether a dependency from one specific layer to another is permitted


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dependency Coupling Fitness Function** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my current file violates any architecture rules."

**🤖 AI Agent:**
> The audit of `src/presentation/controller.ts` is complete. No violations were found; all imports comply with your defined architectural boundaries.

---

**👤 You:**
> "What layer does 'src/data/repository.ts' belong to?"

**🤖 AI Agent:**
> The file `src/data/repository.ts` has been identified as belonging to the 'data' layer.

---

**👤 You:**
> "Verify if a dependency from presentation to data is allowed."

**🤖 AI Agent:**
> The rule check returned that this connection is not allowed under your current architecture rules.


## ❓ FAQ

**Q: How does the server identify architectural layers?**
The `identify_layer` tool parses the file path and looks for specific directory markers to determine which layer (e.g., domain, data, or presentation) the file belongs to.

**Q: Can I use this to prevent circular dependencies?**
Yes, by using `audit_imports` with rules that forbid specific layer-to-layer connections, you can detect and block illegal dependency paths.

**Q: What AI clients are compatible?**
This server is accessible via Vinkius Edge and works with Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dependency-coupling-fitness-function](https://vinkius.com/mcp/dependency-coupling-fitness-function)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dependency Coupling Fitness Function** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dependency-coupling-fitness-function` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dependency Coupling Fitness Function** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dependency-coupling-fitness-function": {
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
