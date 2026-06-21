# Cerbos MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cerbos)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Decouple authorization logic from your application. Evaluate permissions, generate query plans, and manage access control via AI.

## Description
Connect your **Cerbos** instance to any AI agent to manage complex authorization policies through natural language conversation.

### What you can do

- **Permission Evaluation** — Use `check_resources` to instantly verify if a principal can perform specific actions on resources based on your policies.
- **Query Planning** — Generate AST-based query plans with `plan_resources` to filter database results according to user permissions.
- **AuthZEN Compliance** — Leverage standardized access requests using `authzen_evaluation` and `authzen_evaluations` tools.
- **System Monitoring** — Check instance health and build metadata using `get_server_info` and `get_authzen_config`.

### How it works

1. Subscribe to this server
2. Provide your Cerbos instance base URL (e.g., `http://localhost:3592`)
3. Start auditing and testing your access control logic directly from your chat interface

### Who is this for?

- **Software Engineers** — debug complex RBAC/ABAC policies without manual API calls
- **Security Auditors** — verify permission logic across different roles and resource attributes
- **DevOps Teams** — monitor Cerbos instance metadata and configuration status


## Available Tools
- **get_authzen_config**: Returns endpoint URLs for the AuthZEN APIs
- **authzen_evaluation**: Single action evaluation using the AuthZEN entity model
- **authzen_evaluations**: Supports execute_all, deny_on_first_deny, and permit_on_first_permit semantics.

Batch evaluation of multiple access requests using AuthZEN
- **check_resources**: This is a read-only evaluation.

Evaluates permissions for a principal on a set of resources
- **plan_resources**: Produces a query plan for obtaining a list of resources a principal is allowed to access
- **get_server_info**: Returns the version and build details of the Cerbos instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cerbos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if principal 'user_123' with role 'editor' can 'edit' resource 'document:abc'."

**🤖 AI Agent:**
> I've evaluated the request using `check_resources`. For principal 'user_123', the action 'edit' on resource 'document:abc' is ALLOWED based on the current policy.

---

**👤 You:**
> "Generate a query plan for 'view' action on 'expense' resources for principal 'manager'."

**🤖 AI Agent:**
> Using `plan_resources`, I've generated the AST. The condition requires the 'department' attribute of the resource to match the principal's department. You can apply this filter to your database query.

---

**👤 You:**
> "Show me the Cerbos server build details."

**🤖 AI Agent:**
> I've retrieved the server info using `get_server_info`. Your instance is running version 0.34.0, built on 2024-01-15.


## ❓ FAQ

**Q: Can I check if a specific user has permission to access a resource?**
Yes. Use the `check_resources` tool by providing the principal (user) details and the resource information. The agent will return an evaluation of allowed or denied actions.

**Q: How do I generate a filter for my database based on user permissions?**
Use the `plan_resources` tool. It produces a query plan (AST) that you can use to construct database queries, ensuring users only see records they are authorized to access.

**Q: Is it possible to verify the Cerbos server version via AI?**
Yes, the `get_server_info` tool retrieves the version, build date, and commit hash of your connected Cerbos instance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cerbos](https://vinkius.com/mcp/cerbos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cerbos** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cerbos` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cerbos** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cerbos": {
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
