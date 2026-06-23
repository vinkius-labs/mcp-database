# Aserto MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aserto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage authorization policies and evaluate access control decisions via Aserto — run Rego queries, check user permissions, and audit decision logs.

## Description
Connect your **Aserto** tenant to any AI agent to manage and evaluate fine-grained access control policies through natural conversation.

### What you can do

- **Authorization Checks** — Use `authz_is` to determine if a specific user identity is authorized to perform actions based on policy and resource context.
- **Rego Query Execution** — Execute custom Rego queries against your authorizer using `authz_query` to inspect policy data or evaluate complex logic.
- **Decision Trees** — Retrieve full decision tree values across policy modules with `authz_decisiontree` for UI logic or deep policy inspection.
- **Control Plane Management** — Send commands to connected Edge Authorizers using `control_plane_exec` to sync policy instances or directories.
- **Audit & Logging** — List and retrieve decision logs using `list_decision_logs` to maintain a clear audit trail of all authorization events.

### How it works

1. Subscribe to this server
2. Enter your Aserto Tenant ID and API URL
3. Provide your Authorizer and Decision Logs API keys
4. Start evaluating security policies directly from your AI assistant

### Who is this for?

- **Security Engineers** — quickly test policy changes and verify authorization logic without manual API calls
- **Backend Developers** — integrate and debug fine-grained access control (FGAC) during the development lifecycle
- **Compliance Officers** — audit decision logs and verify that access control policies meet regulatory requirements


## Available Tools (7)
- **authz_decisiontree**: Get decision tree values across all policy modules
- **authz_is**: Determine if a user is authorized to perform an action
- **authz_query**: Execute a general Rego query against the Authorizer
- **control_plane_exec**: Send commands to a connected Edge Authorizer
- **get_decision_log**: Retrieve a signed download URL for a specific log object
- **list_decision_logs**: List available decision log storage objects
- **query_decision_logs**: Query the last N decisions from decision logs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aserto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if user 'alice@example.com' is authorized to 'read' the 'document_123' resource using the 'peoplefinder' policy."

**🤖 AI Agent:**
> I've evaluated the policy via `authz_is`. The decision for 'read' is **true**. Alice has the required permissions based on the provided resource context.

---

**👤 You:**
> "Run a Rego query to list all roles defined in 'data.system.roles'."

**🤖 AI Agent:**
> Executing `authz_query`... The query returned the following roles: ['admin', 'editor', 'viewer'].

---

**👤 You:**
> "List the available decision logs for my current policies."

**🤖 AI Agent:**
> I've retrieved the decision logs using `list_decision_logs`. I found 3 storage objects available for the 'production-policy' ID. Would you like to inspect a specific log?


## ❓ FAQ

**Q: How do I verify a specific permission for a user?**
Use the `authz_is` tool. You need to provide the identity context (user), the policy context (the path to the rule), and any relevant resource context to get a boolean decision.

**Q: Can I execute complex Rego logic through the agent?**
Yes! The `authz_query` tool allows you to run any valid Rego query against your authorizer, enabling you to inspect data or evaluate custom logic on the fly.

**Q: Is it possible to trigger a policy sync on an Edge Authorizer?**
Yes. Use the `control_plane_exec` tool with the instance ID and the appropriate command (e.g., `{"discovery": {}}`) to manage your connected authorizers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aserto](https://vinkius.com/mcp/aserto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aserto** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aserto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aserto** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aserto": {
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
