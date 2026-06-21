# Railway MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/railway-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage cloud deployments via Railway — list projects, inspect services, track deployments and manage variables and volumes from any AI agent.

## Description
Connect your **Railway** account to any AI agent and take full control of your cloud deployments through natural conversation.

### What you can do

- **Project Discovery** — List all projects and retrieve their details including names, descriptions and timestamps
- **Environment Management** — View all deployment environments (production, staging, development) per project
- **Service Inspection** — List all services (containers, databases, plugins) within a project, optionally filtered by environment
- **Deployment Tracking** — View deployment history with status (success, failed, deploying) for any service
- **Variable Management** — List, set and delete environment variables for services in specific environments
- **Volume Audit** — List persistent storage volumes with their sizes and associated services
- **Domain Management** — Review custom domains and their SSL certificate status for any service

### How it works

1. Subscribe to this server
2. Enter your Railway Personal Access Token
3. Start managing your cloud deployments from Claude, Cursor, or any MCP-compatible client

Stop clicking through the Railway dashboard to check deployment status or manage environment variables. Your AI acts as a dedicated cloud operations engineer.

### Who is this for?

- **Developers** — inspect services, track deployments and manage environment variables without leaving your IDE
- **DevOps Engineers** — audit project configurations, review deployment statuses and manage persistent volumes
- **Team Leads** — monitor project health, environment segregation and variable security across services


## Available Tools
- **delete_variable**: Provide the service_id, environment_id and variable name. WARNING: the variable will no longer be available to deployments after deletion.

Delete an environment variable from a Railway service
- **list_deployments**: Each deployment has an ID, status (success, failed, deploying, removed), creation and update timestamps. Use the service_id from list_services.

List deployments for a Railway service
- **list_domains**: Each domain has an ID, the domain string and SSL status (verified, pending, failed). Use this to audit which services are accessible via custom URLs.

List custom domains for a Railway service
- **list_environments**: g. production, staging, development) configured within a specific Railway project. Each environment has its own set of services, variables and deployments. Use the project_id from list_projects.

List environments in a Railway project
- **get_project**: Provide the project ID obtained from list_projects.

Get details for a specific Railway project
- **list_projects**: Each project groups related services, environments and deployments together. Returns project ID, name, description and timestamps. Use this as the starting point for all Railway operations.

List all Railway projects
- **list_services**: Optionally filter by environment_id to see services in a specific environment only. Each service represents a deployable unit like a web app, API, database or Redis instance.

List services in a Railway project
- **set_variable**: Requires the service_id, environment_id, variable name and value. The variable will be available to all deployments of that service in the given environment.

Set an environment variable for a Railway service
- **list_variables**: Each variable has a name and scope (service, environment, project). Variable values are NOT returned for security — only names and scopes. Use service_id and environment_id from their respective list tools.

List environment variables for a Railway service
- **get_viewer**: Use this to verify which account the API token belongs to.

Get current authenticated Railway user details
- **list_volumes**: Each volume has an ID, name, associated service ID and size in gigabytes. Volumes provide persistent storage that survives deployments and restarts.

List persistent volumes in a Railway project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Railway** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all my Railway projects and their services."

**🤖 AI Agent:**
> I found 3 projects: 'my-api' (2 services: api-web, postgres), 'frontend-app' (1 service: nextjs), and 'worker-service' (1 service: redis). Would you like the deployment history for any specific service?

---

**👤 You:**
> "Set the DATABASE_URL variable for my api-web service in production."

**🤖 AI Agent:**
> Done! I've set the `DATABASE_URL` environment variable for the api-web service in the production environment. The new value will be available on the next deployment.

---

**👤 You:**
> "What's the deployment status of my api-web service?"

**🤖 AI Agent:**
> The api-web service has 4 deployments. The most recent one deployed successfully 2 hours ago with image tag v2.3.1. The previous deployment (v2.3.0) failed due to a missing environment variable. Would you like more details?


## ❓ FAQ

**Q: How do I create a Railway Personal Access Token?**
Log in to the [**Railway Dashboard**](https://railway.com/dashboard), go to **Account Settings** > **Tokens**, and click **Create Token**. You can create a no-workspace token for broad access or a project-scoped token for limited access. Copy the token immediately — it won't be shown again.

**Q: Can I manage environment variables via the agent?**
Yes! Use `list_variables` to see all variable names (values are hidden for security) for a service in an environment. Use `set_variable` to create or update a variable with a name and value, and `delete_variable` to remove one. You'll need the service_id and environment_id from the list tools.

**Q: What types of services does Railway support?**
Railway supports any containerized service: web applications (Node.js, Python, Go, Rust, Java), databases (PostgreSQL, MySQL, Redis, MongoDB), message brokers and custom Docker images. Each service is deployed as an isolated container with its own environment variables, domains and persistent volumes.

**Q: How do I find my service_id and environment_id?**
Use `list_projects` to get your project_id, then `list_environments` with that project_id to get the environment_id. Next, use `list_services` with the project_id (and optionally environment_id) to get the service_id. These IDs are required for variable, deployment and domain operations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/railway-alternative](https://vinkius.com/mcp/railway-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Railway** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `railway-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Railway** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "railway-alternative": {
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
