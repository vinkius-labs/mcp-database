# Nile (PostgreSQL for Multi-Tenant Apps) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nile-postgresql-for-multi-tenant-apps)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Manage tenant-aware databases via Nile — provision B2B tenants, monitor DB metrics, and audit user access.

## Description
Connect your **Nile** account to any AI agent and take full control of your tenant-aware PostgreSQL infrastructure, B2B tenant isolation, and database performance through natural conversation.

### What you can do

- **Database Orchestration** — List high-level PostgreSQL targets and retrieve detailed configuration JSON, including storage sizes and state tracking directly from your agent
- **Virtualized Multi-Tenancy** — Instantly provision and manage highly isolated virtual tenant boundaries (shards) to support multi-tenant SaaS architectures automatically within Postgres
- **Operational Performance** — Pull exact monitoring metrics reflecting true active connections, storage exhaustion layers, and compute utilization tracked over your database instances
- **User Lifecycle Audit** — Enumerate globally tracked users and correlate their identities to internal virtual tenants to ensure accurate cross-tenant access control
- **Tenant Discovery** — Query the strict virtual boundaries natively splitting tenant data to isolate exact SaaS tenant IDs before performing deep data inspections
- **Metadata Retrieval** — Deep-dive into specific Database endpoints to retrieve precise structural representations and operational state vectors instantly

### How it works

1. Subscribe to this server
2. Enter your Nile API URL and API Key
3. Start managing your multi-tenant infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SaaS Developers** — provision new B2B tenants and verify database isolation through natural conversation without manual CLI scripts
- **Database Engineers** — monitor storage exhaustion and active connection counts across multiple Nile databases directly from your workspace
- **Backend Architects** — audit user identity mappings and manage tenant-specific data sharding efficiently to maintain high-scalability standards


## Available Tools
- **list_databases**: Identifies root connectivity endpoints (name bindings) necessary for querying physical data.

List high-level tenant-aware PostgreSQL databases provisioned on Nile
- **get_database**: Get configuration and state details for a specific Nile Database
- **list_tenants**: List active virtualized B2B tenants living within a Nile database
- **create_tenant**: Provision a new highly isolated virtual Tenant boundary inside the DB
- **list_users**: Enumerate globally tracked users capable of accessing tenant slices
- **get_metrics**: Pull exact operational performance numbers tracking Database strain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nile (PostgreSQL for Multi-Tenant Apps)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active databases in my Nile account"

**🤖 AI Agent:**
> I've retrieved your Nile databases. Highlights include 'production-v1' (Status: Active), 'staging-cluster', and 'analytics-db'. Would you like to see the configuration details or metrics for the production database?

---

**👤 You:**
> "Create a new isolated tenant called 'Acme-Corp' in the 'production-v1' database"

**🤖 AI Agent:**
> Provisioning virtual tenant boundary… Success. I've created 'Acme-Corp' (ID: ten-12345) inside your production database. This tenant is now logically isolated and ready for data sharding. Would you like me to verify the initial metrics for this new boundary?

---

**👤 You:**
> "Show me the compute and storage metrics for database 'production-v1'"

**🤖 AI Agent:**
> Retrieving performance metrics… For 'production-v1', you currently have 45 active connections out of a 100 limit. Storage usage is at 2.4 GB (12% of cap). Compute utilization averaged 15% over the last hour. Everything looks healthy. Would you like a list of active users?


## ❓ FAQ

**Q: How does Nile handle tenant isolation through the agent?**
Nile uses virtualized multi-tenancy. When your agent uses the `create_tenant` tool, Nile's control plane automatically generates a distinct routing logic container within Postgres, ensuring that data for the new B2B client is logically separated from other tenants.

**Q: Can I monitor the health of my Nile databases through a conversation?**
Yes. Use the `get_metrics` tool with a specific database name. Your agent will retrieve real-time operational performance numbers, including active connections and compute utilization, helping you identify load spikes or storage exhaustion instantly.

**Q: Can my agent list all registered users and see which tenants they belong to?**
Absolutely. Use the `list_users` tool to enumerate all identities natively authenticated within Nile. Your agent will report the user mappings to internal virtual tenants, making it easy to audit cross-tenant access control across your entire database ecosystem.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nile-postgresql-for-multi-tenant-apps](https://vinkius.com/mcp/nile-postgresql-for-multi-tenant-apps)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nile (PostgreSQL for Multi-Tenant Apps)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nile-postgresql-for-multi-tenant-apps` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nile (PostgreSQL for Multi-Tenant Apps)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nile-postgresql-for-multi-tenant-apps": {
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
