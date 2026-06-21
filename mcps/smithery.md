# Smithery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smithery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

AI MCP registry: discover, search, and connect MCP servers to your agents via Smithery.

## Description
### What you can do

Connect AI agents to the Smithery Registry for comprehensive MCP server discovery and management:

- **Search MCP servers** — find servers by name, description, or tags with semantic search
- **Get server details** — review metadata, verification status, and user counts
- **Discover tools** — list all tools (functions) exposed by any registered MCP server
- **Discover resources** — list all data resources available from MCP servers
- **Discover prompts** — list all prompt templates exposed by MCP servers
- **Create connections** — connect to MCP servers via Smithery Connect with automatic OAuth handling
- **Manage connections** — list, inspect, and remove MCP server connections
- **Generate service tokens** — create scoped, time-limited tokens for frontend/agent access
- **View analytics** — monitor server usage, adoption trends, and performance metrics

### How it works

1. **Get your Smithery API key** from smithery.ai/account/api-keys
2. **Ask your AI agent** to search the registry, discover server capabilities, or create connections
3. **Natural language commands** replace manual Smithery dashboard navigation
4. **Zero OAuth configuration** — Smithery Connect handles tokens and sessions automatically

### Who is this for?

Essential for **AI application developers**, **agent architects**, **platform engineers**, **MCP server publishers**, and **enterprise AI teams** building with the Model Context Protocol. Let AI agents discover relevant MCP servers, review their capabilities, create managed connections, and monitor usage analytics. Perfect for teams integrating multiple MCP servers who want to streamline server discovery, eliminate manual OAuth configuration, and enable AI-driven MCP ecosystem management.


## Available Tools
- **create_connection**: Smithery handles OAuth, tokens, and sessions automatically. Requires the server namespace and connection configuration (mcpUrl, optional headers, metadata). Returns the connection ID, status, and server info. Use this to integrate MCP servers into your applications without managing authentication complexity.

Create a new connection to an MCP server via Smithery Connect
- **create_service_token**: The token has limited permissions defined by the policy (namespaces, resources, operations, metadata, TTL). Returns the token string. Use this to provide secure, time-limited access to MCP servers without exposing your main API key.

Generate a scoped service token for frontend/agent access to MCP servers
- **delete_connection**: This action cannot be undone. Requires namespace and connection ID. Use this to clean up unused connections or revoke access.

Remove an MCP server connection
- **get_connection**: Requires namespace and connection ID. Use this to review connection details or troubleshoot connectivity issues.

Get detailed information about a specific MCP connection
- **get_server_analytics**: Requires the server qualified name. Use this to monitor server adoption, identify usage trends, or troubleshoot performance issues.

Get usage analytics for a specific MCP server
- **get_server_details**: Requires the qualified name (e.g., "smithery/hello-world" or "github/github") from search_servers results. Use this to review server capabilities before connecting.

Get detailed information about a specific MCP server from the Smithery registry
- **get_server_prompts**: Returns prompt names, descriptions, and argument definitions. Requires the server qualified name. Use this to discover reusable prompt workflows available from the server.

List all prompt templates exposed by a specific MCP server
- **get_server_resources**: Returns resource URIs, names, descriptions, and MIME types. Requires the server qualified name. Use this to understand what data the server provides read access to.

List all resources exposed by a specific MCP server
- **get_server_tools**: Returns tool names, descriptions, input schemas, and annotations. Requires the server qualified name. Use this to understand what actions the server can perform before connecting it to your agents.

List all tools exposed by a specific MCP server
- **list_connections**: Returns connection IDs, names, statuses, creation dates, and metadata. Use this to audit which connections are active, review connection configurations, or identify unused connections.

List all connections for a specific MCP server namespace
- **search_servers**: Returns matching servers with qualified names, descriptions, verification status, user counts, and deployment info. Use optional filters to narrow by namespace, verified status, or deployment state. Results include pagination metadata. Use this as the first step to discover available MCP servers before connecting or installing them.

Search the Smithery registry for MCP servers by name, description, or tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smithery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for verified GitHub-related MCP servers"

**🤖 AI Agent:**
> I'll search the Smithery registry for verified GitHub MCP servers.

---

**👤 You:**
> "Show me all tools exposed by the Stripe MCP server"

**🤖 AI Agent:**
> I'll retrieve the complete tool catalog from the Stripe MCP server.

---

**👤 You:**
> "Create a connection to the Slack MCP server for my workspace"

**🤖 AI Agent:**
> I'll create a managed connection to the Slack MCP server through Smithery Connect.


## ❓ FAQ

**Q: Do I need a Smithery account to use this MCP server?**
Yes, you need a free Smithery account to generate an API key. Sign up at smithery.ai, then go to Account Settings > API Keys to create your key. The key gives access to the registry search, server details, and connection management features.

**Q: How does Smithery Connect handle OAuth for MCP servers?**
Smithery Connect automatically handles OAuth flows, token refresh, and session management for MCP servers that require authentication. You don't need to configure redirect URIs, client IDs, or manage token expiration. Simply create a connection and Smithery manages the authentication lifecycle, providing your agents with seamless access.

**Q: Can I search for verified MCP servers only?**
Yes! Use the verified filter in the search_servers tool by setting verified=true. This returns only servers that have been verified by Smithery, ensuring higher quality and security standards. Verified servers display a verification badge and have undergone additional review.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smithery](https://vinkius.com/mcp/smithery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smithery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `smithery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smithery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smithery": {
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
