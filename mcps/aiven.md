# Aiven MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aiven)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Manage Aiven cloud infrastructure — provision databases, manage projects, and monitor services directly from your AI agent.

## Description
Connect your **Aiven** account to any AI agent to manage your open-source data infrastructure through natural language. Take full control of your managed databases and cloud resources without leaving your chat interface.

### What you can do

- **Project & Account Management** — List, create, and inspect accounts and projects to organize your infrastructure environments.
- **Service Provisioning** — Deploy and manage services like PostgreSQL, MySQL, Redis, and Kafka across multiple cloud providers.
- **Networking & VPCs** — Configure and list project VPCs to ensure secure and isolated connectivity for your data services.
- **Billing & Organizations** — Monitor invoices, manage billing groups, and handle organization-level projects and users.
- **Team Collaboration** — Manage account teams and project access to streamline DevOps workflows.

### How it works

1. Subscribe to this server
2. Enter your Aiven API Token
3. Start managing your cloud infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — provision and scale database clusters directly from the terminal or IDE.
- **Backend Developers** — check service status and connection details without switching to the Aiven console.
- **SRE Teams** — automate infrastructure audits and monitor billing across multiple projects.


## Available Tools (30)
- **add_card**: Add credit card for user
- **create_account_team**: Create a new team in an account
- **create_account**: Create a new account
- **create_billing_group**: Create a billing group
- **create_project**: Create a project
- **create_project_vpc**: Create a VPC in a cloud for the project
- **create_service**: Create a new service
- **delete_account**: Delete empty account
- **delete_project**: Delete project
- **delete_service**: Terminate a service
- **get_account**: Get account details
- **get_project**: Get project details
- **get_service**: Get service information
- **invite_organization_user**: Invite a user to the organization
- **list_account_projects**: List projects belonging to account
- **list_account_teams**: List teams belonging to an account
- **list_accounts**: List accounts you have access to
- **list_billing_group_invoices**: Get invoices for a billing group
- **list_billing_groups**: List billing groups
- **list_cards**: List user credit cards
- **list_organization_projects**: List projects under the organization
- **list_organization_vpcs**: List organization VPCs
- **list_organizations**: List organizations the user belongs to
- **list_project_service_types**: List available service types for a project
- **list_project_vpcs**: List VPCs for a project
- **list_projects**: List projects
- **list_services**: List services in a project
- **update_account**: Update existing account
- **update_project**: Update project
- **update_service**: Update service configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aiven** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Aiven accounts I have access to."

**🤖 AI Agent:**
> I've retrieved your accounts. You have access to 'Primary-Org' (ID: acc123) and 'Dev-Sandbox' (ID: acc456).

---

**👤 You:**
> "Show me the service types available for project 'ecommerce-prod'."

**🤖 AI Agent:**
> For 'ecommerce-prod', you can deploy: pg (PostgreSQL), mysql, redis, kafka, opensearch, and clickhouse.

---

**👤 You:**
> "List all active services in the project 'data-analytics'."

**🤖 AI Agent:**
> I found 2 active services in 'data-analytics': 'pg-master' (PostgreSQL) and 'kafka-main' (Kafka). Both are currently in 'RUNNING' state.


## ❓ FAQ

**Q: Can I see my cloud network configurations and VPCs?**
Yes, use the `list_project_vpcs` tool with your project name to retrieve all Virtual Private Clouds configured for that environment.

**Q: Is it possible to automate the creation of a new database service?**
Absolutely. The `create_service` tool allows your agent to provision new database or messaging instances by providing the required configuration payload.

**Q: How do I check my billing history or invoices?**
You can use the `list_billing_group_invoices` tool to fetch a list of all invoices associated with a specific billing group ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aiven](https://vinkius.com/mcp/aiven)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aiven** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aiven` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aiven** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aiven": {
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
