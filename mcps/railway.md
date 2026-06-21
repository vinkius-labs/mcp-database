# Railway MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/railway)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Equip your AI with direct access to your Railway infrastructure — manage projects, deployments, services, and environment variables.

## Description
Connect your **Railway** cloud infrastructure to an AI agent, streamlining operations directly from your chat terminal. By configuring this integration, the AI gains programmatic management over your active deployments and environments.

### What you can do

- **Project Management** — Create new projects or query existing ones to assess active cloud architectures without opening the web dashboard.
- **Deployment Oversight** — Review build statuses, trigger new deployments, and read rollout logs to ensure stable releases.
- **Service Configuration** — List, update, or restart operational services mapped within your Railway projects securely.
- **Environment Variables** — Manage sensitive configuration keys by securely pulling, updating, or syncing environment values across instances.

### How it works

1. Enable the MCP server integration for Railway.
2. Add your Railway API Token to the configuration.
3. Ask your AI to list projects, fetch deployment health, or handle your services seamlessly.

### Who is this for?

- **DevOps Engineers** — Restart unhealthy containers or verify environment variables quickly from within a VS Code interface.
- **Fullstack Developers** — Trigger deployments after wrapping up a pull request and oversee the operational results interactively.
- **System Administrators** — Conduct fast routine checks on service connectivity scaling without having to rely entirely on separate client applications.


## Available Tools
- **create_project**: Creates a new Railway project
- **delete_project**: This action is irreversible.

Deletes a Railway project
- **get_project**: Retrieves details for a specific Railway project
- **get_service_instances**: Retrieves runtime configuration for a service
- **list_deployments**: Lists deployments for a specific project, environment, and service
- **list_projects**: Lists all Railway projects accessible by the token
- **list_variables**: Lists environment variables for a service
- **restart_service**: Restarts a running service instance
- **trigger_deploy**: Triggers a new deployment for a service
- **whoami**: Retrieves the authenticated Railway user profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Railway** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects on my Railway account."

**🤖 AI Agent:**
> I retrieved your projects using `list_projects`. You currently have two active projects: 'ECommerce Backend' (ID: prj_xyz123) and 'Auth Service' (ID: prj_abc789).

---

**👤 You:**
> "Restart the deployment for the ECommerce Backend service."

**🤖 AI Agent:**
> I executed `restart_service`. The service 'ECommerce Backend' successfully began recycling its containers. You can track the current startup health via the logs.

---

**👤 You:**
> "Has the latest Production build finished yet?"

**🤖 AI Agent:**
> Using the `get_deployments` query, I found the latest deployment status. The Production build on service 'sv_222' successfully completed 4 minutes ago and is currently in a 'SUCCESS' state.


## ❓ FAQ

**Q: How do I create a Railway API token?**
Log into your main Railway dashboard. Navigate to your Account Settings and head to the 'Tokens' section. Generate a standard Personal Access API Token, copy it definitively, and paste it into the secure configuration field provided by the MCP integration here.

**Q: Can I target specific environments (like Staging vs Production)?**
Yes. Each API operation supports passing explicit `project_id` and `environment_id` variables, ensuring the AI performs operations strictly inside your requested boundaries.

**Q: Is restarting a service destructive?**
It behaves identically to clicking 'Restart' on the Railway dashboard. It forces an immediate container recycle for the specific service based on the last successful build.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/railway](https://vinkius.com/mcp/railway)
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
3. Set Type to "SSE", enter `railway` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Railway** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "railway": {
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
