# Cerbos (Access Control) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cerbos-access-control)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Decouple authorization from your code. Manage policies, check permissions, and audit access control directly through your AI agent.

## Description
Connect your **Cerbos** instance to any AI agent to streamline authorization management and policy auditing through natural language.

### What you can do

- **Permission Checks** — Use `check_resources` to evaluate if a principal (user) has the rights to perform specific actions on resources.
- **Query Planning** — Generate AST query plans with `plan_resources` to filter database results based on complex authorization logic.
- **Policy Management** — List, retrieve, add, or delete policies (RBAC/ABAC) using the Admin API tools like `list_policies` and `add_policy`.
- **Schema & Auditing** — Inspect resource schemas and review access logs with `list_auditLogs` to ensure compliance.
- **Health & Metrics** — Monitor your PDP (Policy Decision Point) status with `get_health` and `get_metrics` directly from the chat.

### How it works

1. Subscribe to this server
2. Enter your Cerbos PDP URL and Admin credentials (if required for policy management)
3. Start auditing and managing your access control logic from Claude, Cursor, or any MCP client

### Who is this for?

- **Security Engineers** — quickly audit existing policies and verify permission logic without manual API calls
- **Backend Developers** — test authorization scenarios and generate database filter plans during development
- **Compliance Officers** — retrieve audit logs and policy definitions to ensure organizational security standards


## Available Tools (19)
- **add_policy**: Add a new policy
- **add_schema**: Add or update a schema
- **authzen_evaluation**: Perform a single AuthZEN access evaluation
- **authzen_evaluations**: Perform batch AuthZEN access evaluations
- **check_resources**: Check permissions for a set of resources
- **delete_policy**: Delete a policy by ID
- **disable_policy**: Disable a policy
- **enable_policy**: Enable a policy
- **get_authzen_config**: Get AuthZEN configuration metadata
- **get_health**: Get Cerbos health status
- **get_metrics**: Get Prometheus metrics from Cerbos
- **get_policy**: Get a specific policy by ID
- **get_schema**: Get a specific schema by ID
- **get_server_info**: Get Cerbos server version and build information
- **list_audit_logs**: List audit logs
- **list_policies**: List all policies
- **list_schemas**: List all schemas
- **plan_resources**: Produce a query plan (AST) for filtering resources
- **update_policy**: Update an existing policy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cerbos (Access Control)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if user 'user_123' with role 'admin' can 'delete' the resource 'document:abc'."

**🤖 AI Agent:**
> I've checked the permissions using `check_resources`. For principal 'user_123', the action 'delete' on 'document:abc' is ALLOWED based on the current policy configuration.

---

**👤 You:**
> "Show me the health status and version of my Cerbos server."

**🤖 AI Agent:**
> The Cerbos server is currently 'READY' (v0.34.0). All systems are operational and the policy engine is active.

---

**👤 You:**
> "List all policies and tell me if there are any for the 'expense' resource."

**🤖 AI Agent:**
> I've retrieved the list of policies. You have 12 policies active, including 'resource.expense.v1', which handles authorization for expense reports.


## ❓ FAQ

**Q: Can I test if a specific user has access to a resource without writing code?**
Yes. You can ask the agent to use the `check_resources` tool by providing the principal (user) details and the resource you want to check. The agent will return the allowed or denied status based on your Cerbos policies.

**Q: How do I view all the authorization policies currently loaded in my Cerbos server?**
Simply ask the agent to 'list all policies'. It will invoke the `list_policies` tool (requires Admin credentials) and display the IDs of all active policies in your environment.

**Q: Can the AI help me generate filters for my database based on permissions?**
Yes, by using the `plan_resources` tool. The agent will generate a query plan (AST) that describes the conditions under which a user is allowed to access resources, which you can then apply to your database queries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cerbos-access-control](https://vinkius.com/mcp/cerbos-access-control)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cerbos (Access Control)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cerbos-access-control` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cerbos (Access Control)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cerbos-access-control": {
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
