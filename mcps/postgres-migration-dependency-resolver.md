# Postgres Migration Dependency Resolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/postgres-migration-dependency-resolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Resolves the execution order of SQL migrations using graph theory to prevent deployment errors.

## Description
The Postgres Migration Dependency Resolver uses Kahn's algorithm and directed acycl-ic graphs (DAG) to determine the exact, deterministic sequence for executing database migrations. By analyzing dependencies between migration IDs, it identifies the correct execution order, detects circular references that would block deployment, and verifies the integrity of your dependency graph. Use `resolve_migration_order` to find the safe path, `validate_dependency_integrity` to catch ghost dependencies, and `analyze_down_stream_impact` to understand the blast radius of a single migration change.


## Available Tools (3)
- **resolve_migration_order**: Resolves the execution order of migrations
- **validate_dependency_integrity**: Validates that all dependencies exist
- **analyze_downstream_impact**: Analyzes the downstream impact of a migration change


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postgres Migration Dependency Resolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the execution order for these migrations: [{'id': 'm1', 'requires': []}, {'id': 'm2', 'requires': ['m1']}]"

**🤖 AI Agent:**
> The execution order is: m1, m2. Total migrations processed: 2.

---

**👤 You:**
> "Check if my migration dependencies are valid for: [{'id': 'v1', 'requires': ['v0']}]"

**🤖 AI Agent:**
> The integrity check failed. Missing dependency: v0.

---

**👤 You:**
> "What is the impact of changing migration 'init_schema' in my list?"

**🤖 AI Agent:**
> Changing 'init_schema' affects 5 migrations: ['users', 'profiles', 'orders', 'payments', 'logs'].


## ❓ FAQ

**Q: How does the tool detect circular dependencies?**
The `resolve_migration_order` tool uses Kahn's algorithm to track in-degrees. If migrations remain with non-zero in-degrees after the process, they are identified as part of a cycle.

**Q: What happens if I reference a migration ID that doesn't exist?**
You should use the `validate_dependency_integrity` tool. It will return `isValid: false` and provide a list of all missing migration IDs found in your requirements.

**Q: Can I see which migrations are affected if a specific migration fails?**
Yes, the `analyze_downstream_impact` tool performs a reverse lookup to find all migrations that transitively depend on your target ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/postgres-migration-dependency-resolver](https://vinkius.com/ai-agent-connect/postgres-migration-dependency-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Postgres Migration Dependency Resolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `postgres-migration-dependency-resolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Postgres Migration Dependency Resolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "postgres-migration-dependency-resolver": {
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
