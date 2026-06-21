# Clever Cloud (Developer PaaS API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clever-cloud-developer-paas-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Clever Cloud infrastructure—apps, add-ons, and deployments—directly from your AI agent.

## Description
Connect your **Clever Cloud** account to any AI agent and take full control of your PaaS resources through natural conversation.

### What you can do

- **Application Management** — List, create, and inspect your applications. Get detailed metadata and configuration for any specific app.
- **Add-on Provisioning** — List all your provisioned services like databases or Redis, and provision new ones on the fly.
- **Deployment Workflows** — Trigger new deployments for your applications directly from your chat or IDE.
- **Organization Control** — Manage multiple organizations, list their specific applications, and create new organizational units.
- **User Insights** — Retrieve your current user profile and settings to verify access levels.

### How it works

1. Subscribe to this server
2. Enter your Clever Cloud API credentials (Consumer Key, Secret, and Tokens)
3. Start managing your cloud infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly check application statuses and trigger deployments without leaving the terminal or editor.
- **Full-stack Developers** — provision databases (add-ons) and manage app configurations while writing code.
- **Technical Leads** — oversee multiple organizations and applications across the entire Clever Cloud ecosystem.


## Available Tools (14)
- **create_application**: Provide necessary configuration in the body.

Create a new Clever Cloud application
- **create_organization**: Provide configuration in the body.

Create a new organization
- **delete_application**: Delete an application
- **get_addon**: Get details of a specific add-on
- **get_application_logs**: Fetch application logs
- **get_application**: Get details of a specific application
- **get_current_user**: Get information about the current user
- **list_addons**: ).

List all your add-ons
- **list_applications**: List all your Clever Cloud applications
- **list_instances**: List running instances
- **list_organization_applications**: List applications in an organization
- **list_organizations**: List organizations you belong to
- **provision_addon**: Provide configuration in the body.

Provision a new add-on
- **trigger_deployment**: Trigger a deployment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clever Cloud (Developer PaaS API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Clever Cloud applications."

**🤖 AI Agent:**
> I've retrieved your applications. You have 3 active apps: 'frontend-prod' (ID: app_123), 'api-gateway' (ID: app_456), and 'worker-service' (ID: app_789).

---

**👤 You:**
> "Trigger a new deployment for application app_456."

**🤖 AI Agent:**
> Deployment triggered successfully for 'api-gateway' (app_456). The platform is now building and deploying your latest changes.

---

**👤 You:**
> "Show me the details of my provisioned add-ons."

**🤖 AI Agent:**
> You have 2 active add-ons: a PostgreSQL database (ID: addon_abc) and a Redis instance (ID: addon_xyz). Both are currently in 'running' status.


## ❓ FAQ

**Q: Can I trigger a new deployment for a specific application using this server?**
Yes! Use the `trigger_deployment` tool by providing the `appId`. You can optionally specify deployment options like a commit ID in the request body.

**Q: How do I see all the databases and services (add-ons) I have active?**
Simply use the `list_addons` tool. It will return a list of all provisioned add-ons, including databases and other managed services across your account.

**Q: Is it possible to manage applications within a specific organization?**
Yes. You can use `list_organizations` to find the `orgId`, and then use `list_organization_applications` to see only the apps belonging to that specific organization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clever-cloud-developer-paas-api](https://vinkius.com/mcp/clever-cloud-developer-paas-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clever Cloud (Developer PaaS API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clever-cloud-developer-paas-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clever Cloud (Developer PaaS API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clever-cloud-developer-paas-api": {
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
